# 자동차 경주 게임

## 사용자 입력

- [x] 사용자는 경주할 자동차들의 이름을 쉼표로 구분하여 입력한다
- [x] 사용자는 시도할 횟수로 숫자 값을 입력한다

## 게임 진행 로직

- [x] 사용자가 입력한 자동차 이름들과 그 개수에 따라 자동차 인스턴스 생성
- [x] 사용자가 입력한 횟수만큼 각 자동차는 0에서 9 사이의 임의의 값을 산출하여 전진 여부 결정
  - [x] 0에서 9 사이에서 4 이상의 무작위 값이 나온 경우 해당 회차 때 해당 자동차는 전진
- [x] 전진하는 자동차를 출력할 때 자동차 이름도 함께 출력
- [x] 모든 회차가 종료된 이후 가장 멀리 간 자동차(들)을 출력
  - [x] 우승자가 여러 명일 경우 쉼표(,)를 이용하여 구분

## 유효성 및 예외 처리
- 사용자가 잘못된 값을 입력할 경우, [ERROR]로 시작하는 에러 메시지 출력 후 해당 부분의 입력을 다시 받는다
  - [x] 자동차 이름을 입력하지 않은 경우 예외 처리
  - [x] 자동차 이름이 6글자 이상인 경우 예외 처리 
  - [x] 자동차 이름에 띄어쓰기가 있는 경우 예외 처리
  - [x] 자동차명이 중복되는 경우 예외 처리
  - [x] 시도 회수가 숫자가 아닌 경우 예외 처리
  - [x] 시도 회수가 1보다 작은 경우 예외 처리
  