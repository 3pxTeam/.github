<div align="center">

# 3px Team 🎨

**디자인 파일을 위한 버전 관리 도구를 개발하는 팀입니다**

[![GitHub](https://img.shields.io/badge/GitHub-3px--team-black?style=flat&logo=github)](https://github.com/3px-team)
[![Project](https://img.shields.io/badge/Project-DGit-blue?style=flat&logo=git)](https://github.com/uzih05/DGIT)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat)]()

</div>

---

## 🚀 프로젝트

### DGit - 디자인 파일 버전 관리 시스템
<div align="center">
<!-- 프로젝트 아이콘 자리 -->
<img src="assets/icon.png" width="200px" alt="DGit Logo"/>
</div>

디자인 파일(.psd, .ai) 전용 버전 관리 시스템

- 🎯 **현재 상태**: CLI 기반 베타 버전 개발 완료
- 📁 **지원 형식**: Adobe Photoshop, Illustrator 파일 메타데이터 분석
- ⚙️ **기술**: Go, LZ4/Zstandard 압축 알고리즘
- 🔗 **CLI 저장소**: [3px-team/dgit-cli](https://github.com/3px-team/dgit-cli)
- 🖥️ **GUI 저장소**: [3px-team/dgit-desktop](https://github.com/3px-team/dgit-desktop)
- 🌐 **Web 저장소**: 개발예정
---

## 🛠️ 설치 및 사용법

### 📋 필요 조건
- Go 1.21 이상
- macOS, Windows, 또는 Linux

### ⚡ 빠른 설치

<table>
<tr>
<td width="50%">

#### 1️⃣ 소스코드에서 빌드
```bash
# 저장소 클론
git clone https://github.com/uzih05/DGIT.git
cd DGIT

# 빌드
go build -o dgit

# 전역 설치 (선택사항)
sudo mv dgit /usr/local/bin/
```

</td>
<td width="50%">

#### 2️⃣ 설치 확인
```bash
dgit --help
```

**출력 예시:**
```
🎨 DGit - Design File Version Control
Available Commands:
  init     Initialize repository
  add      Add files to staging
  commit   Create new version
  status   Check file status
  log      View history
  restore  Restore files
```

</td>
</tr>
</table>

### 🎯 5분만에 시작하기

```bash
# 1. 저장소 초기화
dgit init

# 2. 디자인 파일 추가
dgit add *.psd *.ai

# 3. 첫 번째 버전 생성
dgit commit -m "초기 디자인 파일"

# 4. 상태 확인
dgit status
```

### 📚 명령어 가이드

| 명령어 | 📝 설명 | 💡 예시 |
|--------|---------|---------|
| `dgit init` | 저장소 초기화 | `dgit init` |
| `dgit scan` | 디자인 파일 검색 | `dgit scan .` |
| `dgit add` | 파일 스테이징 | `dgit add *.psd` |
| `dgit commit` | 버전 생성 | `dgit commit -m "로고 업데이트"` |
| `dgit status` | 상태 확인 | `dgit status` |
| `dgit log` | 히스토리 조회 | `dgit log` |
| `dgit restore` | 파일 복원 | `dgit restore v2 logo.psd` |

---

## 👥 팀

<div align="center">

<table>
<tr>
<td align="center" width="33%">
<img src="https://github.com/uzih05.png" width="100px" style="border-radius: 50%"/><br>
<b>지헌</b><br>
<sub>🧑‍💻 팀장, 백엔드 개발</sub><br>
<a href="https://github.com/uzih05">@uzih05</a><br>
<code>Go</code> <code>Performance</code>
</td>
<td align="center" width="33%">
<img src="https://github.com/uijin0817.png" width="100px" style="border-radius: 50%"/><br>
<b>의진</b><br>
<sub>🎨 프론트엔드 개발</sub><br>
<a href="https://github.com/uijin0817">@uijin0817</a><br>
<code>React</code> <code>UI/UX</code>
</td>
<td align="center" width="33%">
<img src="https://github.com/Jihun0602.png" width="100px" style="border-radius: 50%"/><br>
<b>지훈</b><br>
<sub>💻 프론트엔드 개발</sub><br>
<a href="https://github.com/Jihun0602">@Jihun0602</a><br>
<code>React</code> <code>Web</code>
</td>
</tr>
</table>

</div>

---

## 📊 개발 현황

### ✅ 구현 완료
- [x] **CLI 버전**: 터미널에서 명령어로 사용 가능
- [x] **파일 분석**: PSD, AI 파일의 레이어, 크기, 색상 모드 추출
- [x] **압축 시스템**: 디자인 파일 효율적 저장
- [x] **기본 명령어**: `add`, `commit`, `status`, `log`, `restore`

### 🚧 현재 개발 중
- [ ] **데스크톱 GUI**: Electron 기반 그래픽 사용자 인터페이스
- [ ] **웹 인터페이스**: 브라우저 기반 관리 도구

### 📋 향후 개발 예정
- [ ] **UI/UX 개선**: 사용자 친화적 인터페이스
- [ ] **파일 형식 확장**: Sketch, Figma 지원
- [ ] **협업 기능**: 서버 구축을 통한 팀 협업

---

## 🛠️ 기술 스택

<div align="center">

**Backend**
<br>
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Compression](https://img.shields.io/badge/LZ4_Zstd-FF6B35?style=for-the-badge)

**Frontend**
<br>
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![Electron](https://img.shields.io/badge/Electron-191970?style=for-the-badge&logo=Electron&logoColor=white)

</div>

---

## 📖 문서

### 📁 지원 파일 형식

| 형식 | 지원 수준 | 분석 가능한 메타데이터 |
|------|-----------|----------------------|
| 🔵 **Adobe Photoshop (.psd)** | ✅ 완전 지원 | 레이어, 크기, 색상 모드, 비트 뎁스 |
| 🟠 **Adobe Illustrator (.ai)** | ✅ 완전 지원 | 아트보드, 레이어, 색상 공간 |
| 🟡 **Sketch (.sketch)** | 🔶 기본 지원 | 파일 크기, 수정 시간 |
| 🟢 **Figma (.fig)** | 🔶 기본 지원 | 파일 크기, 수정 시간 |

### 🔧 문제 해결
프로젝트 사용 중 문제가 발생하면 [Issues](https://github.com/uzih05/DGIT/issues)에 문의해주세요.

---

## 📞 연락처

<div align="center">

[![CLI Project](https://img.shields.io/badge/⌨️_CLI_Version-dgit--cli-blue?style=for-the-badge)](https://github.com/3px-team/dgit-cli)
[![Desktop Project](https://img.shields.io/badge/🖥️_Desktop_GUI-dgit--desktop-green?style=for-the-badge)](https://github.com/3px-team/dgit-desktop)
![Web Project](https://img.shields.io/badge/🌐_Web_Interface-dgit--web-orange?style=for-the-badge)

---
