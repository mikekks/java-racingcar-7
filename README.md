# java-racingcar-precourse

### Input
- [x] 사용자로부터 입력을 받는 클래스
  - [x] 자동차 이름을 입력을 받아 문자열 목록 반환하는 기능
  - [x] 시도 횟수를 입력으로 받아 숫자를 반환하는 기능
- [x] 올바르지 않은 입력을 검증한다.
  - [x] 자동차이름이 없거나 빈문자열일 경우
  - [x] 시도횟수가 숫자가 아닌 경우

### Output
- [x] 결과 또는 진행과정을 출력하는 클래스
  - [x] 실행 결과 출력 기능
  - [x] 최종 우승자 출력 기능

### RacingGame
- [x] 전체적인 게임 흐름을 통제하는 클래스
- [x] 자동차 동작 호출 기능 구현
- [x] 게임 시작하는 기능 구현

### Cars
- [x] Car 목록을 저장하는 일급컬렉션
- [x] 턴마다 모든 Car move 시도
- [x] 우승자 판단 및 목록 반환

### Car
- [x] 이름과 현재 위치 저장
- [x] 전진 시도 기능
  - [x] 전진 기능

### CarValidator
- [x] 자동차 이름 관련 잘못된 입력 검증
  - [x] 이름이 공백인 경우

### TurnValidator
- [ ] 시도 횟수가 음수인 경우

### Random
- [x] 0-9 사이의 무작위 값을 출력하는 기능
- [x] RealRandom : 실제 비즈니스 로직에 사용하는 Random 구현체
- [x] MockRandom : 테스트 코드 로직에 사용하는 Random 구현체

### Winners
- [x] 우승자 Car 목록을 저장하는 일급컬렉션
- [x] 우승자 목록을 반환하는 기능

### Turn
- [x] 현재 턴을 저장하고 있는 변수
- [ ] 사용자 입력값에 대한 검증을 진행한다.

--- 

### 기능 요구 사항
초간단 자동차 경주 게임을 구현한다.

* 주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.
* 각 자동차에 이름을 부여할 수 있다. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.
* 자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.
* 사용자는 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.
* 전진하는 조건은 0에서 9 사이에서 무작위 값을 구한 후 무작위 값이 4 이상일 경우이다.
* 자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다. 우승자는 한 명 이상일 수 있다.
* 우승자가 여러 명일 경우 쉼표(,)를 이용하여 구분한다.
* 사용자가 잘못된 값을 입력할 경우 IllegalArgumentException을 발생시킨 후 애플리케이션은 종료되어야 한다.