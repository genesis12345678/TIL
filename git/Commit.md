# 커밋 관리

### 작업을 커밋할 때 권장사항
1. 하나의 커밋에는 한 단위의 작업을 넣는다.
   - 한 작업을 여러 버전에 걸쳐 커밋하지 않는다.
   - 여러 작업을 한 버전에 커밋하지 않는다.
2. 커밋 메시지는 어떤 작업이 이뤄졌는지 알아볼 수 있어야 한다.

### 커밋 메시지 컨벤션

**공통으로 사용되는 커밋 메시지 작성방식**
```text
type: subject

body (optional)
...
...
...

footer (optional)
```
- 예시
```text
feat: 압축파일 미리보기 기능 추가

사용자의 편의를 위해 압축을 풀기 전에
다음과 같이 압축파일 미리보기를 할 수 있도록 함
 - 마우스 오른쪽 클릭
 - 윈도우 탐색기 또는 맥 파인더의 미리보기 창

Closes #125
```

**Type**

| 타입       | 설명                           |
|----------|------------------------------|
| feat     | 새로운 기능 추가                    |
| fix      | 버그 수정                        |
| docs     | 문서 수정                        |
| style    | 공백, 세미콜론 등 스타일 수정            |
| refactor | 코드 리팩토링                      |
| perf     | 성능 개선                        |
| test     | 테스트 추가                       |
| chore    | 빌드 과정 또는 보조 기능(문서 생성기능 등) 수정 |

**Subject**
- 커밋의 작업 내용 간략히 설명

**Body**
- 길게 설명할 필요가 있을 시 작성

**Footer**
- `Breaking Point`가 있을 때
- 특정 이슈에 대한 해결 작업일 떄

**[Gitmoji](https://gitmoji.dev/)를 사용해서 `Type`을 이모티콘으로 표현할 수도 있다.**

### 세심하게 스테이징 하고 커밋하기

다음 명령어로 `hunk`별 스테이징을 진행할 수 있다.
```text
git add -p
```
- `?` : 옵션 설명 보기
- `y` 또는 `n`으로 각 헝크 선택
- 이러면 한 파일에 대해서도 변경사항을 보다 세세하게 다루게 된다. 때문에 자연스럽게 같은 파일인데도 `Staging area`에도 있고, `Working directory`에 있게 된다.

변경사항을 확인하고 커밋하기
```text
git commit -v
```
- 이 명령으로 무엇이 변경되었나를 확인해보고 커밋을 진행할 수 있다.
- 위 `git add -p`로 헝크 별로 커밋을 하면 같은 파일 이더라도 부분(파트)별로 세세하게 나누어서 커밋을 할 수가 있다.

변경사항을 확인만 하기
```text
git diff --staged
```
- `git commit -v`는 변경사항 확인과 커밋을 동시에 하는 작업이라면 `git diff --staged`는 변경사항을 확인만 하는 작업을 한다.

### 커밋하기 애매한 변화 치워두기

현재 변경사항 치워두는 명령어
```text
git stash
```
- **`git add`로 스테이징에 올라가 있는 파일만 치워둔다.**
- `git stash save`와 같다.

원하는 시점, 원하는 브랜치에서 다시 적용하기
```text
git stash pop
```
- 가장 마지막에 치워둔 변경사항을 적용한다.
- `pop`말고 `apply`도 있는데, `pop`은 스태시를 삭제하면서 적용하고 `apply`는 적용하고 삭제하지는 않는다.

원하는 것만 치워두기
```text
git stash -p
```
- `git add -p`처럼 세세하게 스태시 처리 할 수 있다.
- 가장 마지막에 변경된 파일부터 물어본다.

메시지와 함께 스태시
```text
git stash -m "메시지"
```

스태시 목록 보기
```text
git stash list
```
- 리스트 상의 번호로 `apply`, `drop`, `pop`을 할 수 있다.
- 예) `git stash apply stash@{1}`

**참고로 스태시를 적용 한다는 것은 바로 커밋이 되어버리는 게 아니라 변경사항을 추가한다는 것이다.** 즉, 변경사항을 적용하고 추가 작업을 해서 `add`후 커밋할 수 있는 것이다.

**Stash 사용법 정리**

| 명령어                    | 설명                          | 비고                |
|------------------------|-----------------------------|-------------------|
| git stash              | 현 작업을 치워두기                  | 끝에 save 생략        |
| git stash apply        | 치워둔 마지막 항목(번호 없을 시) 적용      | 끝에 번호로 항목 지정 가능   |
| git stash drop         | 치워둔 마지막 항목(번호 없을 시) 삭제      | 끝에 번호로 항목 지정 가능   |
| git stash pop          | 치워둔 마지막 항목(번호 없을 시) 적용 및 삭제 | `apply` + `drop`  | 
| git stash branch(브랜치명) | 새 브랜치를 생성하여 pop             | 충돌사항이 있는 상황 등에 유용 |
| git stash clear        | 치워둔 모든 항목들 비우기              |                   |


### 커밋 수정하기

마지막 커밋 메시지 수정하기
```text
git commit --amend
```
또는
```text
git commit --amend -m "메시지"
```

과거 커밋 내역을 수정하는 다양한 방법

| 명령어         | 설명         |
|-------------|------------|
| `p`, pick   | 커밋 그대로 두기  |
| `r`, reword | 커밋 메시지 변경  |
| `e`, edit   | 수정을 위해 정지  |
| `d`, drop   | 커밋 삭제      |
| `s`, squash | 이전 커밋에 합치기 |

```text
git rebase -i  (변경하고 싶은 대상 커밋 바로 이전 커밋 해시)
```
- 이 명령어를 입력하면 편집기로 이동해서 각 커밋에 대해 재설정을 할 수 있다.
- `e` 명령어로 수정을 시작하면 개발자가 수정을 마칠 때까지 대기한다.
  - 예를 들어 한 커밋을 두 개의 커밋으로 나누어서 커밋을 재시도하려면 `git reset HEAD~`로 이전 커밋으로 돌아간 다음 변화들을 따로 스테이징 및 커밋 처리를 한다.
  - 그리고 `git rebase --continue`로 수정을 완료한다.

### 커밋 태그

**Git의 Tag**
- 특정 시점을 키워드로 저장하고 싶을 때
- 커밋에 버전 정보를 붙이고자 할 때
- 예를 들어 버전이 2.0.0일 때 이렇게 나눌 수 있다.
  - 2.(`MAJOR`), 0.(`MINOR`), 0(`PATCH`)
    - 기존 버전과 호환되지 않을 정보로 API가 바뀌면 `MAJOR` 버전을 올린다.
    - 기존 버전과 호환되면서 새로운 기능을 추가할 때는 `MINOR` 버전을 올린다.
    - 기존 버전과 호환되면서 버그를 수정한 정도라면 `PATCH` 버전을 올린다.

| 태그 종류       | 설명                            |
|-------------|-------------------------------|
| lightweight | 단순히 특정 커밋을 가리키는 용도            |
|annotated| 작성자 정보와 날짜, 메시지, GPG 서명 포함 가능 |

마지막 커밋에 태그 달기(`lightweight`)
```text
git tag (태그)
```
```text
git tag v2.0.0
```

현존하는 태그 확인
```text
git tag
```

원하는 태그의 내용 확인
```text
git show v2.0.0
```

태그 삭제
```text
git tag -d v2.0.0
```

마지막 커밋에 태그 달기(`annotated`)
```text
git tag -a v2.0.0
```
입력 후 메시지 작성 또는
```text
git tag v2.0.0 -m '설명'
```
- `-m`태그가 `-a`태그를 암시한다.

원하는 커밋에 태그 달기
```text
git tag (태그명) (커밋 해시) -m '메시지'
```

태그 필터링으로 조회
```text
git tag -l 'v1.*'
```
- 태그가 `v1.`으로 시작하는 모든 태그명 조회

원하는 버전으로 체크아웃
```text
git checkout v1.0.0
```

특정 태그 원격에 올리기
```text
git push (원격명) (태그명)
```
- `GitHub`에 태그가 추가된다.

특정 태그 원격에서 삭제
```text
git push --delete (원격명) (태그명)
```

로컬의 모든 태그 원격에 올리기
```text
git push --tags
```