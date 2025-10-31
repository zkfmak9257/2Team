# Source Tree 는 Atlassian에서 만든 Git GUI(그래픽 인터페이스) 툴입니다.
 - tip
  미리보기 시 표로 보실 수 있습니다.

터미널 명령어 없이도 Git을 시각적으로 쉽게 조작할 수 있게 도와주는 앱입니다.

## Source Tree 의 핵심 역할
 - 명령어 대신 클릭으로 Git 작업을 쉽게 관리하는 프로그램
---

| 기능 | 설명 | 대응되는 Git 명령어 |
|------|------|----------------------|
| **저장소 만들기 (Repository Init)** | 새로운 Git 저장소 생성 | `git init` |
| **클론(Clone)** | 원격 저장소를 로컬에 복사 | `git clone <url>` |
| **커밋(Commit)** | 변경된 파일을 저장소에 기록 | `git commit -m "message"` |
| **스테이징(Stage)** | 커밋할 파일 선택 | `git add <file>` |
| **푸시(Push)** | 로컬 변경사항을 원격에 업로드 | `git push origin <branch>` |
| **풀(Pull)** | 원격 변경사항을 로컬로 가져와 병합 | `git pull` |
| **페치(Fetch)** | 원격 변경사항만 가져오고 병합하지 않음 | `git fetch` |
| **리베이스(Rebase)** | 커밋 순서를 재정렬해 깔끔한 히스토리 유지 | `git rebase` |
| **병합(Merge)** | 다른 브랜치의 내용을 현재 브랜치에 합침 | `git merge <branch>` |
| **리셋(Reset)** | 특정 커밋 상태로 되돌림 (이전 커밋 삭제 가능) | `git reset --hard <commit>` |
| **리버트(Revert)** | 선택한 커밋의 변경사항을 반대로 되돌림 | `git revert <commit>` |
| **체리픽(Cherry-pick)** | 다른 브랜치의 특정 커밋만 가져오기 | `git cherry-pick <commit>` |
| **브랜치 생성(Create Branch)** | 새 작업 브랜치 만들기 | `git branch <branch>` |
| **브랜치 전환(Checkout)** | 작업할 브랜치 변경 | `git checkout <branch>` |
| **태그(Tag)** | 특정 커밋에 버전표시나 마일스톤 추가 | `git tag <name>` |
| **로그(Log)** | 커밋 히스토리 조회 | `git log --oneline --graph` |
| **충돌 해결(Merge Conflict)** | 병합 중 충돌난 파일 시각적으로 정리 | (자동 병합 도구 내장) |

---

## 🖥️ 주요 화면 구성 (Main Interface Layout)

| 구역 | 이름 | 설명 |
|------|------|------|
| **① 왼쪽 패널 (Sidebar)** | 브랜치, 원격 저장소, 태그, 스태시 등 Git 요소들을 목록으로 표시 | 어떤 브랜치에서 작업 중인지 쉽게 파악 가능 |
| **② 커밋 그래프 (Commit Graph)** | 브랜치별 커밋 흐름을 선으로 시각화 | 협업 시 브랜치 관계를 한눈에 확인 가능 |
| **③ 커밋 리스트 (Commit History)** | 선택한 브랜치의 커밋 기록 (커밋 메시지, 작성자, 날짜 등) | 최근 변경 내역 추적 가능 |
| **④ Diff 뷰어 (File Diff Viewer)** | 변경된 파일 내용을 비교(diff)해서 표시 | 추가/삭제된 라인 강조 표시 |
| **⑤ 하단 상세 창 (Details Pane)** | 선택된 커밋의 세부 내용, 변경된 파일 목록 | 특정 커밋의 실제 변경 내용 확인 가능 |
| **⑥ 상단 도구 바 (Toolbar)** | Pull, Push, Commit, Branch 등 주요 버튼 | Git 명령어를 클릭 한 번으로 실행 가능 |

---

## ⚙️ 자주 쓰는 기능 (Frequently Used Actions)

| 기능 | 설명 | 대응 Git 명령어 |
|------|------|----------------|
| **Commit** | 변경된 파일을 저장소에 기록 | `git commit -m "message"` |
| **Push** | 로컬 커밋을 원격 저장소로 업로드 | `git push origin <branch>` |
| **Pull** | 원격 저장소의 변경사항을 병합하여 가져오기 | `git pull` |
| **Fetch** | 원격 변경사항만 가져오고 병합은 안 함 | `git fetch` |
| **Merge** | 다른 브랜치의 변경사항을 현재 브랜치에 합치기 | `git merge <branch>` |
| **Rebase** | 커밋들을 다른 브랜치 위로 재배치 | `git rebase <branch>` |
| **Revert** | 특정 커밋의 변경사항을 되돌리는 새 커밋 생성 | `git revert <commit>` |
| **Reset** | 특정 커밋으로 되돌림 (히스토리 수정 가능) | `git reset --hard <commit>` |
| **Cherry-pick** | 다른 브랜치의 특정 커밋만 가져오기 | `git cherry-pick <commit>` |
| **Branch Create** | 새 브랜치 생성 | `git branch <name>` |
| **Checkout** | 다른 브랜치로 전환 | `git checkout <name>` |
| **Stash** | 작업 중인 변경사항을 임시로 저장 | `git stash` / `git stash pop` |
| **Tag** | 특정 커밋에 버전 표시 (릴리즈용) | `git tag v1.0.0` |

---

wjdqudwls