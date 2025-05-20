## 👋 안녕하세요! 개발자 최재훈입니다

![header](https://capsule-render.vercel.app/api?type=wave&color=0:0C0C0C,100:1F1F1F&height=300&section=header&text=Welcome%20to%20CJH's%20GitHub&fontSize=60&fontColor=ffffff)

### 🚀 소개
- 🎯 **Java**, **Spring Boot**, **MariaDB** 기반의 백엔드 개발을 주력으로 합니다  
- 🤝 협업을 중요하게 생각하며, 함께 성장하는 개발 문화를 지향합니다  
- 🛠️ 단순 구현을 넘어, 문제를 구조적으로 해결하는 걸 좋아합니다  

---

### 💻 기술 스택

<p align="left">
  <img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white"/>
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB"/>
  <img src="https://img.shields.io/badge/React%20Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
</p>


---

### 📌 대표 프로젝트

> **GreenShare (1~2차)**  
> Raspberry Pi + Python 기반 스마트팜 IoT 기기 자동제어 시스템  
> React 기반 웹 연동으로 실시간 센서 시각화 및  
> 사용자 참여형 커뮤니티(JWT 인증, 게시판, 댓글, 좋아요) 구축  
> 🔗 https://github.com/cjh1939/greenShareFront.git  

---

> **GreenShare App (3차)**  
> React Native 기반 스마트팜 IoT 모바일 앱  
> Spring Boot REST API 연동 및 JWT 인증 포함  
> UI/UX 개선 및 커뮤니티 기능 모바일 최적화  
> 🔗 https://github.com/cjh1939/greenShareApp.git  

---

## 👨‍👩‍👧‍👦 팀원 소개

<table>
  <tr>
    <td align="center">
      <img src="https://avatars.githubusercontent.com/u/23456789?v=4" width="100px;" alt="정한길"/><br />
      <sub><b>정한길 </b></sub><br />
      <sub>👨‍💻 라즈베리파이 lot , 대쉬보드</sub><br />
      <a href="https://github.com/hankiljung"> GitHub</a>
    </td>
    <td align="center">
      <img src="https://avatars.githubusercontent.com/u/23456789?v=4" width="100px;" alt="이두용"/><br />
      <sub><b>이두용</b></sub><br />
      <sub>🏠 홈, 검색, 게시글 CRUD</sub><br />
      <a href="https://github.com/alee5899">GitHub</a>
    </td>
    <td align="center">
      <img src="https://avatars.githubusercontent.com/u/45678901?v=4" width="100px;" alt="조광진"/><br />
      <sub><b>조광진</b></sub><br />
      <sub>🛍게시글 에디터 , 웹소켓 , 라즈베리파이 iot </sub><br />
      <a href="https://github.com/PangJin97">GitHub</a>
    </td>
    <td align="center">
      <img src="https://avatars.githubusercontent.com/u/45678901?v=4" width="100px;" alt="최재훈"/><br />
      <sub><b>최재훈</b></sub><br />
      <sub>🔐 로그인, 팔로우, 좋아요 , 회원가입</sub><br />
      <a href="https://github.com/cjh1939/">GitHub</a>
    </td>
  </tr>
</table>






## 📁 프로젝트 구조 (1~2차 GreenShare – React 기반 웹 서비스)

```plaintext
📦 GREENSHAREFRONT
├── 📁 node_modules             # 설치된 외부 라이브러리
├── 📁 public                   # 정적 리소스 (favicon, index.html 등)
├── 📁 src                      # 프론트엔드 소스 디렉토리
│   ├── 📁 apis                 # 서버 통신(API) 모듈
│   │   ├── envApi.js          # 온습도, 조도, 가스 등 환경 센서 데이터 API
│   │   ├── plantStory.js      # 커뮤니티 게시글 관련 API
│   │   ├── qna.js             # Q&A 기능 API
│   │   ├── standardsApi.js    # 기준값 설정 관련 API
│   │   └── userApi.js         # 사용자 인증/정보 API
│   ├── 📁 assets               # 이미지, 폰트 등 정적 파일
│   ├── 📁 components           # 재사용 가능한 공통 컴포넌트 모음
│   ├── 📁 consts               # 상수 관리 (예: 센서 유형, 색상 정의 등)
│   ├── 📁 redux                # 상태 관리 (Redux)
│   │   ├── authCheck.js       # 로그인 체크 유틸
│   │   ├── authSlice.js       # 사용자 상태 슬라이스
│   │   ├── axiosInstance.js   # Axios 공통 인스턴스
│   │   └── store.js           # Redux Store 설정
│   ├── 📁 utils                # 날짜 포맷 등 공통 유틸 함수
│   ├── App.jsx                # App 루트 컴포넌트
│   ├── App.css                # 전역 스타일 정의
│   ├── main.jsx               # React 진입점
│   ├── index.css              # Reset 및 기본 스타일
├── index.html                 # HTML 템플릿
├── vite.config.js             # Vite 설정
├── package.json               # 프로젝트 정보 및 의존성
├── .gitignore                 # Git 제외 파일 목록
└── README.md                  # 프로젝트 설명 문서


### 📊 GitHub 활동

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=cjh1939&show_icons=true&theme=tokyonight)
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=cjh1939&layout=compact&theme=tokyonight)](https://github.com/anuraghazra/github-readme-stats)

---

### 📫 연락처
- 📧 이메일: `chemddhkd@gmail.com`
- 💼 LinkedIn: [linkedin.com/in/yourname](https://linkedin.com/in/yourname)

---

<!--
**cjh1939/cjh1939** 님의 프로필 README입니다 ✨  
이 파일은 GitHub 프로필 페이지에 자동으로 표시됩니다.
-->
