<div align="center">
  <img src="profile/assets/icon.png" alt="3pxTeam Logo" width="120" height="120">
  
  # 3pxTeam

  디자인 워크플로우를 혁신하는 도구를 만듭니다.
</div>

## 우리가 해결하는 문제

Git은 개발자에게는 완벽하지만, 디자이너에게는 복잡합니다. 수 GB에 달하는 PSD 파일, 바이너리 형태의 Sketch 파일, 레이어 구조가 복잡한 디자인 에셋들... 기존 버전 관리 시스템으로는 한계가 있었습니다.

**DGit**은 디자인 파일을 위해 처음부터 다시 설계된 버전 관리 시스템입니다.

## 프로젝트

### 🚀 [DGit CLI](https://github.com/3pxTeam/DGIT-CLI)
디자인 파일 전용 버전 관리의 핵심 엔진
- Rust로 구현된 고성능 CLI 도구
- LZ4 압축을 통한 효율적인 대용량 파일 처리
- 레이어별 변경사항 추적 및 관리

### 🎨 [DGit macOS](https://github.com/3pxTeam/DGIT-MAC)
아름다운 네이티브 macOS 경험
- Electron 기반의 네이티브 macOS 인터페이스
- 드래그 앤 드롭 지원
- 시각적 커밋 히스토리 및 브랜치 관리

## 지원하는 파일 형식

| Adobe | Sketch | Figma | 기타 |
|-------|--------|-------|------|
| `.psd` | `.sketch` | `.fig` | `.png` |
| `.ai` | | `.figma` | `.jpg` |
| `.xd` | | | `.svg` |

## 왜 DGit인가?

- **속도**: 기존 Git 대비 5배 빠른 대용량 파일 처리
- **압축**: LZ4 알고리즘으로 평균 60% 용량 절약
- **직관성**: 복잡한 Git 명령어 없이 간단한 워크플로우
- **macOS 네이티브**: Mac 사용자를 위한 완벽한 통합

## 시작하기

```bash
# DGit CLI 설치
curl -sSL https://install.dgit.dev | sh

# 새 프로젝트 시작
dgit init
dgit add design.psd
dgit commit -m "첫 번째 디자인 버전"
```

[macOS GUI 다운로드](https://github.com/3pxTeam/DGIT-MAC/releases)에서 더 쉬운 시각적 인터페이스를 경험해보세요.

## 커뮤니티

- 💬 **이슈 & 토론**: [GitHub Issues](https://github.com/3pxTeam/DGIT-CLI/issues)
- 📢 **업데이트**: [Releases](https://github.com/3pxTeam/DGIT-CLI/releases) 페이지 팔로우
- 🔗 **피드백**: 실제 프로젝트에서 사용해보고 경험을 공유해주세요

## 기여하기

DGit은 디자인 커뮤니티와 함께 만들어갑니다:

- 🐛 **버그 리포트**: 문제를 발견하면 알려주세요
- 💡 **기능 제안**: 필요한 기능이 있다면 제안해주세요  
- 🔧 **코드 기여**: Pull Request로 직접 개발에 참여하세요
- 📖 **문서 개선**: 더 나은 사용법 가이드를 만들어주세요
