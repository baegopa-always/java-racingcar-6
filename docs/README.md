# 자동차 경주
## 기능 목록
- [ ] 사용자는 각 자동차에 이름을 부여할 수 있다. - CarGenerator#createCarList
  - [ ] 사용자로부터 이름을 입력받을 수 있다. - UserInput#setCarName
  - [ ] 자동차 이름은 쉼표(,)를 기준으로 구분한다. - NameValidator#splitComma
  - [ ] 이름이 1자 이상 5자 이하인지 확인한다. - NameValidator#checkNumberOfString
  - [ ] 이름이 대, 소문자 알파벳인지를 확인한다. - NameValidator#checkAlphabets
  - [ ] 이름이 중복되었는지 확인한다. - NameValidator#checkRedundancy
- [ ] 사용자는 몇 번의 이동을 할 것인지를 입력할 수 있다. - UserInput#setRoundOfGame
  - [ ] 입력한 값이 1 이상 10 이하의 자연수인지 확인한다. - RoundValidator#checkNaturalNumber
- [ ] 0 에서 9 사이에서 무작위 값을 구한다. RandomNumberGenerator#createRandomNumber
  - [ ] 무작위 값이 4 이상일 경우 전진한다. - Car#accelerate
  - [ ] 무작위 값이 4 이상인지 확인한다. - Car#canAccelerate
- [ ] 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다. - RacingCar#printRaceResult
  - [ ] 전진하는 자동차의 이름을 알 수 있다. - Car#getName
  - [ ] 전진하는 자동차의 상태를 알 수 있다. - Car#getState
- [ ] 자동차 경주 게임을 완료한 후 최종 우승자를 출력한다. - RacingCar#printWinner
  - [ ] 우승자는 한 명 이상일 수 있다. - Result#listWinner
  - [ ] 우승자가 여러 명일 경우 쉼표(,)를 이용하여 구분한다.- Result#splitComma

## 예외 사항
- [ ] 사용자가 잘못된 값을 입력할 경우 IllegalArgumentException을 발생시킨 후 애플리케이션은 종료되어야 한다.


## 기능 요구 사항
초간단 자동차 경주 게임을 구현한다.

- 주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.
- 각 자동차에 이름을 부여할 수 있다. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.
- 자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.
- 사용자는 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.
- 전진하는 조건은 0에서 9 사이에서 무작위 값을 구한 후 무작위 값이 4 이상일 경우이다.
- 자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다. 우승자는 한 명 이상일 수 있다.
- 우승자가 여러 명일 경우 쉼표(,)를 이용하여 구분한다.
- 사용자가 잘못된 값을 입력할 경우 IllegalArgumentException을 발생시킨 후 애플리케이션은 종료되어야 한다.