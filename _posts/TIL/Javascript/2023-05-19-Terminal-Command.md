---
title: Terminal Command
categories: [Today I Learned, Javascript]
tags: [Javascript] # TAG names should always be lowercase
---

### Print Working Directory

- 현재 디렉토리까지 경로 출력

```bash
pwd
```

<br>

### Change Directory

- 디렉토리 이동

```zsh
cd <dirname>
```

- 상위 디렉토리 이동

```zsh
cd ..
```

- 홈 디렉토리 이동

```zsh
cd ~
```

<br>

### Create

- 파일 생성

```zsh
touch <filename>
```

- 디렉토리 생성

```zsh
mkdir <dirname>
```

<br>

### REMOVE

- 파일 삭제

```zsh
rm <filename>
```

- 디렉토리 포함 내부 파일 전체 삭제

```zsh
rm -rf <dirname>
```

- 디렉토리 삭제 [비어있는 폴더]

```zsh
rmdir <dirname>
```

<br>

### Concatenate

- 파일 내용보기

```zsh
cat <filename>
```

<br>

### List

- 현재 경로의 파일 및 디렉토리 조회

```zsh
ls
```

- 현재 경로의 숨김파일 및 디렉토리 포함 조회

```zsh
ls -a
```

- 숨김파일 및 디렉토리 포함 리스트 출력

```zsh
ls -al
```

<br>

### Vi

- 문서 편집

```zsh
vi <filename>
        #a (입력모드)
        #i (입력모드)
        #ESC (입력모드 나가기)
        #:w (저장)
        #:q (닫기)
        #:wq (저장 및 닫기)
```
