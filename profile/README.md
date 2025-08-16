<div align="center">
  <img src="assets/icon.png" alt="3pxTeam Logo" width="120" height="120">
  
  # 3pxTeam
  디자인 워크플로우를 개선하는 도구를 만듭니다.
</div>

## 우리가 해결하고자 하는 문제

Git은 개발자에게는 완벽하지만, 디자이너에게는 복잡합니다. 수십 MB에 달하는 PSD 파일, 바이너리 형태의 Sketch 파일, 레이어 구조가 복잡한 디자인 에셋들... 기존 버전 관리 시스템으로는 다루기 어려운 부분들이 있었습니다.

**DGit**은 이러한 디자인 파일의 특성을 고려하여 새롭게 설계한 버전 관리 시스템입니다.

## 프로젝트

### 🔧 [DGit CLI](https://github.com/3pxTeam/DGIT-CLI)
디자인 파일 버전 관리의 핵심 엔진

- **Go 언어 기반** CLI 도구
- **3단계 캐시 시스템**: LZ4 → Zstd → Archive 최적화
- **디자인 파일 메타데이터 추적**: 레이어, 크기, 색상 모드 변경 감지
- **지능형 압축**: 파일 특성에 따른 최적 알고리즘 선택

### 🎨 [DGit macOS](https://github.com/3pxTeam/DGIT-MAC)
직관적인 macOS 네이티브 인터페이스

- **Electron 기반** 크로스 플랫폼 GUI
- **macOS 스타일** 디자인 (다크 테마, 신호등 컨트롤)
- **시각적 프로젝트 관리**: 드래그 앤 드롭, 커밋 히스토리
- **CLI 통합**: 백엔드 DGit CLI와 완벽 연동

## 지원하는 파일 형식

| **완전 지원** | **기본 지원** | **일반 파일** |
|---------------|---------------|---------------|
| Adobe Photoshop (`.psd`) | Sketch (`.sketch`) | 이미지 파일 |
| Adobe Illustrator (`.ai`) | Figma (`.fig`) | 기타 바이너리 |
| | Adobe XD (`.xd`) | |

*완전 지원: 메타데이터 분석 및 변경 추적 / 기본 지원: 파일 버전 관리*

## DGit의 특징

- **효율적인 압축**: LZ4/Zstd 알고리즘으로 저장 공간 최적화
- **빠른 처리**: 3단계 캐시를 통한 성능 개선
- **디자이너 친화적**: 복잡한 Git 명령어 없이 간단한 워크플로우
- **메타데이터 추적**: 단순 파일 변경을 넘어 디자인 요소별 변경 사항 추적

## 시작하기

**CLI 버전:**
```bash
# 프로젝트 초기화
dgit init

# 파일 추가 및 커밋
dgit add design.psd
dgit commit -m "첫 번째 디자인 버전"

# 상태 확인
dgit status
```

**GUI 버전:**
[DGit macOS](https://github.com/3pxTeam/DGIT-MAC/releases)에서 시각적 인터페이스를 통해 더 쉽게 시작할 수 있습니다.

## 기술 스택

**CLI (핵심 엔진):**
- Go 언어
- LZ4/Zstd 압축 라이브러리
- 커스텀 파일 파서 (PSD/AI)

**GUI (macOS 인터페이스):**
- Electron + Node.js
- HTML/CSS/JavaScript
- 네이티브 macOS 스타일링

## 개발 현황

현재 로컬 버전 관리에 중점을 두고 있으며, 향후 클라우드 협업 기능과 더 많은 파일 형식 지원을 계획하고 있습니다.

## 피드백 및 기여

- 🐛 **이슈 리포트**: [GitHub Issues](https://github.com/3pxTeam/DGIT-CLI/issues)
- 💡 **기능 제안**: 실제 디자인 작업에서 필요한 기능을 제안해주세요
- 📖 **사용 경험**: 프로젝트를 사용해보시고 피드백을 공유해주세요
