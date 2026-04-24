# 3D Bag Store - 프리미엄 가방 쇼핑몰

Three.js를 사용한 3D 가방 쇼핑몰 웹 애플리케이션입니다.

## 기능

- 🎨 3D 가방 모델 뷰어
- 🔄 360도 회전 가능
- 🎨 색상 선택 (5가지 색상)
- 🔢 수량 선택 (1-99개)
- 💰 할인율 표시
- 🛒 장바구니 담기 기능
- 📱 반응형 디자인

## 기술 스택

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **3D Graphics**: Three.js, GLTFLoader
- **Styling**: Tailwind CSS
- **Icons**: SVG Icons

## 로컬 실행

```bash
# Python 3
python3 -m http.server 8080

# Node.js (설치 필요)
npx serve .

# 또는 Live Server 확장기 사용
```

## 배포

### GitHub Pages를 통한 배포

1. 이 레포지토리를 GitHub에 푸시
2. Settings > Pages로 이동
3. Source를 "Deploy from a branch"로 설정
4. Branch를 "main"과 "/root"로 선택
5. Save 클릭

### Netlify를 통한 배포

1. [Netlify](https://netlify.com)에 가입
2. "New site from Git" 선택
3. GitHub 레포지토리 연결
4. Build settings:
   - Build command: `echo "No build required"`
   - Publish directory: `.`
5. Deploy site 클릭

### Vercel을 통한 배포

1. [Vercel](https://vercel.com)에 가입
2. "New Project" 선택
3. GitHub 레포지토리 연결
4. Framework Preset: "Other"
5. Deploy 클릭

## 파일 구조

```
3d_web/
├── index.html          # 메인 페이지
├── assets/            # 3D 모델 파일
│   ├── leatherbag.glb
│   ├── casualhandbag.glb
│   ├── redhandbag.glb
│   └── handbag.glb
├── css/
│   └── style.css      # 스타일시트
├── js/
│   └── main.js        # 자바스크립트
└── README.md          # 프로젝트 설명
```

## 주요 기능 설명

### 3D 모델 뷰어
- Three.js를 사용하여 3D 가방 모델 로드
- 마우스 드래그로 360도 회전
- 터치 디바이스 지원

### 상품 선택
- 색상 선택: 브라운, 블랙, 화이트, 코랄, 티얼
- 수량 선택: 1-99개까지 선택 가능
- 실시간 가격 및 할인율 표시

### 쇼핑 기능
- 장바구니에 상품 담기
- 선택한 옵션(색상, 수량) 정보 전달
- 장바구니 아이콘 애니메이션 효과

## 브라우저 호환성

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 라이선스

MIT License
