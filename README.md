# **프로젝트 : JoeunMovie** 🎬

<p align="center">
  <!-- 대표 이미지가 있으면 경로만 바꿔서 사용하세요 -->
  <img src="./movie/src/main/webapp/static/img/movie/대표이미지.png" width="600" alt="JoeunMovie 대표 이미지">
</p>

> 영화 정보를 탐색하고, 리뷰를 남기며, 관리자 페이지에서 영화/회원/리뷰를 관리할 수 있는 **웹 기반 영화 플랫폼**

<br>

## 📌 시연 영상
<!-- 배포 링크 또는 유튜브 링크로 교체하세요 -->
[![시연 영상](./movie/src/main/webapp/static/img/thumbnail.png)](https://www.youtube.com/watch?v=YOUR_VIDEO_ID)

> ⬆️ 이미지를 클릭하면 시연 영상으로 이동합니다.

<br>

---

## 📋 목차
- [1. 프로젝트 개요](#1-프로젝트-개요)
- [2. 프로젝트 구조](#2-프로젝트-구조)
- [3. 주요 기능](#3-주요-기능)
- [4. 기술 스택](#4-기술-스택)
- [5. Architecture](#5-architecture)
- [6. 화면 UI](#6-화면-ui)
- [7. 자체 평가 의견](#7-자체-평가-의견)

---

<br>

## 1. 프로젝트 개요

### 1-1. 프로젝트 주제
- 영화 정보 탐색 및 리뷰 플랫폼 **"JoeunMovie"**

### 1-2. 기획 의도
- 사용자가 영화 정보를 쉽게 조회하고, 리뷰를 남기며
- 관리자는 영화/회원/리뷰를 관리할 수 있는 웹 서비스를 구현

### 1-3. 기대효과
- 영화 탐색/리뷰 작성 경험을 한 곳에서 제공
- 관리자 기능을 통해 콘텐츠(영화) 및 사용자 운영 효율화

<br>

---

## 2. 프로젝트 구조

### 2-1. 디렉토리 구조 (요약)
```
Joeun-Movie/
├── README.md
└── movie/                               ← WebApp
    ├── src/main/java/movie/
    │   ├── Servlet/                     ← 서블릿 컨트롤러 (관리자/마이페이지/상세 등)
    │   ├── Service/                     ← 비즈니스 로직
    │   ├── DAO/                         ← DB 접근 계층
    │   ├── DTO/                         ← DTO/Entity
    │   └── filter/                      ← 인코딩 필터 등
    ├── src/main/webapp/
    │   ├── page/                        ← JSP 페이지 (관리자/마이페이지 등)
    │   └── static/                      ← CSS/JS/이미지
    └── sql/                             ← SQL 스크립트(있다면)
```

<br>

---

## 3. 주요 기능

| 구분 | 기능 |
|:---:|:---|
| 🎬 영화 | 영화 상세 조회 (`/detail`) / 키워드 기반 검색 파라미터 지원 |
| ⭐ 리뷰 | (관리자) 전체 리뷰 목록 조회 (`/admin/review/list`) / (마이페이지) 내 리뷰 목록 조회 (`/mypage/reviewlist`) |
| 👤 회원 | 회원가입 / 로그인 / 로그아웃 / 아이디 중복 체크 (`/id-check`) |
| 🔐 로그인 유지 | 토큰 기반 로그인 유지(검증/갱신/삭제) + 로그아웃 시 쿠키 토큰 제거 |
| 🧾 마이페이지 | 마이페이지 화면, 내 정보 화면 제공 (`/mypage/mypage`, `/mypage/info`, `/mypage/userinfo`) |
| 🛠 관리자 | (영화) 등록/목록/상세/삭제 + 포스터 이미지 업로드(Multipart) / (회원) 목록/상세 / (리뷰) 목록 |
| 🌐 공통 | UTF-8 인코딩 필터 적용(한글 깨짐 방지) |

> ✅ **관리자 영화 관리 기능 예시**
> - 영화 목록: `/admin/movie/list`
> - 영화 등록: `/admin/movie/create` (포스터 이미지 업로드 포함)
> - 영화 상세(관리자): `/admin/movie/info`
> - 영화 삭제: `/admin/movie/delete`

<br>

---

## 4. 기술 스택

### Frontend (View)
<div align="left">
  <img src="https://img.shields.io/badge/JSP-007396?style=for-the-badge">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
</div>

### Backend
<div align="left">
  <img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white">
  <img src="https://img.shields.io/badge/Jakarta_Servlet-000000?style=for-the-badge">
</div>

### Database
<div align="left">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white">
</div>

### Tools
<div align="left">
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white">
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white">
</div>

<br>

---

## 5. Architecture

- **Servlet + JSP 기반 MVC 구조**
  - Servlet: 요청 처리/라우팅 및 Service 호출
  - Service/DAO: 비즈니스 로직 및 DB 접근
  - JSP: 화면 렌더링
- **세션 기반 로그인 + 토큰 기반 로그인 유지(자동 로그인)** 혼합 구조
- **파일 업로드(Multipart)**를 통한 영화 포스터 등록 지원

<br>

---

## 6. 화면 UI
> 아래는 예시 템플릿입니다. 실제 이미지 경로로 교체해서 사용하세요.

### 메인 화면
<details>
  <summary>메인 화면 보기</summary>
  <img src="./movie/src/main/webapp/static/img/ui/main.png" width="720" alt="메인화면">
</details>
<br>

### 영화 상세
<details>
  <summary>영화 상세 화면 보기</summary>
  <img src="./movie/src/main/webapp/static/img/ui/detail.png" width="720" alt="영화상세">
</details>
<br>

### 마이페이지
<details>
  <summary>마이페이지 화면 보기</summary>
  <img src="./movie/src/main/webapp/static/img/ui/mypage.png" width="720" alt="마이페이지">
</details>
<br>

### 관리자 (영화/회원/리뷰)
<details>
  <summary>관리자 화면 보기</summary>
  <img src="./movie/src/main/webapp/static/img/ui/admin.png" width="720" alt="관리자">
</details>

<br>

---

## 7. 자체 평가 의견

### 7-1. 잘된 점
- 서블릿 기반 MVC 구조로 요청/응답 흐름을 명확히 분리
- 관리자 페이지(영화/회원/리뷰)를 통해 운영 기능까지 포함
- 포스터 이미지 업로드 등 실제 서비스형 기능(파일 처리) 구현
- UTF-8 인코딩 필터 적용으로 한글 깨짐 이슈 최소화

### 7-2. 한계점
- 테스트 코드가 부족하여 변경 시 회귀 검증이 어려움
- 인증 구조(세션 + 토큰 유지)가 확장/보안 측면에서 개선 여지 존재
- UI/UX 및 기능 설명(README) 보강 필요
