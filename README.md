# [Java Console Project(2023)] ERP 인사 관리 프로그램
Java Console창을 활용하여 제작한 ERP 인사 관리 프로그램입니다.

<br>

## 🔖 목차
- [📄 프로젝트 개요](#프로젝트-개요)
- [✒️ 기획 배경](#%EF%B8%8F기획-배경)
- [📌 구현 목표](#구현-목표)
- [👨‍👩‍👧‍👦 업무 분담](#업무-분담)
- [💻 주요 구현 기능](#주요-구현-기능)
- [📚 산출물](#산출물)

<br>

### 📄프로젝트 개요
- **프로젝트명**: ERP 인사 관리 프로그램
- **분류**: Java Console Project
- **주제**: Java Console창을 활용하여 간편한 인사 관리로 사용자/관리자 모두에게 불필요한 사무 절차를 줄일 수 있는 All-in-one 인사 관리 프로그램을 제작하고자 하였습니다.
- **개발 환경**: Java 11, Eclipse, Draw.io, Google Drive
- **사용 기술**: 파일 입출력 기반 데이터 처리
- **주요 기능**: 관리자의 기초 환경 설정·인사 관리·근태 관리·급여 관리·퇴직 관리·증명서 발급 승인 및 내역 조회 기능, 사용자(일반 회원)의 근태 이력 조회·연차 조회 및 신청·급여명세서 조회·조직도 및 부서별 현황 조회·마이페이지·증명서 발급 신청 기능
- **담당 업무**: 사용자 마이페이지 기능 및 증명서 발급 신청 기능, 관리자 증명서 발급 승인 및 조회 기능
- **획득 역량**: 프로그램 개발 절차, 파일 입출력 기반 데이터 처리, MVC 패턴에 기반한 패키지 설계
- **프로젝트 기간**: 2023.08.10 ~ 2023.08.24 (15일)

<br>

### ✒️기획 배경
: 기존 인사 관리 ERP 시스템에서 사용도가 높은 항목 위주로 시스템 재구성

<br>

### 📌구현 목표
1. `사용자/관리자별 기능 구현`
    1. 사용자: 사용자가 속한 조직 내 전반적인 인사 정보 확인 가능
        - 근태 확인
        - 연차 조회 및 신청
        - 급여명세서 확인
        - 부서별 현황 조회
        - 사용자 인사 정보 확인
        - 증명서 발급 신청
    2. 관리자: 전 직원의 인사 현황, 정보 수정, 급여 등의 관리 기능
        - 기초 환경 설정
        - 인사 관리
        - 근태 관리
        - 급여 관리
        - 퇴직 관리
        - 증명서 발급 신청 승인
2. `MVC Architecture Pattern 적용`
    - MVC 패턴에서 착안하여 View, Dao, Vo로 패키지를 구분하여 설계

<br>

### 👨‍👩‍👧‍👦업무 분담
- 김수진: 사용자 조직도, 부서별 현황 조회 기능, 사용자/관리자 연차 관련 기능, 관리자 인사 관련 기능
- **박나래**: 사용자 마이페이지 기능, 사용자/관리자 증명서 관련 기능, 발표
- 염현빈: Open API 기능, 로그인 기능, 관리자 퇴직금 관련 기능
- 임성은: 관리자 인사 관련 기능
- 차수민: Open API 기능, 사용자/관리자 근태 관련 기능
- 허수경: 사용자/관리자 급여 관련 기능

<br>

### 💻주요 구현 기능
1. 사용자 기능
    - 연차 조회 및 신청 → 연차 신청 내역 조회
      <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/44c198d6-fff2-4808-b602-3d42b2a66c42" alt="사용자 기능_연차신청내역조회">
    - 근태 확인 → 특정 월의 근태 내역 조회
      <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/96d755d1-f269-419b-8cfe-5a39235b50f0" alt="사용자 기능_특정월의근태내역조회">
    - 마이페이지 → 인사 현황 조회
      <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/48c455d5-a69d-4225-a6b6-603de7acd045" alt="사용자 기능_인사현황조회">
    - 마이페이지 → 비밀번호 변경
      <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/e5a5bb6e-b9cb-4cd1-a464-c4ddfe39ad5b" alt="사용자 기능_비밀번호변경">
    - 증명서 발급 신청
      <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/fff8807e-09c3-4d81-ac0f-a785de9bda42" alt="사용자 기능_증명서발급신청">
2. 관리자 기능
    - 급여관리정보 → 근로소득 일괄 입력 및 직원별 급여명세서 조회
      <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/09e7ae7d-5be7-4cba-b02f-699e0b989cee" alt="관리자 기능_급여관리정보">
    - 근태관리정보 → 출/퇴근 시간 조정
      <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/7463b552-4635-436f-a6dd-eb6cf370cda3" alt="관리자 기능_근태관리정보">
    - 증명서 발급 신청 승인
      <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/3def4962-87a8-4b6e-9b0c-23496a63d066" alt="관리자 기능_증명서발급신청승인">
    - 증명서 발급 신청 내역 조회
      <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/92081a12-dccc-43d0-91c9-d48a1f5b27cd" alt="관리자 기능_증명서발급신청내역조회">
<!--
<details>
    <summary>주요 구현 기능 미리보기 📷</summary>
        <div markdown="1">
            <img src="" alt="">
        </div>
</details>
-->
<br>

### 📚산출물
- 기획서 (3장)
- 요구분석서 (10장)
- 순서도
- 화면 설계서 (42장)
- 기능명세서 (22장)
- 데이터 관계도
- PPT
- 요약본 (5장)

<details>
    <summary>산출물 미리보기 📷</summary>
        <div markdown="1">
            <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/f8bd4857-3cba-461b-b4bd-94e159e37714" alt="기획서">
            <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/8543e75a-9599-4bbe-b8a8-144d157aa9a5" alt="요구분석서">
            <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/3731aed1-1b9e-42fb-8e4b-f9bf9e0f0d03" alt="순서도">
            <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/d86992c6-7f55-4b43-b389-c6f1a96e1f15" alt="화면 설계서">
            <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/22a8b8cf-b50b-4907-9f89-acceeb658154" alt="기능명세서">
            <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/fc32a38d-b052-4888-b40a-023e9043926a" alt="데이터 관계도">
            <img src="https://github.com/NaraeP/Java-Project_ERP/assets/140796673/2e3ad994-5c54-4347-a2bb-f071571d947b" alt="요약본">
        </div>
</details>
