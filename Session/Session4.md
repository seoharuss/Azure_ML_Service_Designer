# Preview the data of the pipeline model

만약 해당 세션의 첫 화면이 어색하시다면 [이전 세션](./Session3.md)을 다시 확인해보시는걸 추천합니다 !

- 스스로 만들어 본 파이프라인의 전체 모습입니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/40fda552-f463-41ac-a719-e6ef4bc5439c)

- 파이프라인 구축이 완료가 되면 모든 컴포넌트 왼편에 초록색으로 표시가 됩니다.
- `Split Data` 컴포넌트의 `o` 아이콘에 마우스 오른쪽 버튼을 클릭해서 `데이터 미리보기`를 클릭합니다.
- 데이터가 초기에 설정했던대로 7:3 비율로 분할되어 있는 것을 확인할 수 있습니다.
  > 언제 7:3으로 분할했는지 기억이 안나시나요? [이 부분](./Session3.md)에서 한 것을 다시 확인해보세요 !

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/4ed4d2fe-acf4-482f-9d59-34c18883dc0d)

- 다시 돌아와서, 똑같이 `Score Model` 컴포넌트의 `o` 아이콘에 마우스 오른쪽 버튼을 눌러서 `데이터 미리보기`를 클릭해보면, 모델이 예측한 정보를 확인할 수 있습니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/b4049c72-cede-4c6b-a1c5-909d5877209a)

- 마찬가지로 `Evaluate Model` 컴포넌트의 `o` 아이콘에 마우스 오른쪽 버튼을 눌러서 `데이터 미리보기`를 클릭합니다.
- 그러면 데이터 결과가 가로로 길게 나오는 것을 확인할 수 있습니다.
  > 데이터 결과를 맨 오른쪽으로 쭉 스크롤을 해보면 `Cofficient of Determination`이 나오는데, 해당 내용은 정확도를 표현한 것이므로 정확도가 **0.999997**인 것을 확인할 수 있습니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/ef1466f2-0a38-4a58-a515-2690d0232862)

- 이로써 근속연수에 따른 연봉 예측 모델이 만들어졌습니다.
- 이제 이 모델을 배포해 보려고 합니다 !
- 상단에 `게시` 버튼을 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/c6dc2b57-9fda-4753-be0b-082b338f8a8d)

- 여기서PipelineEndpoint 옵션을 `새로 만들기`로 클릭하고, 이름은 원하는대로 지어주시면 됩니다.
- 그리고 `게시` 버튼을 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/5ab7afba-816b-4824-9977-a13a4f493c2c)

- 그러면 배포가 진행되고, 배포가 완료되면 상단의 알림창에 본인이 지정한 Pipeline Endpoint 이름(예 : newnewnew)의 링크를 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/f6162081-1340-4615-aaef-7e40c8efa820)

- 그러면 본인이 구축한 파이프라인과 함께 오른쪽 파이프라인 엔드포인트 개요에 개인의 `REST 엔트포인트`와 `REST 엔드포인트 설명서`가 나와있습니다.
  > "파이프라인 엔드포인트 개요"를 스크롤 하면서 확인하시면 됩니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/ba9ac21d-5546-4e91-9c08-7ff2e6ee26f4)

### 이를 활용하는 방법
- ChatGPT에게 엔드포인트 설명서를 복사 붙여넣기하여 "이 엔드포인트를 활용하여 파이썬 코드를 만들어줘"와 같이 요구하여 코드를 간편하게 얻을 수 있습니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/e53d315d-16ec-4d1b-a12d-2e8710b8c162)

### 파이프라인 관리
- 다시 `디자이너` 탭을 클릭하면 자신이 디자이너로 만들었던 파이프라인을 확인할 수 있습니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/d3eeedca-9257-429d-bf6e-8efe8cb58d1d)

# Session 4. Summary
해당 세션에서는 파이프라인이 구축된 후, 머신러닝의 결과 데이터를 확인해보는 방법과 이를 배포하고, 활용하는 예시에 대해 확인해봤습니다.

축하합니다 ! 이것으로 모든 세션이 끝났습니다 !

