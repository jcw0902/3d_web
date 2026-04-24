# 배포 가이드

## GitHub Pages를 통한 배포 단계

### 1. GitHub Pages 설정
1. GitHub 레포지토리로 이동: https://github.com/jcw0902/3d_web
2. Settings 탭 클릭
3. 왼쪽 메뉴에서 Pages 선택
4. Source 섹션에서 "Deploy from a branch" 선택
5. Branch: "main" 선택
6. Folder: "/ (root)" 선택
7. Save 버튼 클릭

### 2. 배포 확인
- 배포가 완료되면 다음 URL에서 접속 가능:
  - https://jcw0902.github.io/3d_web/
- 배포에는 보통 1-2분 소요

### 3. 대체 배포 옵션

#### Netlify 배포
1. https://netlify.com 접속
2. GitHub 계정으로 로그인
3. "New site from Git" 클릭
4. 3d_web 레포지토리 선택
5. Build settings:
   - Build command: 비워둠
   - Publish directory: 비워둄 (기본값)
6. "Deploy site" 클릭

#### Vercel 배포
1. https://vercel.com 접속
2. GitHub 계정으로 로그인
3. "New Project" 클릭
4. 3d_web 레포지토리 선택
5. Framework Preset: "Other" 선택
6. "Deploy" 클릭

## 배포 후 테스트 항목

- [ ] 3D 모델이 정상적으로 로드되는가?
- [ ] 색상 변경이 작동하는가?
- [ ] 수량 선택이 작동하는가?
- [ ] 장바구니 담기가 작동하는가?
- [ ] 모바일에서 반응형으로 표시되는가?
- [ ] 모든 브라우저에서 호환되는가?

## 문제 해결

### 3D 모델이 로드되지 않을 경우
- CORS 정책 확인
- 파일 경로 확인 (assets/ 폴더 내 파일)
- 콘솔 에러 확인

### 스타일이 깨질 경우
- Tailwind CSS CDN 로딩 확인
- CSS 파일 경로 확인
- 브라우저 캐시 삭제

## 배포 성공 확인
배포가 성공하면 다음 기능들이 웹에서 정상 작동합니다:
- 3D 가방 모델 뷰어
- 색상 및 수량 선택
- 할인율 표시
- 장바구니 기능
