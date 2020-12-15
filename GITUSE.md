### Git  local Update
```
$ git init : 빈 저장소를  local에 만들고 싶을 때
$ git status : local git의 상태 (빨간색으로 뜨면 안 올라갔다는 뜻)
$ git add . : every file updating local git
$ git commit -m " " : 어떤 파일인지 설명 하는 것
$ git log : git 기록 보여줌 (q 치면 빠져나올 수 있다)

```

#### 과거로 돌리기 
1. 현재 내용을 없애고 과거로 돌리기
```
commit 04657c210e29c99d21f7afa56aba5e9b13e23808
Author: ChaeChae0505 <chaey@koreatech.ac.kr>
Date:   Mon Dec 14 17:50:33 2020 +0900
```
- git log 의 commit 앞 6자리 복사 
```
$ git reset 04657c --hard
다시 미래로 못감
```
2. 과거 잠깐 다녀오기
```
$ git revert 04657c 
> wq
미래 시점 남아있음
```

### git brach

```
$ git brach <만들고 싶은 brach 명> : git brach 생성 > 이때 그 전에 있던 branch 상태를 그대로 가져감
$ git branch : brach 확인
$ git checkout <만든 branch> : <만든 branch>로 이동

> 두개 같이 하고 싶을 때 git checkout -b <새로운 branch 명>

> 하고 난 후 branch 그대로 github에 올리는 법
$ git add .
$ git commit -m "적고 싶은 말"
$ git push origin <새로만든 브랜치 명>
```


#### main brach로 이동
```
$ git checkout master : master branch로 이동하기
$ git merge <가져올 branch> : 합치는 방법
> 수정 파일이 다르면 merge가 잘 되지만 같은 파일을 수정하면 선택 해야함 
> 다른 브랜치에서 같은 파일 수정하는 것 안하는 것이 좋음
$ git rebase <가져올 branch> : 합칠 때 log기록에 한줄로 남는 merge 방법

$ git branch -D <없애고 싶은 git branch> : branch 없애는 방법



$ git log --graph --all --decorate : 변화를 시각화 해서 보여줌

```

### Github 사용하기
```
$ git config --global user.email "(내 메일 주소) "
$ git config --global user.name "(내 이름) "
$ git remote add origin {url} : url에 올리고 싶을 때 
$ git push -u origin master : 현재 status를 git master에 올린다

$ git remote : 올린 repository 이름 확인 가능
```
- 설정을 한번 해두면 아래와 같이 올릴 수 있다 
```
$ git add . : every file updating local git
$ git commit -m "1st" : git commit message
$ git push origin master : update local git ----> github 

```
- .gitignore !! 을 통해서 올려지지 않는 파일 설정 가능 


### git clone
```
$ git clone -b <branch> {url} : 원하는 branch 다운받고 싶을 때
$ git clone {url} : {url} 다운 받을 수 있음

$ git fetch : github에 수정 된 파일이 있는지 확인하는 법
$ git status : 원격이랑 다른 점 뜬다
$ git pull origin master(or branch명) : 원하는 브랜치 파일 받아 오는 법 

> pull 먼저 받고 작업하는게 무조건 좋음!!!!! 협업 시

$ git branch -a :  local / github 브랜치 어떻게 생성 되있는지 다 볼 수 있어 remotes/~(github)

```

$ rm -rf ./.git : git remove
$ git init : git initialize
$ git add . : every file updating local git
$ git status : status in local git
$ git commit -m "1st" : git commit message
$ git remote -v : when your git origin status
$ git push origin master : update local git ----> github 

$ git checkout -b <branch> : new <branch> and check in <branch> // local
$ git push --set-upstream origin <branch> : local branch upstream branch git hub 

### Windows 에서는 source tree 씁시다!!! 더 쉬워
