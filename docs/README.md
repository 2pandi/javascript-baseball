# 숫자 야구 게임

1부터 9까지 서로 다른 수로 이루어진 3자리 숫자가 주어지고 player가 예상한 숫자를 제시하여 주어진 숫자를 맞추면 이기는 게임이다.

## 구현 기능 목록

### A. 게임 기능 구현

1. 게임을 시작하면 게임 시작 문구를 출력한다. `숫자 야구 게임을 시작합니다.`
2. 임의의 3자리 숫자를 생성한다.(사용되는 수: 1 ~ 9)
   a. 각 자리의 숫자는 중복되지 않는다.
3. 숫자 입력을 요청하는 문구를 출력한다. `숫자를 입력해주세요`
4. player가 제시하는 3자리 숫자를 입력받는다.
   a. 입력된 값이 3자리의 숫자가 아닌 경우를 제한 한다.
   b. 동일한 숫자를 2개 이상 입력한 경우를 제한 한다.
   c. 제한되는 상황인 경우 `throw`문으로 종료시킨다.
5. 제시된 숫자에 대한 결과를 출력한다.
   a. 같은 수가 같은 자리에 있는 경우 `스트라이크`
   b. 다른 자리에 있는 경우 `볼`
   c. 같은 수가 전혀 없는 경우 `낫싱`
   d. a 경우와 b 경우가 동시에 발생하면 ` `(공백 문자)로 구분하여 볼, 스트라이크 순서로 출력한다.
6. player가 생성된 숫자를 맞추는 경우 게임을 종료한다.
   a. 게임 종료 메시지를 출력한다. `3개의 숫자를 모두 맞히셨습니다! 게임 종료`
   b. 종료 후 (1, 2)명령어를 통해 다시 시작하거나 완전히 종료할 수 있는 메시지를 출력한다. `게임을 새로 시작하려면 1, 종료하려면 2를 입력하세요.`
7. 게임 종료 후 명령어를 입력 받아 게임을 다시 시작하거나 완전히 종료한다.
   a. `1`을 입력받는 경우 게임을 다시 시작한다.
   b. `2`를 입력받는 경우 게임을 완전히 종료한다.

### B. 개발 기능 구현

1. `npm install` 명령어를 통해 패키지를 설치한다.
2. MissionUtils 라이브러리를 설치한다.
3. Jest를 이용하여 정리한 기능 목록이 정상 동작하는지 확인한다.