# 🤝 The Jumper 프로젝트 기여 가이드

The Jumper 프로젝트에 관심을 가져주셔서 감사합니다! 이 문서는 프로젝트에 기여하는 방법을 안내합니다.

## 📋 목차

- [시작하기 전에](#시작하기-전에)
- [개발 환경 설정](#개발-환경-설정)
- [기여 방법](#기여-방법)
- [코드 스타일](#코드-스타일)
- [커밋 메시지 규칙](#커밋-메시지-규칙)
- [Pull Request 가이드](#pull-request-가이드)
- [이슈 리포트](#이슈-리포트)

## 🚀 시작하기 전에

### 기여할 수 있는 방법들
- 🐛 **버그 리포트**: 게임에서 발견한 버그를 신고
- 💡 **기능 제안**: 새로운 기능이나 개선사항 제안
- 🔧 **코드 기여**: 버그 수정, 새 기능 구현, 성능 개선
- 📖 **문서 개선**: README, 주석, 가이드 개선
- 🎨 **디자인**: UI/UX 개선, 그래픽 리소스 제공
- 🧪 **테스트**: 게임 테스트 및 품질 보증

## 💻 개발 환경 설정

### 필수 요구사항
- 최신 웹 브라우저 (Chrome, Firefox, Safari, Edge)
- 텍스트 에디터 또는 IDE (VS Code 권장)
- Git

### 설정 단계
1. 리포지토리 포크
```bash
# GitHub에서 Fork 버튼 클릭 후
git clone https://github.com/YOUR_USERNAME/the-jumper.git
cd the-jumper
```

2. 원본 리포지토리를 upstream으로 추가
```bash
git remote add upstream https://github.com/ORIGINAL_OWNER/the-jumper.git
```

3. 로컬 서버 실행 (선택사항)
```bash
# Python 3
python -m http.server 8000

# Node.js
npx serve .

# 또는 브라우저에서 직접 index.html 열기
```

## 🛠️ 기여 방법

### 1. 이슈 확인
- 기존 이슈를 먼저 확인해주세요
- 중복된 이슈가 있는지 검색해보세요
- 새로운 이슈라면 이슈를 생성해주세요

### 2. 브랜치 생성
```bash
git checkout -b feature/your-feature-name
# 또는
git checkout -b bugfix/issue-number-description
```

### 3. 변경사항 적용
- 코드를 수정하거나 새 기능을 추가합니다
- 변경사항을 테스트합니다

### 4. 커밋 및 푸시
```bash
git add .
git commit -m "feat: add awesome new feature"
git push origin feature/your-feature-name
```

### 5. Pull Request 생성
- GitHub에서 Pull Request를 생성합니다
- 템플릿에 따라 상세한 설명을 작성합니다

## 🎨 코드 스타일

### JavaScript 스타일
```javascript
// ✅ 좋은 예
class Player {
    constructor() {
        this.x = 0;
        this.y = 0;
        this.velocity = { x: 0, y: 0 };
    }
    
    jump() {
        if (this.onGround) {
            this.velocity.y = -15;
        }
    }
}

// ❌ 나쁜 예
class player{
var x=0,y=0;
function jump(){if(this.onGround)this.velocity.y=-15;}
}
```

### CSS 스타일
```css
/* ✅ 좋은 예 */
.game-container {
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(135deg, #1a1a2e, #16213e);
}

/* ❌ 나쁜 예 */
.game-container{display:flex;justify-content:center;background:#1a1a2e;}
```

### 일반 규칙
- **들여쓰기**: 4칸 스페이스
- **네이밍**: camelCase 사용
- **주석**: 복잡한 로직에는 주석 추가
- **함수**: 한 가지 일만 하는 작은 함수
- **변수**: 의미있는 변수명 사용

## 📝 커밋 메시지 규칙

### 커밋 메시지 형식
```
type(scope): description

[optional body]

[optional footer]
```

### 타입별 예시
```bash
# 새 기능
git commit -m "feat: add double jump ability"

# 버그 수정
git commit -m "fix: collision detection with spikes"

# 문서 업데이트
git commit -m "docs: update README with new controls"

# 스타일 변경
git commit -m "style: improve player glow effect"

# 리팩토링
git commit -m "refactor: optimize particle system performance"

# 테스트 추가
git commit -m "test: add collision detection tests"
```

### 커밋 타입들
- `feat`: 새로운 기능
- `fix`: 버그 수정
- `docs`: 문서 변경
- `style`: 코드 스타일 변경 (기능 변경 없음)
- `refactor`: 리팩토링
- `test`: 테스트 추가/수정
- `chore`: 빌드, 설정 파일 수정

## 🔍 Pull Request 가이드

### PR 제목
- 명확하고 간결하게 작성
- 커밋 메시지 규칙과 동일한 형식 사용

### PR 설명 템플릿
```markdown
## 변경사항
- [ ] 새 기능 추가
- [ ] 버그 수정
- [ ] 문서 업데이트
- [ ] 성능 개선

## 상세 설명
이 PR에서 구현한 내용을 자세히 설명해주세요.

## 테스트
- [ ] 로컬에서 테스트 완료
- [ ] 브라우저 호환성 확인
- [ ] 모바일에서 테스트 완료

## 스크린샷 (해당시)
변경사항을 보여주는 스크린샷이나 GIF를 첨부해주세요.

## 관련 이슈
Closes #123
```

### 리뷰 프로세스
1. 자동 체크 통과 확인
2. 코드 리뷰 대기
3. 피드백 반영
4. 승인 후 머지

## 🐛 이슈 리포트

### 버그 리포트 템플릿
```markdown
## 버그 설명
버그에 대한 명확하고 간결한 설명

## 재현 방법
1. '...' 페이지로 이동
2. '...' 버튼 클릭
3. '...' 입력
4. 오류 발생

## 예상 동작
무엇이 일어날 것으로 예상했는지 설명

## 실제 동작
실제로 무엇이 일어났는지 설명

## 스크린샷
가능하다면 스크린샷 첨부

## 환경 정보
- OS: [예: Windows 10]
- 브라우저: [예: Chrome 91.0]
- 디바이스: [예: Desktop, Mobile]

## 추가 정보
기타 참고할만한 정보
```

### 기능 제안 템플릿
```markdown
## 기능 설명
새로운 기능에 대한 명확한 설명

## 해결하려는 문제
이 기능이 해결하는 문제나 개선점

## 제안하는 해결책
어떻게 구현할지에 대한 아이디어

## 대안
고려해본 다른 해결책들

## 추가 정보
기타 참고할만한 정보나 예시
```

## 🎯 개발 우선순위

### 높은 우선순위
1. 🐛 **치명적 버그**: 게임을 플레이할 수 없게 만드는 버그
2. 🔒 **보안 이슈**: 보안 관련 문제들
3. 📱 **접근성**: 모든 사용자가 게임을 즐길 수 있도록

### 중간 우선순위
1. 🎮 **게임플레이 개선**: 새로운 기능, 밸런스 조정
2. 🎨 **UI/UX 개선**: 사용자 경험 향상
3. 🚀 **성능 최적화**: 게임 성능 개선

### 낮은 우선순위
1. 🎵 **추가 기능**: 배경음악, 효과음 등
2. 📖 **문서화**: README, 주석 개선
3. 🧪 **실험적 기능**: 새로운 아이디어 테스트

## 📞 도움이 필요하신가요?

- 💬 **토론**: [GitHub Discussions](https://github.com/your-username/the-jumper/discussions)
- 📧 **이메일**: your-email@example.com
- 🐛 **버그 리포트**: [Issues](https://github.com/your-username/the-jumper/issues)

## 🙏 감사합니다!

여러분의 기여가 The Jumper를 더 좋은 게임으로 만듭니다. 
작은 기여도 큰 도움이 됩니다! 🎮✨