# SQL

- 데이터를 관리하기 위해 설계된 특수 목적의 프로그래밍 언어이다.
- 표준, 데이터베이스안의 테이블 생성, 삭제, 조회, 수정
- 오라클,mySQL,....에서도 사용 가능
- 형식 : 명령어;

# sqlite 조작어

- sqlite 프로그램 조작 명령어
- 조작 명령어 스타일 : .명령어 (.help는 조작 명령어 도움)
- 데이타베이스 열거나 새로 생성 : .open 데이타베이스이름.db
- 데이타베이스 안에 모든 테이블 조회 : .table

# 테이블 조회

- 테이블안에 있는 모든 레코드 조회
- select * from 테이블이름;
- 테이블 조회시 깔끔하게 표시 : .header on -> .mode column -> select * from 테이블이름;
- 레코드 수를 5개로 제한하여 조회 : select * from 테이블이름 limit 5;
- 테이블에서 특정 컬럼만 추출해서 조회하고 싶다 : select 컬럼명1,칼럼명2,.. from 테이블이름;
- 조건에 맞는 레코드만 추출하기 : select * from 테이블이름 where 조건; (조건 = and , or , not , 비교연산자)
- 조건에 맞는 레코드만 추출하고 동시에 특정 칼럼 추출 : select * from 테이블이름 where 조건1,조건2,..;

# SQL 명령어

- 테이블 생성하기 : create table 테이블이름(컬럼명1 데이터형식,컬럼명2 데이터형식,...);
- .table - 데이터베이스 테이블 목록 보기
- .schema 테이블이름 - 테이블 구조 표시
- 테이블 조회시 깔끔하게 표시 : .header on -> .mode column -> select * from 테이블이름;
- 데이터 삽입하기 : insert into 테이블이름 values('값1','값2',...);
- 데이터 삭제하기 : delete from 테이블이름 where 열이름='값';
- 데이터 수정하기 : update 테이블이름 set 열이름='수정값' where 열이름='값';