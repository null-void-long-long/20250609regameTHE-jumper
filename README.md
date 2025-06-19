# 🎮 The Jumper

**The Jumper**는 지오메트리 대시에서 영감을 받은 리듬 기반 플랫포머 게임입니다. 네온 스타일의 사이버펑크 디자인과 중독성 있는 게임플레이를 제공합니다.

![Game Screenshot](https://img.shields.io/badge/Platform-Web-brightgreen) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)

## 🚀 게임 플레이

### 🎯 목표
- 장애물을 피하면서 최대한 멀리 이동하세요
- 금색 다이아몬드를 수집하여 높은 점수를 획득하세요
- 레벨을 완주하여 마스터가 되어보세요!

### 🎮 조작법
| 조작 | 액션 |
|------|------|
| **스페이스바** | 점프 |
| **마우스 클릭** | 점프 |
| **터치** | 점프 (모바일) |
| **R키** | 게임 재시작 |

## ✨ 주요 기능

### 🎨 비주얼 효과
- **네온 글로우**: 모든 게임 요소에 발광 효과
- **파티클 시스템**: 점프와 충돌 시 화려한 파티클
- **트레일 효과**: 플레이어 이동 궤적 표시
- **리듬 펄스**: 비트에 맞춘 화면 펄스 효과
- **동적 배경**: 움직이는 그리드와 배경 요소

### 🎪 게임 요소
- **🔺 가시 장애물**: 삼각형 모양의 치명적인 함정
- **🧱 벽 장애물**: 높이뛰기가 필요한 벽
- **🟨 플랫폼**: 점프할 수 있는 공중 발판
- **💎 수집 아이템**: 회전하는 다이아몬드 (100점)

### 🎭 게임 모드
- **일반 모드**: 클래식한 원샷 원킬 모드
- **연습 모드**: 체크포인트 시스템으로 구간 연습 가능

## 🛠️ 기술 스택

- **HTML5 Canvas**: 게임 렌더링
- **Vanilla JavaScript**: 게임 로직 및 물리 엔진
- **CSS3**: UI 스타일링 및 애니메이션
- **Web Audio API**: 리듬 및 사운드 효과 (예정)

## 🎯 게임 시스템

### 📊 점수 시스템
- **기본 점수**: 이동 거리에 비례 (1점/프레임)
- **아이템 보너스**: 다이아몬드 수집 시 100점
- **완주 보너스**: 레벨 완료 시 1000점

### 🏃‍♂️ 물리 엔진
- **중력**: 현실적인 점프 물리
- **충돌 감지**: 픽셀 퍼펙트 충돌 시스템
- **플랫폼 착지**: 위에서만 착지 가능
- **관성**: 부드러운 움직임과 회전

## 🚀 실행 방법

### 💻 로컬에서 실행
1. 리포지토리를 클론합니다
```bash
git clone https://github.com/your-username/the-jumper.git
cd the-jumper
```

2. HTML 파일을 브라우저에서 엽니다
```bash
# 방법 1: 파일 더블클릭
open index.html

# 방법 2: 로컬 서버 실행
python -m http.server 8000
# 또는
npx serve .
```

3. 브라우저에서 `http://localhost:8000`으로 접속

### 🌐 온라인 플레이
GitHub Pages에서 바로 플레이하세요: [플레이하기](https://your-username.github.io/the-jumper/)

## 📱 브라우저 지원

| 브라우저 | 지원 버전 |
|----------|-----------|
| Chrome | 60+ ✅ |
| Firefox | 55+ ✅ |
| Safari | 12+ ✅ |
| Edge | 79+ ✅ |
| Mobile Safari | 12+ ✅ |
| Chrome Mobile | 60+ ✅ |

## 🎮 게임 팁

### 🏆 고득점 전략
1. **리듬 맞추기**: 비트에 맞춰 점프하면 더 정확해집니다
2. **아이템 수집**: 모든 다이아몬드를 놓치지 마세요
3. **연습 모드**: 어려운 구간은 연습 모드로 마스터하세요
4. **타이밍**: 성급하게 점프하지 말고 타이밍을 기다리세요

### 🎯 초보자 가이드
- 처음에는 연습 모드로 시작하세요
- 장애물 패턴을 익히는 것이 중요합니다
- 점프 타이밍은 약간 이른 것이 좋습니다
- 화면을 너무 응시하지 말고 리듬을 느껴보세요

## 🔮 향후 업데이트 예정

### 🎵 v2.0 - 사운드 업데이트
- [ ] 배경 음악 추가
- [ ] 효과음 시스템
- [ ] 비트 동기화 개선

### 🎨 v3.0 - 시각 업데이트  
- [ ] 새로운 플레이어 스킨
- [ ] 배경 테마 변경
- [ ] 더 많은 파티클 효과

### 🎪 v4.0 - 게임플레이 확장
- [ ] 새로운 장애물 타입
- [ ] 파워업 아이템
- [ ] 멀티플레이어 모드

### 🛠️ v5.0 - 에디터 모드
- [ ] 레벨 에디터
- [ ] 커뮤니티 레벨 공유
- [ ] 리플레이 시스템

## 🤝 기여하기

프로젝트 개선에 참여해주세요! 

### 🐛 버그 리포트
버그를 발견하셨나요? [이슈](https://github.com/your-username/the-jumper/issues)를 등록해주세요.

### 💡 새 기능 제안
새로운 아이디어가 있으신가요? [토론](https://github.com/your-username/the-jumper/discussions)에서 공유해주세요.

### 🔧 Pull Request
1. 리포지토리를 포크합니다
2. 새 브랜치를 만듭니다 (`git checkout -b feature/AmazingFeature`)
3. 변경사항을 커밋합니다 (`git commit -m 'Add some AmazingFeature'`)
4. 브랜치에 푸시합니다 (`git push origin feature/AmazingFeature`)
5. Pull Request를 생성합니다

## 📄 라이센스

이 프로젝트는 MIT 라이센스 하에 배포됩니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.

## 🙏 감사의 말

- **지오메트리 대시**: 게임 컨셉 영감
- **웹 개발 커뮤니티**: 끝없는 학습 자료
- **플레이어들**: 피드백과 지원

## 📞 연락처

- **개발자**: [당신의 이름](mailto:your-email@example.com)
- **프로젝트**: [GitHub](https://github.com/your-username/the-jumper)
- **이슈**: [Issues](https://github.com/your-username/the-jumper/issues)

---

⭐ 이 프로젝트가 마음에 드셨다면 스타를 눌러주세요!  
🎮 지금 바로 플레이하고 최고 점수에 도전해보세요!

**만든 날짜**: 2025년 6월  
**최종 업데이트**: 2025년 6월  
**버전**: v1.0.0
