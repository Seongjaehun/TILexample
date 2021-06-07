# 원격 저장소 (remote repository)

## 기본 설정

1. 로컬 git 저장소 준비 (로컬 저장소: 컴퓨터 내에 만드는 폴더 및 파일)
2. Github repository 생성
3. Repository default branch 변경 (settings -> repositories)
   - main -> master로 변경

<br>

# 명령어

## 원격 저장소 주소 추가

```bash
$ git remote add origin 저장소URL
```

> "git아, 원격 저장소(remote) 추가해줘(add) origin 이라는 이름으로 저장소 URL을!"

- origin은 원격 저장소 이름!

<br>

```bash
$ git remote -v # 제대로 원격 저장소가 추가되었는지 확인

origin  https://github.com/Seongjaehun/TIL.git (fetch)
origin  https://github.com/Seongjaehun/TIL.git (push)
```

> 잘못 add한 경우
>
> ~~~bash
> $ git remote rm origin
> ~~~

<br>

## 원격 저장소에 업로드 (push)

```bash
git push -u origin master
```

> "git아, push 해줘 origin이라는 이름의 원격저장소에 master 브랜치로!"

> **원격 저장소에는 commit이 올라간다.**
>
> 즉, commit 이력이 없다면 push 할 수 없으며, commit 이력에 있는 대상만 올라감

