[Dlib 방식 얼굴 detection] OpenCV 라이브러리 사용   

- pip install cmake   
- pip install dlib   
- pip install face_recognition   
   
인식할 대상의 얼굴 사진 10 ~ 25장 준비    
준비한 사진의 특징 추출(추가 전처리 : face_landmark, face_alignment)   

Harr보단 정확도가 높아졌으나, 아직도 얼굴 각도, 해상도 등의 영향으로 얼굴을 검출 못하는 경우가 있었음
미리 학습된 모델을 받아(caffemodel), deploy.prototxt.txt(구조) 이를 코드로 실행하여 얼굴 탐색함
