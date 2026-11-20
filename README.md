# 서경인사이드 — Community Backend

SW 전문인재양성 팀 프로젝트에서 개발한 커뮤니티 웹 서비스의 Spring Boot 백엔드입니다.

게시판 및 회원 기능을 중심으로 구성된 커뮤니티 서비스를 위한 서버 애플리케이션으로, React 프론트엔드와 분리된 구조로 개발했습니다.

## 기술 스택

| 구분 | 기술 |
| --- | --- |
| Language | Java 21 |
| Framework | Spring Boot 4 |
| Web | Spring Web MVC |
| Persistence | Spring Data JPA |
| Database | MySQL |
| Build | Gradle |
| Container | Docker |
| CI/CD | GitLab CI |

## 프로젝트 구성

- Spring Boot 기반 서버 애플리케이션
- Spring Web MVC 기반 HTTP 요청 처리
- Spring Data JPA 및 MySQL 연동
- Gradle 기반 빌드 구성
- Docker 이미지 빌드 환경
- GitLab CI 공통 파이프라인 연결

## CI/CD 구성

백엔드 저장소의 `.gitlab-ci.yml`에서 공통 배포 저장소의 CI 설정을 참조하도록 구성했습니다.

GitLab Runner에서 Docker 이미지를 빌드한 뒤 Container Registry에 업로드하며, 테스트 환경 배포에 사용할 수 있도록 빌드된 이미지를 관리하는 구조입니다.

## 담당 역할 — CI/CD 환경 구성

백엔드 애플리케이션의 CI 빌드 설정과 실행 환경 구성 작업에 참여했습니다.

- Docker 이미지 빌드 및 Container Registry 업로드 설정
- Gradle Wrapper 실행 권한 설정
- GitLab Runner 아키텍처 설정
- Docker-in-Docker 서비스 설정 수정

CI/CD 구성과 관련 작업은 [Deploy 저장소](https://github.com/0rchid241/SW_Project_CICD_Deploy)에 정리했습니다.

## 관련 저장소

- [Community Frontend](https://github.com/0rchid241/SW_Project_CICD_Frontend)
- [Community Deploy](https://github.com/0rchid241/SW_Project_CICD_Deploy)
