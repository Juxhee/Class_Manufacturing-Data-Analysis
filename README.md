## 전자제조 데이터 분석 수업 : 프레스 공정 불량품 예측을 위한 제조 데이터 분석 및 시각화 프로젝트


### 분석 목적
- 프레스 내 환경 데이터와 프레스 공정 내에서의 불량 정보 데이터를 활용해 최종 제품의 불량품 여부 예측에 대한 인사이트 도출



### 데이터셋

- 인공지능 중소벤처 제조 플랫폼 KAMP 의 프레스기 AI 데이터셋 활용 
- https://www.kamp-ai.kr/
1) 작업시간 동안 프레스 공정 내 환경 데이터 
`PressRawDataset.csv`

2) 작업시간 동안 프레스 공정 내 불량 유형 별 불량 발생 개수 데이터 
`PressError.csv`

</br>


### EDA
`press_eda.ipynb`
</br>

#### 상관관계 분석 
![image](https://user-images.githubusercontent.com/60679596/146933677-9aef1a6f-a85b-4cd4-9ef0-e2cc8df46d41.png)


#### 날짜 별 불량품 추이 확인

![image](https://user-images.githubusercontent.com/60679596/146933763-4175ef55-727c-47ce-9102-9a0c9eb6b762.png)

</br>
</br>

### 클러스터링 

#### 목적 : 프레스 공정 내 품질이 최종 완제품의 불량여부에 미치는 영향을 알아보고자 클러스터링을 통해 클러스터 별 공정 내 특성을 확인해보고자 함
#### 사용된 알고리즘 : Kmeans, DBSCAN, Mean Shift

</br>

- 분석 1 : Kmeans
`clustering_kmeans.ipynb`
</br>

![image](https://user-images.githubusercontent.com/60679596/146933870-456f68c3-0d49-45b5-8c27-e5fa9c7065a8.png)

![image](https://user-images.githubusercontent.com/60679596/146933930-44a9f041-1c1b-4fa0-b232-43887d399a68.png)

![image](https://user-images.githubusercontent.com/60679596/146933950-9eb01f76-0257-4243-8585-281b43bc25ba.png)

</br>

- 분석 2 : DBSCAN
`clustering_DBSCAN.ipynb`
</br>

![image](https://user-images.githubusercontent.com/60679596/146934000-6ea300b0-041c-4e41-922e-ae9c301a5e84.png)

![image](https://user-images.githubusercontent.com/60679596/146934010-7371813e-95bf-455f-97e0-0253687926ce.png)

- 분석  3 : Mean Shift
`clustering_MeanShift.ipynb`
</br>

![image](https://user-images.githubusercontent.com/60679596/146934047-561686c1-42e7-4df0-8570-bd37628778dd.png)

![image](https://user-images.githubusercontent.com/60679596/146934059-414fb7e1-312e-44d9-9c2f-8764b0d7017f.png)

</br>
</br>

#### Kmeans 기반 클러스터링 결과 시각화 


![image](https://user-images.githubusercontent.com/60679596/146934111-f19b8de0-4bc0-448b-956b-adebd77dc9b6.png)

![image](https://user-images.githubusercontent.com/60679596/146934130-b84fb46a-7199-4fdd-b274-08eac1a21f44.png)

![image](https://user-images.githubusercontent.com/60679596/146934141-75296636-6210-4a6c-bd46-27bc35bca354.png)


