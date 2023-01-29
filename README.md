# coupon-service

## 요구사항

1. 쿠폰
    1. 저장방법
        1. 이미지 저장 후 경로를 DB에 저장
    2. 사용 여부 체크하기(언제 사용했는지, 누가 사용했는지)
    3. 그룹 공유하기(여러개 그룹에 공유 가능)
    4. 이미지 분석하기(추후 기능)
        1. 어느 회사에서 사용가능한지?
        2. 어떤 메뉴인지?
        3. 금액
        4. 바코드 생성해주기
        5. 이용가능일자
2. 그룹 공유 하기
    1. 그룹에 쿠폰 올라오면 알람 주기
        1. 이용가능일자가 끝나가면 알려주기
    2. 그룹에 들어가는 방법
        1. 누군가의 초대(id 혹은 전화번호)
        2. 그룹 들어가는 링크 전달하기
3. 유저는 여러개의 그룹에 들어가 있을 수 있음

## API

1. 쿠폰
    1. 등록하기
    2. 삭제하기
    3. 조회하기
    4. 그룹 등록하기
    5. 그룹 삭제하기
    6. 이용 등록하기 (이용 일자)
    7. 이용 취소하기
2. 그룹
    1. 생성하기
    2. 삭제하기
    3. 조회하기
    4. 수정하기(그룹명, 그룹 설명 등)
    5. 그룹에 유저 추가하기
        1. 초대링크로 초대하기
        2. id로 초대하기
        3. 전화번호로 초대하기
    6. 쿠폰 목록 조회하기
3. 유저
   1. 등록하기 
   2. 수정하기
   3. 조회하기
   4. 탈퇴하기
   5. 쿠폰 목록 조회하기
      1. 등록한 쿠폰 목록
      2. 이용가능한 쿠폰 목록
   6. 

## ERD

![ERD Image](http://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/ttokey/coupon-service/master/ERD_ver1.0.puml)