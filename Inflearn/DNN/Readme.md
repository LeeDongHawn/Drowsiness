[DNN 방식 얼굴 detection] OpenCV 라이브러리 사용
- Harr보단 정확도가 높아졌으나, 아직도 얼굴 각도, 해상도 등의 영향으로 얼굴을 검출 못하는 경우가 있었음
- 미리 학습된 모델을 받아(caffemodel), deploy.prototxt.txt(구조) 이를 코드로 실행하여 얼굴 탐색함
- GUI 사용 시 직접 파일을 선택하여 결과를 볼 수 있음
