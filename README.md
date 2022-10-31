# Sign Project
<img width="70%" src="https://user-images.githubusercontent.com/100760303/198922437-11f3ded8-6f1b-4f73-8118-98b1d27cf11c.png"/>
<br>

## 상세 내용
영어 알파벳과 숫자 수화 이미지를 분류하고 실시간으로 수화를 예측합니다. 단, 숫자 데이터의 경우 제스쳐 모션으로 인해 9(J)와 25(Z)의 경우는 제외합니다.
청각 장애인분들이 컴퓨터 비전 애플리케이션을 사용할 때 더 나은 의사소통을 할 수 있었으면 하는 마음에 프로젝트를 진행하였습니다.

<br>

### Image Classification
숫자 이미지를 Tesorflow의 EfficientNetB0 모델을 사용하여 분류하였고, 알파벳 이미지는 직접 층을 쌓은 모델을 사용하여 분류하였습니다.

### OpenCV를 활용한 Hand Detection과 Real Time
<img width="70%" src="https://user-images.githubusercontent.com/100760303/198994526-b82b6217-9f45-4f1b-ae4f-694799418fdb.PNG"/>
<img width="70%" src="https://user-images.githubusercontent.com/100760303/198994599-dc4940e5-e39c-46c4-a83b-94e0199c95a0.PNG"/>
<br>

다운 받은 이미지 데이터만으로는 실시간 예측을 할 때 성능이 나아지지 않는다는 문제점을 발견하였습니다. 따라서 OpenCV를 활용해 Hand Detection으로 수화 제스쳐의 모션을 따고 해당 이미지들을 직접 촬영하고 수집하여 모델링을 다시 진행하였습니다. 그 결과 실시간으로 수화를 예측할 때 성능이 좋아진 것을 확인할 수 있었습니다. 위의 두 사진이 직접 수집한 이미지 데이터입니다.

<br>

## 결과
<img width="50%" src="https://user-images.githubusercontent.com/100760303/198924488-e7c28b35-98f8-4e20-9ef6-f2b1bdc0912f.jpg"/>
<img width="50%" src="https://user-images.githubusercontent.com/100760303/198924592-902c3c66-2e09-4ac7-ba9c-24f701ede75a.jpg"/>
<img width="50%" src="https://user-images.githubusercontent.com/100760303/198924662-e3b9a2a4-5a11-42be-841f-460116eeaec3.jpg"/>
<br>

## Streamlit
https://eunjida-streamlit-sign-language-0--sign-language-sw6rhz.streamlitapp.com/
