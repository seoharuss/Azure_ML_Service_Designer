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
