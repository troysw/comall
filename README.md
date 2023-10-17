# Final Third
축구 정보 사이트 백엔드 포트폴리오

## 사용 언어 및 프레임워크

Java 17 , Springboot 3.1.1

## 주요 라이브러리

JPA, Lombok, jwt

### 왜 17, 3?

- 현재 재직중인 회사에서 내부 고도화(AWS RDS사용계획)를 위해 사용 하기 때문에 적응을 위해.<br/>
- 1번 이유와 이어서 aws를 고려해 jdk도 다소 패키지적 제한이 있는 corretto17 을 사용.<br/>
- java8, 11과 어떤차이가 있나 찾아보고 경험 해보기 위해.


### 패키지 구조

도메인 
 - controller
 - facade
 - service
 - domain
 - repository

기존 레이어드 구조에 파사드 패턴을 추가.

상세 설명 링크
https://velog.io/@ksw_dev/%ED%8F%AC%ED%8A%B8%ED%8F%B4%EB%A6%AC%EC%98%A4-%EB%A0%88%EC%9D%B4%EC%96%B4%EB%93%9C-%EC%95%84%ED%82%A4%ED%85%8D%EC%B3%90


### 추후 구현 목록
- dev, prod profile 생성후 aws free tier로 연동 
- ~~jwt 인증 로그인 및 기본 보안 설정~~
- ~~회원, 권한 엔티티 구현 및 기본 로그인, 회원가입 구현~~
- ~~게시판 엔티티 구현 및 연관관계 설정~~
- epl 라이브 스코어 footmob open api 연동
