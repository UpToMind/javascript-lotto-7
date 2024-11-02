# javascript-lotto-precourse

## MVC 패턴으로 분리시작

- [x] constants 폴더

  - [x] Messages.js

    - [x] "구입 금액을 입력해주세요.\n"
    - [x] "개를 구매했습니다."
    - [x] "당첨 번호를 입력해 주세요.\n"
    - [x] "보너스 번호를 입력해 주세요.\n"
    - [x] "당첨 통계"
    - [x] "---"
    - [x] "3개 일치 (5,000원) - "
    - [x] "4개 일치 (50,000원) - "
    - [x] "5개 일치 (1,500,000원) - "
    - [x] "5개 일치, 보너스 볼 일치 (30,000,000원) - "
    - [x] "6개 일치 (2,000,000,000원) - "
    - [x] "총 수익률은 "
    - [x] "개"
    - [x] "%입니다."

  - [x] Errors.js

    1. 구입 금액에서 에러

    - [x] "[ERROR] 1000원단위로 구매해주세요." NOT_1000_WON
    - [x] "[ERROR] 1000원 이상의 돈을 내주세요." NOT_ENOUGH_MONEY
    - [x] "[ERROR] 숫자를 입력해주세요." NOT_MONEY_BUT_NUMBER

    2. 당첨 번호 에러

    - [x] "[ERROR] 로또 번호는 6개여야 합니다." NOT_6_NUMBERS
    - [x] "[ERROR] 1~45 사이 정수여야 합니다." NOT_1_TO_45
    - [x] "[ERROR] 로또 번호는 중복이 없어야 합니다." NO_REPEATED_NUMBER

    3. 보너스 번호 에러

    - [x] "[ERROR] 보너스 번호는 당첨번호와 달라야 합니다." NOT_BONUS_NUMBER
    - [x] "[ERROR] 1~45 사이 정수여야 합니다." NOT_1_TO_45

  - [x] Conditions.js
    - [x] 1000원
    - [x] 1,45,6
    - [x] 당첨금

- [x] views 폴더
  - [x] InputViews.js
    - [x] 구입 금액 입력
    - [x] 당첨 번호 입력
    - [x] 보너스 번호 입력
  - [x] OutputViews.js
    - [x] 구매한 로또 수량과 번호 출력
    - [x] 당첨 통계와 수익률 출력

구입금액을 입력해 주세요.
8000

8개를 구매했습니다.
[8, 21, 23, 41, 42, 43]
[3, 5, 11, 16, 32, 38]
[7, 11, 16, 35, 36, 44]
[1, 8, 11, 31, 41, 42]
[13, 14, 16, 38, 42, 45]
[7, 11, 30, 40, 42, 43]
[2, 13, 22, 32, 38, 45]
[1, 3, 5, 14, 22, 45]

당첨 번호를 입력해 주세요.
1,2,3,4,5,6

보너스 번호를 입력해 주세요.
7

당첨 통계

---

3개 일치 (5,000원) - 1개
4개 일치 (50,000원) - 0개
5개 일치 (1,500,000원) - 0개
5개 일치, 보너스 볼 일치 (30,000,000원) - 0개
6개 일치 (2,000,000,000원) - 0개
총 수익률은 62.5%입니다.
