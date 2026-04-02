# **프로젝트 : JoeunMovie** 🎬

<p align="center">
  <a href="https://youtu.be/xkNmg4kmPro?si=PUyOHegEQZs6UnqS" target="_blank">
    <img width="2752" height="1536" alt="JoeunMovie_Main" src="https://github.com/user-attachments/assets/c13d03ce-e2e2-4948-86ed-8f2ed9e64566" />
  </a>
</p>

<p align="center">⬆️ <b>위 이미지를 클릭하면 시연 영상(YouTube)으로 이동합니다.</b></p>

<br>

---

## 📋 목차
- [1. 프로젝트 개요](#1-프로젝트-개요)
- [2. 프로젝트 아키텍처](#2-프로젝트-아키텍처)
- [3. 기술 스택](#3-기술-스택)
- [4. 주요 기능](#4-주요-기능)
- [5. 역할](#5-역할)
- [6. 화면 UI](#6-화면-ui)
- [7. 자체 평가 의견](#7-자체-평가-의견)

---

<br>

## 1. 프로젝트 개요

### 1-1. 프로젝트 주제
- 영화 정보 탐색 및 리뷰 플랫폼 **"JoeunMovie"**

### 1-2. 기획 의도
- 다양한 OTT 서비스의 등장으로 인한 콘텐츠 선택 피로도를 줄이기 위해 사용자 중심의 리뷰 및 추천 환경을 기획하였습니다.
- 타인의 리뷰를 참고하여 본인의 취향에 맞는 영화를 빠르고 정확하게 선택할 수 있는 환경 제공을 목표로 합니다.

<br>

## 2. 프로젝트 아키텍처

<br>
<p align="center">
  <img width="100%" alt="JoeunMovie Architecture" src="https://github.com/user-attachments/assets/0e627bf7-5867-4b73-9052-39e336ea3352" />
</p>
<br>

## 3. 기술 스택

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

### Database & Tools
<div align="left">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white">
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white">
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white">
</div>

<br>

## 4. 주요 기능

| 구분 | 기능 상세 |
|:---:|:---|
| 🎬 **영화 서비스** | 영화 상세 조회 및 키워드 기반 검색 |
| ⭐ **리뷰 시스템** | (관리자) 전체 리뷰 통합 관리 / (사용자) 마이페이지 내 리뷰 작성 및 관리 |
| 👤 **사용자 인증** | 회원가입, 로그인/로그아웃, 아이디 중복 체크 |
| 🔐 **보안/유지** | 토큰 기반 자동 로그인 시스템 및 로그아웃 시 쿠키 데이터 즉시 만료 |
| 🛠 **관리자 모드** | 영화 CRUD, 전체 회원 및 리뷰 데이터 관리 |
| 🌐 **인프라** | UTF-8 인코딩 필터 적용으로 전 구간 한글 깨짐 방지 |

<br>

## 5. 역할
**팀원 (4인 프로젝트) — 로그인/회원가입 풀스택 개발 및 프로젝트 발표 담당**

- **프론트엔드:** 로그인/회원가입 UI 설계 및 유효성 검사 로직(`JavaScript`) 구현
- **백엔드:** 서블릿 기반 인증 로직 구현 및 데이터베이스(`MySQL`) 연동
- **로그인 유지:** Cookie와 Token 발급 방식을 혼합한 자동 로그인 기능 구현
- **공통 기능:** 인코딩 필터 적용을 통한 프로젝트 데이터 정합성 유지
- **발표:** 프로젝트 핵심 로직 및 시연 시나리오 구성, 최종 결과물 발표 진행

<br>

## 6. 화면 UI

### 6-1. 로그인 및 회원가입
<p align="center">
  <img width="49%" alt="로그인" src="https://github.com/user-attachments/assets/73c6ff49-5f8a-4f18-9f13-b6669fe4556a" />
  <img width="49%" alt="회원가입" src="https://github.com/user-attachments/assets/6bfd57af-a10a-489e-b0db-40cdbf17c39c" />
</p>

### 6-2. 회원가입 유효성 검사
<p align="center">
  <img width="80%" alt="회원가입-유효성" src="https://github.com/user-attachments/assets/1e48f1a5-52ed-4b86-a1cd-66f3c6b67589" />
</p>

<br>

## 7. 느낀점
- 프로젝트 설계 단계에서 관리자 권한을 충분히 고려하지 못하여 임시로 특정 계정에만 관리 기능을 부여하는 방식으로 보완했습니다.<br>
이 과정에서 구현보다 설계가 훨씬 중요하다는 것을 깨달았고 앞으로는 탄탄한 설계를 최우선으로 하는 개발자로 성장하겠습니다.
