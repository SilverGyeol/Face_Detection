# Face_Detection
저장된 이미지에 맞는 얼굴을 찾아서 인식하는 프로그램

# 1. 데이터 불러오기.
1. 저장된 라이브러리를 가져와서 컴퓨터에 정보를 입력합니다.
![image](https://user-images.githubusercontent.com/94829177/173345779-74505182-4030-4a83-93f7-d85bc3d9cf40.png)

# 2. images 폴더에서 이미지 불러오기.
1. images 폴더에서 이미지를 가져와서 이미지 사이즈를 원하는 크기로 지정합니다.
2. 이미지에서 얼굴이 있는 부분을 예측하여 변수 "predictions" 에 저장합니다.
![image](https://user-images.githubusercontent.com/94829177/173348049-03631e72-5120-4eab-b4fc-46ba9c7158a2.png)

# 3. 이미지에 있는 얼굴을 인식하여 경계 상자를 그린다.
1. 이미지에서 예측확률 0%보다 큰 모든 이미지 주변에 경계 상자를 그립니다.
> 예측확률 범위가 0%보다 큰 것에 경계 상자를 그리기 때문에 정확도가 낮습니다.

![image](https://user-images.githubusercontent.com/94829177/173349170-9e0103a8-2350-4939-b85b-617cf9597065.png)
![image](https://user-images.githubusercontent.com/94829177/173349319-50dd7426-6637-4b63-94d3-a3047cd8d393.png)
<br><br><br>
2. 이미지에서 예측확률 50%보다 큰 모든 이미지 주변에 경계 상자를 그린다.
> 예측확률 범위가 50%보다 큰 것에 경계 상자를 그리기 때문에 정확도가 높습니다.

![image](https://user-images.githubusercontent.com/94829177/173350755-0f5c5820-2078-43b4-b21f-53034079615b.png)
![image](https://user-images.githubusercontent.com/94829177/173350639-076c103f-5cc6-4f48-9710-c0b7de4057a7.png)

# 4. 웹캠을 이용하여 실시간 영상에서 얼굴을 인식한다.
1. images 폴더에 저장되어있는 이미지와 유사도가 높은 형체 주변에 경계 상자를 띄웁니다.

