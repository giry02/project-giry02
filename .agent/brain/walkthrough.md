# GitHub 연결 작업 완료 보고서

## 작업 요약
사용자 요청에 따라 Git 및 GitHub CLI를 설치하고, GitHub 인증 및 원격 저장소 연결을 완료했습니다.

## 수행한 작업
1. **환경 확인 및 설치**:
   - `winget`을 통해 Git과 GitHub CLI 설치 완료.
2. **Git 설정**:
   - 사용자 이름: `giry02`
   - 이메일: `158979591+giry02@users.noreply.github.com` (GitHub 제공 noreply 주소 사용)
3. **GitHub 인증**:
   - `gh auth login`을 통해 브라우저 인증 완료.
4. **저장소 생성 및 연결**:
   - 로컬 저장소 초기화 (`git init`).
   - GitHub 원격 저장소 `project-giry02` 생성 (`gh repo create`).
   - 초기 코드 푸시 완료.

## 결과 확인
터미널에서 다음 명령어로 연결 상태를 확인할 수 있습니다:
```powershell
gh repo view --web
```
위 명령어를 입력하면 브라우저에서 생성된 GitHub 저장소 페이지가 열립니다.

## 저장소 링크
[giry02/project-giry02](https://github.com/giry02/project-giry02)
