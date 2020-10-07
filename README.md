# Virtual_Environment_Process_Analysis & Realtime Monitoring application
제품 공정에 대한 가상 데이터 분석 (2020.08.08 ~ )

## 가상 환경 분석 
Flexsim 소프트웨어를 이용해 EGR Cooler 제품의 조립공정 시뮬레이션 모델을 만든 후 그 과정에서 생성되는 데이터들을 활용해 머신러닝 분류 알고리즘에 학습시켜 OEE를 항샹시키는 데에 활용할 수 있도록 한다.
  ### 개발 순서
  1. EGR Cooler를 제작하는 공정에 대하여 순서 및 공정 요소를 선정
  2. Flexsim 소프트웨어를 이용하여 EGR Cooler 조립 공정을 제작
  3. 일정 시간을 설정하여 해당 시간의 제품 데이터를 excel 파일로 저장
  4. 저장된 excel 파일을 이용하여 python 머신러닝 분류 알고리즘에서 데이터의 상관관계를 분석

## 실시간 모니터링 어플리케이션
조립공정에서 생성되는 데이터들을 데이터 베이스를 설계하여 적재한 후 웹 서버에서 실시간으로 모티너링 할 수 있는 웹 어플리케이션을 개발한다.
  ### 개발 순서
  1. python으로 Felxsim에서 시뮬레이션으로 생성했던 것과 동일한 데이터를 생성하는 프로그램 제작
  2. DataBase를 MySQL 환경에서 제작
  3. AWS 서버를 EC2 인스턴스로 제작
  4. python 프로그램으로 생성된 데이터를 Server로 Post 요청을 통해 Database에 적재하거나 GET 요청으로 조회 하는 작업 실행
  5. 데이터를 홈페이지에서 조회 할 수 있도록 함
  6. 홈페이지에서 데이터를 활용하여 실시간 OEE를 출력하도록 
