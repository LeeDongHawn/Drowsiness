Inflearn - [OpenCV] 파이썬 딥러닝 영상처리 프로젝트 - 손흥민을 찾아라! 강의를 듣고 정리함   
source_code : https://www.creapple.com/home/main   
작업환경 : python(jupyter notebook)   

Face Detection 방법
- Harris corner detector
- Deep Neural Networks (dnn module)
- Dlib c++ library

강화 - Face Landmark(Dlib)         
https://github.com/davisking/dlib-models (Model)      

강화 - Face Alignment(Dlib)     
기울어진 얼굴을 바로 해주기 위함(인식률 향상)   
1) 이미지의 특징점 찾기        
2) 얼굴 Alignment를 통해 인식률 향상시키기         
3) 동일한 크기로 crop하기   
