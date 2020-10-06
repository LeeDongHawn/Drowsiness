[Dlib 방식 얼굴 detection] OpenCV 라이브러리 사용   

- pip install cmake   
- pip install dlib   
- pip install face_recognition   
   
1. Pickle   
- 인식할 대상의 얼굴 사진 10 ~ 25장 준비(son, tedy 따로)          
- 준비한 사진의 특징 추출(추가 전처리 : face_landmark, face_alignment 등을 사용 가능)   
- 특징들을 모아놓은 pickle 파일 생성    

2. Image Recognition    
- 얼굴 인식하려는 이미지에서 마찬가지로 특징을 뽑아내고, 기존에 존재하는 pickle 파일 간 비교(k-nearest-neighbors 사용)   
- classification 방법으로 KNN은 높은 정확도를 보이지 못함. -> Support Vector Machine 등의 방법을 사용   
- 추가적으로 새로운 이미지에서 얼굴에 사각형을 그려주거나 동작 시간 등을 측정   

Harr, DNN 보다 높은 얼굴 인식 정확도를 보임   
