[DNN 방식 얼굴 detection] OpenCV 라이브러리 사용
- Harr보단 정확도가 높아졌으나, 아직도 얼굴 각도, 해상도 등의 영향으로 얼굴을 검출 못하는 경우가 있었음
- 미리 학습된 모델을 받아(caffemodel), deploy.prototxt.txt(구조) 이를 코드로 실행하여 얼굴 탐색함   
- 추가적으로 이미지나 영상에서 탐색한 얼굴에 사각형 그려줌   


detection 값(4차원 배열)       
detection.shape[2] : 최대 박스 크기   
detection의 3번째 값의 의미 : 얼굴일 확률   
detection의 4번째 값의 의미 : x 좌표의 위치   
detection의 5번째 값의 의미 : 얼굴의 폭   
detection의 6번째 값의 의미 : 얼굴의 높이   

confidenct = detections[0, 0, i, 2] 각 이미지마다의 얼굴일 확률   
min confidence와 비교하여 이보다 크면 box를 그려준다.   
box 그릴 때는 detection에서 찾은 값에 전체 width, height를 곱해준다, box 좌표 획득 가능.      
