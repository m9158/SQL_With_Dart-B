# SQL_ADVANCED 6주차 정규 과제 

📌SQL_ADVANCED 정규과제는 매주 정해진 분량의 『*혼자 공부하는 SQL*』 을 읽고 학습하는 것입니다. 이번주는 아래의 **SQL_ADVANCED_6th_TIL**에 나열된 분량을 읽고 공부하시면 됩니다.

아래의 문제를 풀어보며 학습 내용을 점검하세요. 문제를 해결하는 과정에서 개념을 스스로 정리하고, 필요한 경우 제시된 강의를 참고하여 보완하는 것이 좋습니다.

<!-- 강의 링크는 아래와 같습니다.
https://www.youtube.com/watch?v=cw1wGN0ZdFA&list=PLVsNizTWUw7GCfy5RH27cQL5MeKYnl8Pm&index=19
https://www.youtube.com/watch?v=bMQ_dAoaMzA&list=PLVsNizTWUw7GCfy5RH27cQL5MeKYnl8Pm&index=20
https://www.youtube.com/watch?v=bggWVsBmKag&list=PLVsNizTWUw7GCfy5RH27cQL5MeKYnl8Pm&index=21
-->

**교재 실습 예제 파일은 07_SQL_ADVANCED_Template 레포지토리의 src 폴더에 업로드되어 있습니다. market_db 파일도 해당 폴더에 함께 포함되어 있으니 참고하시기 바랍니다.**

**👀(수행 인증샷은 필수입니다.)** 

## SQL_ADVANCED_6th_TIL

### 7장 스토어드 프로시저
#### 01. 스토어드 프로시저 사용 방법
#### 02. 스토어드 함수와 커서
#### 03. 자동 실행되는 트리거 


## Study Schedule

| 주차  | 공부 범위     | 완료 여부 |
| ----- | ------------- | --------- |
| 1주차 | p.24~99    | ✅         |
| 2주차 | p.102~155   | ✅         |
| 3주차 | p.158~213  | ✅         |
| 4주차 | p.216~271 | ✅         |
| 5주차 | p.274~327 | ✅         |
| 6주차 | p.330~369 | ✅         |
| 7주차 | p.372~407 | 🍽️         |


<br>

<!-- 여기까진 그대로 둬 주세요-->

---

# 1️⃣ 학습 내용 정리

## 1. 스토어드 프로시저 사용 방법 

1. 스토어드 프로시저 기본
   - 스토어드 프로시저: MySQL에서 제공하는 프로그래밍 기능.
   - 쿼리 문의 집합으로도 볼 수 있으며, 어떠한 동작을 일괄 처리하기 위한 용도로 사용
   - 자주 사용하는 일반적인 쿼리를 반복하는 것보다는 스ㅗ어디 프로시저로 묶어 놓고, 필요할 때마다 간단히 호출만 하면 훨씬 편리하게 MySQL을 운영할 수 있다.

2. 스토어드 프로시저의 생성 및 삭제
   - 삭제를 할 때는 user_proc뒤에 () 괄호를 작성하지 않는다.

3. 스토어드 프로시저 실습
   - 스토어드 프로시저에서 실행시 입력 매개변수를 지정할 수 있다.
   - IN 입력_매개변수_이름 데이터_형식
   - 스토어드 프로시저에서 처리된 결과를 출력 매개변수를 통해 얻을 수 있다.
   - OUT 출력_매개변수_이름 데이터_형식

<!-- 이번 챕터에서는 확인문제를 실습 인증으로 대체하여 진행합니다. 제시된 실습을 흐름에 맞게 진행한 후, 실습 과정이 보일 수 있도록 인증 사진을 2장 이상 제출해 주세요. -->

<img width="1455" height="679" alt="image" src="https://github.com/user-attachments/assets/68e5dbc8-df90-4a0e-8900-71d1c49ab362" />

<img width="1132" height="386" alt="image" src="https://github.com/user-attachments/assets/0957d1de-396b-4f2c-9402-c036efb48f11" />

<img width="1255" height="354" alt="image" src="https://github.com/user-attachments/assets/c0a96cd3-2990-41b7-a099-d4fe98b75f0e" />

<img width="1482" height="624" alt="image" src="https://github.com/user-attachments/assets/0a808fd9-0f55-4140-8193-39e4a9f690ef" />


## 2. 스토어드 함수와 커서 

1. 스토어드 함수
   - MySQL이 사용자가 원하는 모든 함수를 제공하지 않으므로 필요하다면 사용자가 직접 만들어 사용하는 것
   - RETURNS 문으로 반활할 값의 데이터 형식을 지정하고, 본문 안에서는 RETURN 문으로 하나의 값을 반환해야한다
   - 스토어드 함수의 매개변수는 모두 입력변수이다. IN을 붙이지 않는다.

2. 커서로 한 행씩 처리하기
   - 커서는 테이블에서 한 행씩 처리하기 위한 방식이다.
   - 첫번 째 행을 처리한 후 마지막 행까지 한 행씩 접근해서 값을 처리한다.

<img width="576" height="308" alt="image" src="https://github.com/user-attachments/assets/ca9aea84-11cd-45bc-a42f-014b2093d7d8" />

<img width="392" height="410" alt="image" src="https://github.com/user-attachments/assets/0966da68-5b67-4447-a515-002df6d695dc" />



<!-- 이번 챕터에서는 확인문제를 실습 인증으로 대체하여 진행합니다. 제시된 실습을 흐름에 맞게 진행한 후, 실습 과정이 보일 수 있도록 인증 사진을 2장 이상 제출해 주세요. -->

<img width="971" height="475" alt="image" src="https://github.com/user-attachments/assets/a289f962-2c5c-4397-aa5d-2fb026c9c99c" />

<img width="1206" height="550" alt="image" src="https://github.com/user-attachments/assets/fad914bb-d0b5-476f-b9ca-e06ff24af947" />



## 3. 자동 실행되는 트리거 

1. 트리거의 개요
   - 테이블에 INSERT나 UPDATE 또는 DELETE 작업이 발생하면 실행되는 코드

2. 트리거의 기본 작동
   - 트리거는 테이블에서 DML 문의 이벤트가 발생할 때 작동한다.
   - 스토어드 프로시저와 문법이 비슷하지만, call 문으로 직접 실행 시킬 수는 없고 DML 등의 이벤트가 발생할 경우에만 자동으로 실행된다.
   - IN, OUT을 사용할 수 없다.

3. 트리거의 활용
   - 데이터 입력/수정/삭제가 발생할 때, 트리거를 자동으로 작동시켜 데이터를 변경한 사용자와 시간등을 기록할 수 있다.
     

<!-- 이번 챕터에서는 확인문제를 실습 인증으로 대체하여 진행합니다. 제시된 실습을 흐름에 맞게 진행한 후, 실습 과정이 보일 수 있도록 인증 사진을 2장 이상 제출해 주세요. -->

<img width="1204" height="560" alt="image" src="https://github.com/user-attachments/assets/3c02c63e-7d32-438d-be3b-c0c1447b673e" />

<img width="1176" height="425" alt="image" src="https://github.com/user-attachments/assets/4bd368ea-7743-4401-8335-3a5f39625eeb" />

<img width="1211" height="273" alt="image" src="https://github.com/user-attachments/assets/8c873719-8038-478e-a9b4-d3c06bc0ec2e" />


---

# 2️⃣ 실습과제

## 1. 데이터베이스 구축

아래 코드를 MySQL Workbench에 붙여넣은 후,  
**전체 드래그 → 실행 (Ctrl + Shift + Enter)** 하여 데이터베이스를 구축하세요.

```sql
CREATE DATABASE IF NOT EXISTS week6_db;
USE week6_db;

-- 초기화
DROP TABLE IF EXISTS transactions;
DROP TABLE IF EXISTS accounts;

-- 계좌 테이블
CREATE TABLE accounts (
    acc_id INT PRIMARY KEY,
    name VARCHAR(20) NOT NULL,
    balance INT NOT NULL DEFAULT 0 CHECK (balance >= 0)
);

-- 거래 테이블
CREATE TABLE transactions (
    tx_id INT PRIMARY KEY,
    acc_id INT NOT NULL,
    amount INT NOT NULL,
    tx_date DATETIME NOT NULL DEFAULT CURRENT_TIMESTAMP
);

-- 샘플 데이터
INSERT INTO accounts VALUES
(1, '진아', 20000),
(2, '혜인', 8000),
(3, '규서', 55000),
(4, '규영', 12000);
```

## 2. 실습 문제

다음 문제를 수행하고 실행 결과를 확인 후 인증 사진을 아래에 업로드하세요.
(추가 수행도 필수입니다.)


### 1. 스토어드 프로시저

**다음 요구사항을 만족하는 프로시저 `sp_add_balance`를 생성하시오.**
- 입력값: `p_acc_id INT`, `p_amount INT`
- 기능:
  - 해당 계좌의 `balance`에 `p_amount`를 더합니다.

**추가 수행**
- 프로시저를 1회 이상 CALL 하시오.
- 실행 후 `accounts` 테이블을 조회하여 잔액이 변경되었는지 확인하시오.

---

### 2. 스토어드 함수

**다음 요구사항을 만족하는 함수 `fn_is_vip`를 생성하시오.**
- 입력값: `p_balance INT`
- 반환값:
  - `p_balance >= 50000` 이면 `'VIP'`
  - 그렇지 않으면 `'일반'`

**추가 수행**
- `accounts` 테이블을 조회하면서 `fn_is_vip(balance)` 결과를 함께 출력하시오.

---

### 3. 커서(Cursor)

**accounts 테이블의 모든 계좌를 커서로 순회하면서 각 계좌의 `name`과 `balance`를 출력하는 프로시저를 작성하시오.**

**추가 수행**
- 프로시저를 CALL 하여 결과를 확인하시오.

---

### 4. 트리거(Trigger)

**transactions 테이블에 새로운 데이터가 INSERT 될 때 해당 `acc_id`의 `accounts.balance`가 자동으로 증가하도록 트리거를 생성하시오.**

**추가 수행**
- transactions에 직접 INSERT 하시오.
- accounts 잔액이 자동으로 증가하는지 확인하시오.


<!-- 이 부분을 지우고 인증사진을 제출해주세요.-->


### 🎉 수고하셨습니다.







