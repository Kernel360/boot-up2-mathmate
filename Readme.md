# MathMate - 수학을 친구처럼! 쉽고 재미있게 수학 개념을 익힐 수 있는 서비스

![logo](./logo.png)

# 🩵MathMate🩵 - 프로젝트 개요

> **MathMate : 당신의 수학 친구가 되어드릴게요.**

> **기획기간: 2024.07.15~2024.07.17**

<br>

> **따분하고 어려운 수학 개념서에 의해 "학습 부진" 상태가 된 중고등학생들의 수학 학력 수준을 높여주고, 저렴한 구독료로 Q&A 서비스를 이용하여 수학 공부에 어려움을 겪는 학생들에게 도움을 줄 수 있는 서비스**

## 🗓️ 기획안

### 요구사항 정의서
[요구사항 정의서 - 구글도큐먼트](https://docs.google.com/spreadsheets/d/1SwFm62ZFwaKZ_Ii6iGEoF-KPWIPlPxRlNmaQUcv1MYc/edit?usp=sharing)

<br>

### 기능명세서
 [기능 명세서 - 노션](https://sincere-nova-ec6.notion.site/cd31748f48af4b04b5fca1513349a272?pvs=4)

<br>

### 프로젝트 계획서
[프로젝트 계획서 - 노션](https://sincere-nova-ec6.notion.site/80697b45493446acb5723012b60797c7?pvs=4)

<br>

### 아키텍쳐 설계
![스크린샷 2024-07-18 오후 12 26 36](https://github.com/user-attachments/assets/1ee4ef9a-5973-492d-9ade-a506147b0f61)

#### 클라이언트
- 플러터
  -  크로스 플랫폼 개발 지원
  -  풍부한 디자인 도구 지원
  -  핫 로딩으로 개발 기간을 단축
#### 서버
- AWS EC2
  - 용량을 늘리거나 줄일 수 있다.
  - 사용한만큼 지불하므로 저렴하다.
  - 사용자가 인스턴스를 완전히 제어할 수 있다.
  - 보안 및 네트워크 구성, 스토리지 관리 효과적이다.
- 스프링 부트
  - 코드의 길이를 줄이는 어노테이션 제공으로 개발 시간 단축
  - 서버(아파치 톰캣)의 내장
  - 스프링 시큐리티, 필터 등 안정적이고 보안이 높은 애플리케이션 개발 가능
- 아파치 톰캣
  -  빠른 서버 배포 가능
  -  스프링 부트에 내장
- AWS RDS
  - 원하는 만큼 사이즈를 늘리거나 줄일 수 있는 탄력성
  - 다양한 DBMS 제공으로 높은 호환성
  - 쉬운 세팅 
- MySQL
  - 가장 대중적인 DBMS
  - 스프링 부트와 높은 호환성
  - 손쉬운 사용
- Redis
  - **높은 트래픽**에서 빠른 DB 통신 제공
  - 다양한 프로그래밍 언어로 개발 가능 
- R3
  - 높은 내구도를 자랑하며 정보를 안전하게 저장 가능
  - 저렴한 비용으로 사용 가능(ec2에 데이터를 저장하면 비용이 많이 나감)
  - 보안성이 뛰어남
  - 속도가 빠름
  - 나라별로 스토리지 버킷 지원이 가능
  - 버킷 버전 관리 가능
#### 외부 Open Api 
- 유니서트
  - 국내 대학교 인증을 위한 API 제공
- 소셜로그인
  - 카카오, 네이버, 구글 등 이미 가입된 사용자의 **가용성**을 높임 



<br>

> 데이터 모델링(ERD) :

![erd](./MathMate.png)

<br>

> 플로우 차트 :

[플로우차트](https://www.figma.com/board/oH6JiSzoebES8RKL24kDVc/Untitled?node-id=0-1&t=KoI5wbtQwKCZmHU1-1)

<br>

> **UI/UX 디자인(Figma)** : [https://www.figma.com/design/JMyzXiXA4zmF2i3AqxTrvO/MathMate?node-id=0-1&t=5i8bVUEYQqG4RP0X-1](https://www.figma.com/design/JMyzXiXA4zmF2i3AqxTrvO/MathMate?node-id=0-1&t=5i8bVUEYQqG4RP0X-1)

## 👥 일석삼조팀 소개

## 🌟 1~2일차

|                    김민주                    |                      양상원                      |               박수형               |
| :------------------------------------------: | :----------------------------------------------: | :--------------------------------: |
| [@Minju-Kimm](https://github.com/Minju-Kimm) | [@sangwonsheep](https://github.com/sangwonsheep) | [@Gyaak](https://github.com/Gyaak) |

## 🌟 3~4일차

|                    김민주                    |                이선우                |                이강민                |
| :------------------------------------------: | :----------------------------------: | :----------------------------------: |
| [@Minju-Kimm](https://github.com/Minju-Kimm) | [@I-migi](https://github.com/I-migi) | [@km2535](https://github.com/km2535) |

## 🌟 프로젝트 소개

## 🌟 시작 가이드

---

## Stacks 🐈

### Environment 🐈🐈

[![Visual Studio Code](https://camo.githubusercontent.com/e44113cc59b363e2f8bea43f073e0a61f2bcd1b2e79161c9cd03e6882cf5a4c2/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f56697375616c25323053747564696f253230436f64652d3030374143433f7374796c653d666f722d7468652d6261646765266c6f676f3d56697375616c25323053747564696f253230436f6465266c6f676f436f6c6f723d7768697465)](https://camo.githubusercontent.com/e44113cc59b363e2f8bea43f073e0a61f2bcd1b2e79161c9cd03e6882cf5a4c2/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f56697375616c25323053747564696f253230436f64652d3030374143433f7374796c653d666f722d7468652d6261646765266c6f676f3d56697375616c25323053747564696f253230436f6465266c6f676f436f6c6f723d7768697465) [![Git](https://camo.githubusercontent.com/8d433710b84192cd318b602aadcf296eed6c443fea42c2f06fba2ce65a49a412/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4769742d4630353033323f7374796c653d666f722d7468652d6261646765266c6f676f3d476974266c6f676f436f6c6f723d7768697465)](https://camo.githubusercontent.com/8d433710b84192cd318b602aadcf296eed6c443fea42c2f06fba2ce65a49a412/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4769742d4630353033323f7374796c653d666f722d7468652d6261646765266c6f676f3d476974266c6f676f436f6c6f723d7768697465) [![Github](https://camo.githubusercontent.com/dc4e9f7ea9597ea5a27629a36afb9ef8697569c621ccb42369070012b4092ae1/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4769744875622d3138313731373f7374796c653d666f722d7468652d6261646765266c6f676f3d476974487562266c6f676f436f6c6f723d7768697465)](https://camo.githubusercontent.com/dc4e9f7ea9597ea5a27629a36afb9ef8697569c621ccb42369070012b4092ae1/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4769744875622d3138313731373f7374796c653d666f722d7468652d6261646765266c6f676f3d476974487562266c6f676f436f6c6f723d7768697465)

### Development 🔨

<div style="display:flex; flex-direction=row;">

<img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=Java&logoColor=white">

<img src="https://img.shields.io/badge/Spring Boot-6DB33F?style=for-the-badge&logo=spring boot&logoColor=white">

<img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white">
<br>
<img src="https://img.shields.io/badge/Amazon AWS-232F3E?style=for-the-badge&logo=amazon aws&logoColor=white">

<img src="https://img.shields.io/badge/html5-E34F26?style=flat-square&logo=html5&logoColor=white">

<img src="https://img.shields.io/badge/css-1572B6?style=flat-square&logo=css3&logoColor=white">
<br>
<img src="https://img.shields.io/badge/javascript-F7DF1E?style=flat-square&logo=javascript&logoColor=black">

<img src="https://img.shields.io/badge/bootstrap-7952B3?style=flat-square&logo=bootstrap&logoColor=white">

</div>

### Communication 💬

[![Slack](https://camo.githubusercontent.com/8b20df4dce83849ed91f5dba04a42e793499dcd1064c094153dba4c1447390f3/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f536c61636b2d3441313534423f7374796c653d666f722d7468652d6261646765266c6f676f3d536c61636b266c6f676f436f6c6f723d7768697465)](https://camo.githubusercontent.com/8b20df4dce83849ed91f5dba04a42e793499dcd1064c094153dba4c1447390f3/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f536c61636b2d3441313534423f7374796c653d666f722d7468652d6261646765266c6f676f3d536c61636b266c6f676f436f6c6f723d7768697465) [![Notion](https://camo.githubusercontent.com/c8820d740db3809eac6809b9da45c5178fdc41e97a6a433046a4a5c05b91ef93/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4e6f74696f6e2d3030303030303f7374796c653d666f722d7468652d6261646765266c6f676f3d4e6f74696f6e266c6f676f436f6c6f723d7768697465)](https://camo.githubusercontent.com/c8820d740db3809eac6809b9da45c5178fdc41e97a6a433046a4a5c05b91ef93/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4e6f74696f6e2d3030303030303f7374796c653d666f722d7468652d6261646765266c6f676f3d4e6f74696f6e266c6f676f436f6c6f723d7768697465) [![GoogleMeet](https://camo.githubusercontent.com/6c2eea8252c0d09fbde43bff66e496f11edd2a8b7adbc4b3bc0d7567ca5d4c17/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f476f6f676c654d6565742d3030383937423f7374796c653d666f722d7468652d6261646765266c6f676f3d476f6f676c652532304d656574266c6f676f436f6c6f723d7768697465)](https://camo.githubusercontent.com/6c2eea8252c0d09fbde43bff66e496f11edd2a8b7adbc4b3bc0d7567ca5d4c17/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f476f6f676c654d6565742d3030383937423f7374796c653d666f722d7468652d6261646765266c6f676f3d476f6f676c652532304d656574266c6f676f436f6c6f723d7768697465)

---

## 화면 구성 📺

| 멘티 메인 페이지 | 리그 확인 페이지 |
| :--------------: | :--------------: |
|                  |                  |

| 커리큘럼 소개 페이지 | 개념 학습 페이지 |
| :------------------: | :--------------: |
|                      |                  |

| 멘토 메인 페이지 | Q&A 게시판 페이지 |
| :--------------: | :---------------: |
|                  |                   |

---

## 주요 기능 📦

### ⭐️왕기초 수학 개념 학습

### ⭐️SKY 누나, 오빠가 알려줄게! Q&A 게시판

### ⭐️티어가 무려 10개! 수학 공부를 더 재미있게 도와주는 리그 시스템

---

## 아키텍쳐

### 디렉토리 구조
