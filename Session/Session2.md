# Session 2. Create VM in Azure Machine Learning Studio

해당 시작부분이 어색하신 분들은 [이전 세션](./Session1.md) 부분을 다시 보는 것을 추천드립니다 !

- 해당 화면에서 중앙 아래의 `studio 시작하기` 버튼을 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/fd4442ca-f85a-495b-9566-f3bf57d3054a)

- 그러면 다음과 같은 창이 뜨는데, 이것이 바로 Machine Learning Studio의 모습입니다 !
  > Tip 🙂 : 왼쪽 탭의 여러 가지 작업들을 나중에 시간될 때 클릭해 보는 것을 추천드립니다 👍
  
  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/c2d7ad0e-76ac-44d0-9a57-11f083c311a0)

- 왼쪽 탭에서 컴퓨팅 탭을 클릭합니다.
- 그리고 중앙 하단의 `새로 만들기`를 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/9e42fcbf-5ce6-4314-afb8-06c6df06874a)

- 먼저, 다음 그림과 같이 컴퓨팅 이름을 작성해야 합니다. (마음대로 작성하셔도 됩니다 !)

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/db991374-8b54-49ae-8625-8bfc7aeb69ad)

- 컴퓨팅 이름을 작성할 때, 다음 요구사항을 충족해야 합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/2d76949f-2ef3-4b3c-95bf-81033af0eb29)

- 컴퓨팅 이름을 작성한 후, virtual machine type를 cpu로 설정합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/9ddf6d31-87a7-40f9-a072-33e17ee49e58)

- 가상머신 크기는 간단한 scikit-learn 실습을 진행하므로 `Standard_DS3_v2`를 선택해줍니다.
- 그리고, 하단의 `검토+만들기`를 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/65e2e954-ae1a-47f7-8a64-7aab0114e6e1)

- 마지막 검토 창에서 선택했던 조건들을 마지막으로 확인할 수 있습니다.
- 하단의 만들기 버튼을 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/fec7186c-72af-47a7-97d8-ee770836c153)

- 그러면, 가상 머신이 생성 중인 것을 확인할 수 있습니다.
- 가상 머신이 생성될 때까지 약 2~3분 가량 걸립니다.
  > Tip 😄 : 컴퓨터 사양에 따라 가상 머신이 생성되는 시간이 다릅니다...

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/40d08f5d-91a9-4470-a8b1-9609e9e84083)

- 생성이 완료되면 상태에 "실행 중" 이라는 표시가 되어있습니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/0cabe9ad-902f-47e9-9910-2e761722da5d)

# Session 2. Summary

해당 세션에서는 Azure Machine Learning Studio에서 VM을 생성하는 과정을 확인해봤습니다.

다음 세션에서는 본격적으로 Desinger 탭에서 파이프라인을 구축해보려고 합니다 !

[여기](./Session3.md)를 클릭해서 흥미로운 다음 세션을 시작해보세요 !
