# 문제 주소
https://programmers.co.kr/learn/courses/30/lessons/59411

## 문제 접근 방법

### 테이블 정보
- ANIMAL_OUTS 테이블은 입양보낸 동물의 정보를 담은 테이블
- ANIMAL_INS 테이블은 동물 보호소에 들어온 동물의 정보를 담은 테이블

### 문제 정리
- 입양을 간 동물 중, 보호 기간이 가장 길었던 동물 두 마리의 아이디와 이름을 조회하는 SQL문을 작성해주세요. 이때 결과는 보호 기간이 긴 순으로 조회해야 합니다.

### 해결방법
1. 입양을 간 보호 동물을 구하는 쿼리를 먼저 작성합니다. 입양간 동물은 ANIMAL_OUTS 테이블과 ANIMAL_INS를 INNER JOIN 하면 구할 수 있습니다. 
2. 보호 기간이 가장 길었던 이므로. 입양시기 - 보호시기 를 계산 후 정렬해야합니다.
3. 2마리를 조회해야합니다.