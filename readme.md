# Goorm Diary

### Index

1. **Function**
2. **사이트맵 구성도**
3. **DB 구성도**
4. **모듈 구성도**
5. **개발 요소**
6. **Deploy(배포)**

--------------

### 1. Function

- 주 기능

  - 담배 검색
    - 브랜드 별
    - 맨솔 유/무
    - TAR mg 별
    - 해외 / 국내
  - 담배 리뷰
    - 맛
    - 타격감
    - 총 점(별점)
    - 개별 코맨트
  - 담배별 상세설명
    - 종류(전자 or 연초)
    - 브랜드
    - 제품명
    - 제품사진(브랜드 사진 등)
    - 가격
    - 출시일
    - 니코틴 함량
    - 타르 함량
  - 개인별 구름일기
    - 내가 현재까지 핀 구름 데이터 저장
    - 일간/월간 별 흡연률 - 그래프형식?
    - 담배 구매시 구름 등록 
      -> 현재 DB에 저장된 담배라면, 데이터 꺼내와서 마이리스트에 추가. 추가한 날짜 등록됨.

- 서브/추가적 기능

  - 금연 클리닉 서비스
  - 기타 등등



### 2. 사이트맵 구조

**main**

- nav(menu, logo, mypage)
- 현재 사용중인 담배 or 담배 등록
  - 흡연 버튼
- 최신 담배 or 담배 리스트(추천 순) -> 3~4개
- 주간 흡연율

**mypage**

- 나의 사랑하는 구름리스트

- 흡연한 구름리스트

- 현재 나의 신체레벨
  구름 흡연율로 본인의 신체상황을 측정하여 표시
  ex) 폐암으로 사망 직전입니다.
  ex2) 아직 초기단계이므로 금연을 추천합니다

- 현재 흡연중인 구름(남은 개수 등)

- 탈퇴(금연) 버튼
  
  1. 정말.. 구름을 버리시겠습니까?
  
    No. 취소
    Yes. 다음 문항으로

  2. 다시 돌아올 소중한 유저분들을 위해, 
  휴먼계정으로 설정하여 유저 데이터는 보존함에 동의하십니까

    No. 휴먼계정
    Yes. ㄹㅇ탈퇴(유저정보 삭제)

**list**

- category (사이드바로 구현)

**detail**

- 구름 상세설명

**auth(login/signup).html**

- 로그인 / 회원가입 창

**myfavorite_list**
- 스크랩한 구름

**current**
- 현재 흡연 진행중인 구름
- 현재 사용자님께서 흡연중인 구름은 OO명 or OO%가 흡연중인 담배입니다.



### 3. DB 구성도



### 4. 모듈 구성도



### 5. 개발요소

- 구름 검색을 위해 한글명칭도 DB에 저장
- 브랜드 DB 1대다 관계 분할?
- 구름 별 이미지 업로드 -> DB 필드 추가



### 6. Deploy

- python anywhere
- heroku
- AWS