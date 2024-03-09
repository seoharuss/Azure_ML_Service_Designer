# Session 3. Use Designer to build pipeline

아무런 의미 없이 파이프라인을 구축하고 실행하면 흥미가 떨어지기에 다음과 같은 하나의 상황을 가정해보려 합니다 😄

만약, 해당 세션의 첫 화면이 어색하시다면 [이전 세션](./Session2.md)을 다시 확인 해보시는걸 추천드립니다 !

## 근속 연수에 따라 연봉을 예측해주는 모델 생성

- 가상 머신이 생성된 이후, 왼쪽 탭에서 `디자이너` 탭을 클릭한 후, `미리 빌드된 클래식 구성 요소를 사용하여 새 파이프라인 만들기`를 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/623adc31-1415-4899-9ad7-52dc8bc7293e)

- 다음과 같은 창이 뜨는데, `구성 요소` 탭에서 여러가지 구성요소들을 볼 수 있습니다.
  > Tip 😄 : 해당 여러가지 컴포넌트들을 끌어다가 자유롭게 배치하여 사용할 수 있습니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/e424c90b-0922-482f-8aa8-765b3cd71590)

- `구성 요소`에서 `Data Input and Output` 세션에서 `Enter Data Manually` 컴포넌트를 오른쪽에 끌어놓습니다.
- 그리고 해당 컴포넌트를 더블 클릭하고, `Data`를 해당 그림처럼 입력해줍니다.
- 입력을 완료했다면, 우측 상단의 `파이프라인 인터페이스`를 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/c91bca14-3b6e-401f-97de-b56ec3bf5bda)

- 입력의 우측 `+` 버튼을 누르고 `컴퓨팅 대상`을 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/8664ae43-da2d-465b-abfa-741b86d40146)

- 입력 이름으로 `Compute instance`를 입력하고, 컴퓨팅 유형을 `컴퓨팅 인스턴스`로 선택합니다.
- 그리고 `Select Azure ML 컴퓨팅 인스턴스`에서 아까 만들어두었던 가상 머신을 선택합니다.
- 그리고 나서 바로 위의 `구성 및 전송` 버튼을 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/556ccf6e-4207-424a-be30-c4224761004b)

- 그러면 다음과 같은 파이프라인 작업 설정 창이 생성됩니다.
- `새로 만들기`를 클릭한 후, 새 실험 이름에 원하는 이름을 작성하고 아래로 스크롤하여 `다음` 버튼을 누릅니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/0acae3d4-1580-48e9-829d-9650de3296f6)

- 입력 및 출력에는 아까 설정했던 가상 머신이 있는 것을 확인할 수 있습니다.
- 선택한 후, `다음` 버튼을 누릅니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/3be2db27-3a03-4989-b8e7-95148aa0c3cb)

- 마지막으로 컴퓨팅 유형 선택에서 `컴퓨팅 인스턴스`를 선택하고, `Select Azure ML 컴퓨팅 인스턴스`에서 내가 만들었던 가상 머신을 클릭합니다.
- 그리고 `검토+제출` 버튼을 누릅니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/b32db277-a2f8-4d81-8561-3919ab2cf9d3)

- 그러면 다음과 같은 알림창이 상단쪽에 나타나면서 파이프라인이 로딩되는 것을 확인할 수 있습니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/0ed9a68a-54f0-4916-9a05-9410dc28a2c5)

- 파이프라인이 성공적으로 제출되었다면 `세부 정보 보기`를 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/fa90cad2-a759-4382-a4ac-bc719825a84b)

- 그러면 다음과 같은 창이 나타납니다.
  > Tip 😄 : 해당 창에서 자신이 구축했던 파이프라인의 동작과 데이터 결과를 상세하게 확인할 수 있습니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/3ea17de6-ba53-433b-b6e7-afa01bf548cf)

- 다음 그림 같이 왼쪽 사선이 계속 돌아가면 아직 가삳머신이 파이프라인을 구축하고 있다고 생각하면 됩니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/70b423dc-ee0a-4ac6-afdf-41069d2886ea)

- 작업이 완료되면 다음과 같이 초록색으로 나타납니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/99340278-4e7c-4440-a864-f686e582e0db)

- 그림과 같이 `o` 아이콘을 마우스 오른쪽 버튼으로 클릭한 후, 데이터 미리보기를 클릭하면, 데이터에 대한 분석 정보를 확인할 수 있습니다.
- 평균값, 중앙값 등 통계에 대한 정보도 볼 수 있고, 데이터 시각화도 확인할 수 있습니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/3197c4de-f0d3-4b28-b7f1-0b930caefde1)

- 다시 이전 창으로 돌아와서, 구성 요소 탭에서 `Machine Learning Algorithms`세션에서 `Linear Regression` 컴포넌트를 끌어옵니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/71283f2e-d062-47f9-bb4e-79b512889977)

- 그리고 구성요소 창에 `split`를 검색하여 `Split Data` 컴포넌트를 끌어옵니다.
- 그리고 `Enter Data Manually` 컴포넌트의 `Dataset`을 `Split Data` 컴포넌트의 상단에 연결해줍니다.
- **`Split Data` 컴포넌트의 왼쪽 output은 학습용 데이터로 사용하고, 오른쪽 output은 테스트용 데이터로 사용한다고 생각하면 됩니다.**

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/65d1ae3b-c565-49d8-8284-8b5e8a55ff66)

- `Split Data` 컴포넌트를 더블 클릭한 후, 다음과 같이 `Fraction of rows in the first output dataset`을 0.7로 설정해줍니다.
  > 컴포넌트의 왼쪽으로 0.7이 빠지고, 오른쪽으로 0.3이 빠진다는 뜻입니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/d5dbdd0c-843d-4911-aaef-ed0d612dfc3f)

- 그리고 다시 컴포넌트 검색창에 `train`을 검색한 후, 아래로 스크롤하여 `Train Model` 컴포넌트를 끌어옵니다.
- 그리고 다음 그림처럼 `Split Data` 컴포넌트와 `Linear Regression` 컴포넌트를 `Train Model` 컴포넌트에 연결해줍니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/dfdd6fca-2fbb-4fc8-9e5e-0dee1afe91cc)

- `Train Model`에 경고 표시가 되어 있는데 이는 `Label column`이 설정되지 않았기 때문입니다.
- 이것을 해결하기 위해 `Train Model` 컴포넌트를 더블 클릭한 후, 오른쪽 상단의 열 편집 버튼을 누릅니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/723518d2-bba4-4885-9918-bfd915b8f355)

- 열 이름에 "연봉"을 입력하고 저장을 누릅니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/bb6e3a0d-9a43-4376-817d-1ac5b1a832cf)

- 다시 돌아와서, 컴포넌트 검색창에 `score`을 검색한 후, `Score Model` 컴포넌트를 끌어옵니다.
- 그리고 그림처럼 `Split Data` 컴포넌트와 `Train Model` 컴포넌트를 `Score Model` 컴포넌트에 연결해줍니다.
  > `Split Data` 모델의 오른쪽 데이터셋(테스트 데이터셋)을 `Score Model` 컴포넌트의 입력으로 주어, `Split Data` 모델의 왼쪽 데이터셋(훈련용 데이터셋)을 `Linear Regression`으로 훈련한 모델을 검증해보는 작업이라고 생각하시면 됩니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/eec82e3e-a71f-4fe0-b716-cc6511286bd4)

- 마지막으로, 컴포넌트 검색창에 `evaluate`를 검색한 후, `Evaluate Model` 컴포넌트를 끌어옵니다.
- 그리고 다음 그림처럼 `Score Model` 컴포넌트의 `Scored Dataset`을 `Evaluate Model` 컴포넌트에 연결해줍니다.
- 그리고 우측 상단의 `구성 및 전송` 버튼을 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/819b1b84-8e38-4a5c-8e64-aa34966deb8b)

- 다음과 같은 창에서도 `제출` 버튼을 누릅니다.
  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/01c363c9-56c1-4f54-a435-ae01d65c79fc)

- 만약 에러 메시지가 출력되면 무시하고 계속 `제출` 버튼을 클릭하면 됩니다.
- 그리고 아까와 같이 파이프라인이 구축되고, 완료되면 `세부 정보 보기`를 클릭합니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/957f7c3b-85eb-4a48-9486-8c74928f1822)
  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/674af210-938b-44d3-93c6-79ff652a55c8)

- 그러면 다음 그림과 같은 창이 생성됩니다.

  ![image](https://github.com/seoharuss/Azure_ML_Service_Designer/assets/127467806/2c49ed50-b7b8-49a7-b156-815540a621a7)

## Session 3. Summary
이번 세션에서
