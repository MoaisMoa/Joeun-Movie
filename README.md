# **프로젝트 : JoeunMovie** 🎬

<p align="center">
  <a href="https://youtu.be/xkNmg4kmPro?si=PUyOHegEQZs6UnqS" target="_blank">
    <img width="2752" height="1536" alt="Gemini_Generated_Image_JoeunMovie" src="https://github.com/user-attachments/assets/c13d03ce-e2e2-4948-86ed-8f2ed9e64566" />
  </a>
</p>

<p align="center">⬆️ <b>위 이미지를 클릭하면 시연 영상(YouTube)으로 이동합니다.</b></p>

<br>

---

## 📋 목차
- [1. 프로젝트 개요](#1-프로젝트-개요)
- [2. 역할 및 담당 기능](#2-역할-및-담당-기능)
- [3. 프로젝트 아키텍처](#3-프로젝트-아키텍처)
- [4. 주요 기능](#4-주요-기능)
- [5. 기술 스택](#5-기술-스택)
- [6. 화면 UI](#6-화면-ui)
- [7. 자체 평가 의견](#7-자체-평가-의견)

---

<br>

## 1. 프로젝트 개요

### 1-1. 프로젝트 주제
- 영화 정보 탐색 및 리뷰 플랫폼 **"JoeunMovie"**

### 1-2. 기획 의도
- 다양한 OTT 서비스의 등장으로 콘텐츠 선택지는 늘어났지만 무엇을 볼지 결정하는 데 오히려 피로도가 증가하고 있다고 판단하였습니다.
- 콘텐츠를 시청한 사람들이 남긴 리뷰와 자신의 취향을 반영한 카테고리별 콘텐츠를 추천해주는 사이트 등이 주목받고 있다는 점을 고려하여 기획을 하게 되었습니다.
- 다른 사람들의 리뷰를 참고하고 자신의 취향에 맞는 영화를 빠르고 쉽게 선택할 수 있는 환경을 제공하는 것을 프로젝트의 목표로 설정했습니다.

<br>

## 2. 역할 및 담당 기능
**팀원 (4인 프로젝트)** **주요 역할: 사용자 인증 시스템 풀스택 구현 및 최종 프로젝트 발표 담당**

| 구분 | 담당 업무 내용 |
|:---:|:---|
| 👤 **사용자 인증** | 회원가입 및 로그인 페이지 UI 설계 및 프론트엔드 기능 구현 |
| 🔐 **인증 보안** | 서버 측 세션 기반 로그인 처리 및 아이디 중복 체크(`AJAX`) 기능 구현 |
| 🍪 **로그인 유지** | Cookie 및 Token을 활용한 자동 로그인(로그인 상태 유지) 로직 구현 |
| 🌐 **공통 처리** | 프로젝트 전체 한글 깨짐 방지를 위한 UTF-8 인코딩 Filter 적용 |
| 📢 **커뮤니케이션** | 프로젝트 진행 단계별 발표 자료 제작 및 최종 시연 발표 담당 |

<br>

## 3. 프로젝트 아키텍처
**Servlet + JSP 기반의 MVC 모델 2 아키텍처 적용**

<br>
<p align="center">
  <img width="100%" alt="JoeunMovie Architecture" src="https://github.com/user-attachments/assets/0e627bf7-5867-4b73-9052-39e336ea3352" />
</p>
<br>

---

## 4. 주요 기능

| 구분 | 기능 상세 |
|:---:|:---|
| 🎬 영화 | 영화 상세 조회 / 키워드 기반 검색 파라미터 지원 |
| ⭐ 리뷰 | (관리자) 전체 리뷰 목록 관리 / (마이페이지) 내 리뷰 작성 및 목록 조회 |
| 👤 회원 | 회원가입 / 로그인 / 로그아웃 / 아이디 중복 체크 (`/id-check`) |
| 🔐 로그인 유지 | 토큰 기반 로그인 유지(검증/갱신/삭제) + 로그아웃 시 쿠키 토큰 제거 |
| 🧾 마이페이지 | 개인 정보 조회 및 수정, 작성 리뷰 관리 화면 제공 |
| 🛠 관리자 | 영화 등록·수정·삭제(Multipart 포스터 업로드) / 회원 및 리뷰 통합 관리 |
| 🌐 공통 | UTF-8 인코딩 필터 적용으로 전 계층 데이터 일관성 유지 |

<br>

---

## 5. 기술 스택

### Frontend
<div align="left">
  <img src="https://img.shields.io/badge/JSP-007396?style=for-the-badge">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
  <img src="https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white">
</div>

### Backend
<div align="left">
  <img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white">
  <img src="https://img.shields.io/badge/Jakarta_Servlet-000000?style=for-the-badge">
  <img src="https://img.shields.io/badge/Apache_Tomcat-F8DC75?style=for-the-badge&logo=apache-tomcat&logoColor=black">
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

## 6. 화면 UI

### 로그인 및 회원가입
<p align="center">
  <img width="49%" alt="로그인" src="https://github.com/user-attachments/assets/73c6ff49-5f8a-4f18-9f13-b6669fe4556a" />
  <img width="49%" alt="회원가입" src="https://github.com/user-attachments/assets/6bfd57af-a10a-489e-b0db-40cdbf17c39c" />
</p>

### 유효성 검사 모달
<p align="center">
  <img width="80%" alt="회원가입-유효성" src="https://github.com/user-attachments/assets/1e48f1a5-52ed-4b86-a1cd-66f3c6b67589" />
</p>

<br>

---

## 7. 자체 평가 의견

### 7-1. 잘된 점
- 서블릿 기반 MVC 구조로 설계하여 비즈니스 로직과 프레젠테이션 로직을 명확히 분리함
- 포스터 이미지 업로드(Multipart) 및 리뷰 관리 등 실무적인 기능 포함
- AJAX를 활용한 아이디 중복 체크 등으로 사용자 편의성 증대

### 7-2. 한계점 및 개선 방향
- 보안성 강화를 위해 차후 세션 방식에서 JWT 기반 인증 방식으로 고도화 필요
- 단위 테스트 코드 도입을 통해 시스템의 안정성 확보 필요
