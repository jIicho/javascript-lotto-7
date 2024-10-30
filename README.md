# javascript-lotto-precourse

## 1. 로또 게임 순서 정리

1. 로또 구입 금액을 사용자에게 입력 받는다.

   - 구입 금액은 1000원 단위로 입력 받으며,
     1000원으로 나누어 떨어지지 않을 경우 예외 처리

2. 당첨 번호를 입력 받는다.

   - 번호는 쉼표(,)를 기준으로 구분한다.
   - 중복되지 않는 수를 입력 받아야한다.
   - 만약 중복될 경우 예외 처리
   - [예외 처리] 1 - 45 사이의 수가 아닐 경우
   - [예외 처리] 중복된 수를 입력했을 경우
   - [예외 처리] 입력받은 번호가 6개가 아닐 경우(공백 작성시)
   - [예외 처리] 입력받은 값이 숫자가 아닐 경우
   - [예외 처리] 입력받은 값이 정수가 아닐 경우

3. 보너스 번호를 입력 받는다.

   - 이전에 입력 받은 당첨 번호와 중복되지 않는 수로 입력받아야 한다.
   - [예외 처리] 당첨 번호와 중복될 경우
   - [예외 처리] 입력 받은 값이 숫자가 아닐 경우
   - [예외 처리] 입력받은 값이 정수가 아닐 경우

4. 로또 구입 금액만큼 발행한 로또 수량과 번호를 출력한다.

   - 로또 번호는 오름차순으로 정렬하여 보여준다.

5. 당첨 내역을 출력한다.

6. 총 수익률을 출력한다.

   - 수익률은 소수점 둘쨰 자리에서 반올림한다.

> 사용자가 잘못된 값을 입력할 경우 에러 메시지와 함께 Error를 발생시키고, 해당 메시지를 출력한 다음 해당 지점부터 다시 입력 받는다.

---

## 2. 기능 구현 목록

1. 구입 금액 입력 및 처리

   - [x] 사용자에게 로또 구입 금액을 입력받는다. (구입 금액은 1,000원 단위로 입력 받는다.)
   - [x] [예외 처리] 구입 금액이 1,000원으로 나누어 떨어지지 않는 경우.
         에러 메시지를 발생시키고, 다시 입력받는 함수를 실행한다.
   - [x] [예외 처리] 구입 금액을 공백으로 작성할 경우.
   - [x] [예외 처리] 구입 금액을 음수로 작성할 경우.

2. 당첨 번호와 보너스 번호 입력 및 처리

   - [ ] 사용자에게 당첨 번호를 입력 받는다. 쉼표(,)를 기준으로 구분한다.
   - [ ] [예외 처리] 당첨 번호가 1 - 45까지 수가 아닐 경우.
   - [ ] [예외 처리] 당첨 번호를 공백으로 처리할 경우. (입력받은 당첨 번호가 6개가 아닐 경우)
   - [ ] [예외 처리] 당첨 번호가 6개 이상일 경우.
   - [ ] [예외 처리] 당첨 번호가 숫자가 아닐 경우.
   - [ ] [예외 처리] 당첨 번호가 음수일 경우.
   - [ ] [예외 처리] 당첨 번호가 정수가 아닐 경우. 예) 2.3

   - [ ] 사용자에게 보너스 번호를 입력 받는다. (당첨 번호와 중복되지 않아야한다.)
   - [ ] [예외 처리] 이전의 당첨 번호와 중복되는 수일 경우
   - [ ] [예외 처리] 보너스 번호가 1 - 45까지 수가 아닐 경우.
   - [ ] [예외 처리] 보너스 번호를 공백으로 처리할 경우.
   - [ ] [예외 처리] 보너스 번호가 숫자가 아닐 경우.
   - [ ] [예외 처리] 보너스 번호가 음수일 경우.
   - [ ] [예외 처리] 보너스 번호가 정수가 아닐 경우. 예) 2.3

3. 실행 결과 출력

   - [ ] 구입 금액만큼 발행한 로또 수량 및 번호를 출력한다.
   - [ ] 로또 번호는 오름차순으로 정렬하여 출력한다.
   - [ ] 당첨 내역을 출력한다.
         당첨 번호 3개 일치시 5,000원
         당첨 번호 4개 일치시 50,000원
         당첨 번호 5개 일치시 1,500,000원
         당첨 번호 5개 일치, 보너스 번호 일치시 30,000,000원
         당첨 번호 6개 일치시 2,000,000,000원
   - [ ] 수익률을 출력한다. (소수점 둘째자리에서 반올림한다.)

---

## 3. 프로그래밍 요구 사항

- indent depth를 3이 넘지 않도록 구현하기.
- 3항 연산자 쓰지 않기.
- 함수 (또는 메서드)가 한가지 일만 하도록 최대한 작게 만들기.
  (길이가 15라인을 넘어가지 않도록 구현한다.)
- else를 지양한다.
- 구현한 기능에 대한 단위 테스트 작성하기.
