# 🚀 GitHub 프로필 꾸미기 가이드

## 📋 단계별 설치 방법

### 1️⃣ GitHub에 새 Repository 만들기

1. GitHub에 로그인
2. 우측 상단 `+` 버튼 클릭 → `New repository` 선택
3. Repository 이름을 **RuBinJang**으로 입력
4. **Public**으로 설정
5. ✅ `Add a README file` 체크 (이미 README가 있으므로 나중에 덮어쓰기)
6. `Create repository` 클릭

> ⚠️ **중요**: Repository 이름은 RuBinJang으로 해주세요!

---

### 2️⃣ 파일 업로드하기

#### 방법 A: 웹 인터페이스 사용 (간단)

1. 생성된 repository 페이지로 이동
2. 기존 README.md 파일 클릭
3. 연필 아이콘(Edit) 클릭
4. 내용을 모두 지우고 새로 만든 README.md 내용 복사 붙여넣기
5. `Commit changes` 클릭

#### 방법 B: Git 명령어 사용 (추천)

```bash
# 1. 프로필 README 폴더로 이동
cd github-profile-readme

# 2. Git 초기화
git init

# 3. 모든 파일 추가
git add .

# 4. 커밋
git commit -m "feat: 창의적인 프로필 README 추가"

# 5. GitHub repository와 연결
git remote add origin https://github.com/JangRuBin2/RuBinJang.git

# 6. 기본 브랜치를 main으로 설정
git branch -M main

# 7. Push
git push -u origin main --force
```

---

### 3️⃣ Snake Animation 설정 (선택사항)

Snake animation이 작동하려면 GitHub Actions를 활성화해야 합니다:

1. Repository의 `Settings` 탭 클릭
2. 좌측 메뉴에서 `Actions` → `General` 클릭
3. `Workflow permissions`에서 **Read and write permissions** 선택
4. `Allow GitHub Actions to create and approve pull requests` 체크
5. `Save` 클릭

> Snake animation은 매일 자동으로 업데이트되며, 처음 실행은 수동으로 해야 할 수 있습니다.
> Repository의 `Actions` 탭에서 `Generate Snake Animation` 워크플로우를 찾아 `Run workflow` 버튼을 클릭하세요.

---

### 4️⃣ 개인 정보 수정하기

README.md 파일에서 다음 부분을 본인 정보로 수정하세요:

#### 연락처 링크 (하단 "Connect With Me" 섹션)

```markdown
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:your.email@example.com)
```
↓ 수정
```markdown
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:실제이메일@gmail.com)
```

#### 소셜 링크
- LinkedIn URL 수정
- Portfolio URL 수정
- Blog URL 수정 (없으면 해당 줄 삭제)

#### About Me 섹션
```typescript
const rubin = {
    location: "Korea 🇰🇷",  // 본인 위치
    role: "Web Developer",    // 본인 역할
    workingOn: "Building amazing web experiences",  // 현재 작업
    learning: ["Next.js", "TypeScript", "Modern Web Architecture"],  // 학습 중인 기술
    motto: "Code with passion, design with purpose"  // 본인 모토
};
```

---

## 🎨 커스터마이징 옵션

### 테마 변경

GitHub Stats 카드의 테마를 변경하고 싶다면:

```markdown
<!-- 현재: theme=radical -->
<img src="https://github-readme-stats.vercel.app/api?username=RuBinJang&theme=radical..."/>

<!-- 다른 테마 옵션: -->
- theme=dark
- theme=tokyonight
- theme=dracula
- theme=monokai
- theme=gruvbox
- theme=onedark
```

### 기술 스택 아이콘 변경

```markdown
<!-- 현재 아이콘 -->
<img src="https://skillicons.dev/icons?i=js,ts,html,css,react,nextjs,nodejs,vue" />

<!-- 다른 옵션들: -->
i=python,java,cpp,go,rust,php,ruby,swift
i=docker,kubernetes,aws,gcp,azure
i=mongodb,postgresql,mysql,redis
```

전체 아이콘 목록: https://skillicons.dev

### 색상 커스터마이징

README의 주요 색상은 보라색(#A855F7)입니다. 변경하려면:

1. README.md에서 `A855F7` 검색
2. 원하는 hex 색상 코드로 변경

---

## ✅ 확인 사항

완료 후 다음을 확인하세요:

- [ ] Repository 이름이 username과 동일한가?
- [ ] Repository가 Public으로 설정되어 있는가?
- [ ] README.md가 repository 루트에 있는가?
- [ ] 프로필 페이지에서 README가 보이는가?
- [ ] 개인 정보(이메일, 링크 등)를 수정했는가?
- [ ] GitHub Actions 권한을 설정했는가? (Snake animation 사용 시)

---

## 🔧 문제 해결

### 프로필에 README가 안 보여요
- Repository 이름을 확인하세요 (username과 정확히 일치해야 함)
- Repository가 Public인지 확인하세요
- 파일 이름이 `README.md`인지 확인하세요 (대소문자 구분)

### GitHub Stats가 안 나와요
- 잠시 기다려보세요 (API 응답에 시간이 걸릴 수 있음)
- Repository가 Public인지 확인하세요
- Username이 정확한지 확인하세요

### Snake animation이 안 나와요
- GitHub Actions 권한을 확인하세요
- Actions 탭에서 워크플로우가 성공했는지 확인하세요
- 처음에는 수동으로 워크플로우를 실행해야 할 수 있습니다

---

## 📚 추가 리소스

- [GitHub Profile README Generator](https://rahuldkjain.github.io/gh-profile-readme-generator/)
- [Awesome GitHub Profile README](https://github.com/abhisheknaiidu/awesome-github-profile-readme)
- [Shields.io](https://shields.io/) - 커스텀 뱃지 만들기

---

**즐거운 프로필 꾸미기 되세요! 🎉**
