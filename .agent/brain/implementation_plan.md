# GitHub 환경 설정 계획

## 목표
사용자 시스템에 Git과 GitHub CLI를 설치하여 버전 관리 및 GitHub 연동을 가능하게 합니다.

## 사용자 검토 필요 사항
> [!IMPORTANT]
> 이 계획은 `winget`을 사용하여 시스템에 소프트웨어(`Git` 및 `GitHub CLI`)를 설치하는 작업을 포함합니다.
> 설치 명령어를 승인해주셔야 합니다.
> 설치 후, 브라우저 연동이 필요한 GitHub CLI 인증(`gh auth login`)은 사용자가 직접 수행해야 할 수도 있습니다.

## 변경 제안 사항
### 시스템 설정
- **Git 설치**: `winget`을 사용하여 Git을 설치합니다.
- **GitHub CLI 설치**: `winget`을 사용하여 `gh`를 설치합니다.

### Git 설정
- **사용자 구성**: `user.name`과 `user.email`을 전역으로 설정합니다 (사용자 입력 필요).
- **저장소 초기화**: 현재 프로젝트 디렉토리에 Git 저장소가 없다면 초기화합니다.

## 검증 계획
### 자동 검증
- `git --version` 명령어로 Git 설치 확인.
- `gh --version` 명령어로 GitHub CLI 설치 확인.
- `git status` 명령어로 저장소 초기화 확인.

### 수동 검증
- 사용자가 `gh auth login`을 실행하여 인증 완료.
