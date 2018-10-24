# 생활코딩 - 지옥에서 온 Git 내용 요약
> 생활코딩 - 지옥에서 온 Git 내용 요약

개인적으로 생활코딩 지옥에서 온 Git 내용을 요약합니다.

출처 [생활코딩 지옥에서 온 Git](https://opentutorials.org/course/2708/15242)

## 저장소 만들기

폴더를 만듭니다.:

```sh
mkdir github-general-guide
```

디렉토리로 이동
```sh
cd github-general-guide
```

현재 디렉토리를 git의(버전)저장소로 만듬
```sh
git init
```

## Git이 관리할 대상으로 파일 등록
파일 생성

```sh
vim f1.txt
```

git이 파일을 추적하도록 명령
```sh
git add f1.txt
```
프로젝트 폴더의 상태를 확인
```sh
git status
```

## 버전 만들기(commit)
### 버전은 의미 있는 변화(완결된 상태)
버전을 만든 사람에 대한 정보를 설정합니다. 이 설정은 ~.gitconfig파일에 저장되고 1번만 해주면 됩니다.

```sh
git config --global user.name "자신의 닉네임"
git config --global user.email "자신의 이메일"
```
## Stage area
- commit 대기 상태를 stage area 라고 합니다. stage area는 commit 대기 상태의 파일들이 가는 곳
- repository: commit이 된 결과가 저장되는 곳 

```sh
git config --global user.name "자신의 닉네임"
git config --global user.email "자신의 이메일"
```

## 변경사항 확인하기
- 로그에서 출력되는 버전 간의 차이점을 출력하고 싶을 때 
```sh
git log -p 
```

- 버전 간의 차이점을 비교할 때
```sh
git diff '버전 id'..'버전 id2'
```

- git add하기 전과 add한 후의 파일 내용을 비교할 때 
```sh
git diff
```

## 과거의 버전으로 돌아가기
- reset VS revert
- reset: 커밋을 취소하고 해당 버전으로 가고 이전 버전들은 삭제
- revert: 커밋을 취소하고 새로운 버전을 만듬


아래 명령은 버전 id로 돌아가는 명령입니다. 
```sh
git reset --hard "버전 id" 
```

버전 id의 커밋을 취소한 내용을 새로운 버전으로 만드는 명령
```sh
git revert "버전 id"
```

## 명령의 빈도와 메뉴얼 보는 방법
명령의 빈도수
 > 아래 명령어들이 40%를 차지함

- commit
- add
- log
- diff
- init

## 수련해봅시다.

## Git의 원리

## gistory 설치
분석도구 gitstory 소개
gistory는 git을 분석하기 위한 도구입니다. 명령을 내렸을 때 git의 내부에서는 어떤 일이 일어나는가를 분석하면서 git이 어떻게 동작하는가를 스스로 공부하는데 도움을 드리기 위해서 고안된 도구입니다. 


* 설치
> gistory로 설치하신분들 중에 .git이 있는 폴더에서 gistroy명령어 못찾는다고 나오시는 분들은
> 1) pip설치 : sudo easy_install pip
> 2) gistory설치 : sudo pip install gistory
하신다음에 gistory실행해 보세요~

## git add의 원리
## objects 파일명의 원리
## 업데이트 내역

* 0.0.1
    * 작업 진행 중

## 정보

이름:정지현 – [@블로그주소](http://stophyun.tistory.com/) 
이메일주소 – jihyunjeong.me@gmail.com

XYZ 라이센스를 준수하며 ``LICENSE``에서 자세한 정보를 확인할 수 있습니다.

[https://github.com/yourname/github-link](https://github.com/dbader/)

## 기여 방법

1. (<https://github.com/yourname/yourproject/fork>)을 포크합니다.
2. (`git checkout -b feature/fooBar`) 명령어로 새 브랜치를 만드세요.
3. (`git commit -am 'Add some fooBar'`) 명령어로 커밋하세요.
4. (`git push origin feature/fooBar`) 명령어로 브랜치에 푸시하세요. 
5. 풀리퀘스트를 보내주세요.

<!-- Markdown link & img dfn's -->
[npm-image]: https://img.shields.io/npm/v/datadog-metrics.svg?style=flat-square
[npm-url]: https://npmjs.org/package/datadog-metrics
[npm-downloads]: https://img.shields.io/npm/dm/datadog-metrics.svg?style=flat-square
[travis-image]: https://img.shields.io/travis/dbader/node-datadog-metrics/master.svg?style=flat-square
[travis-url]: https://travis-ci.org/dbader/node-datadog-metrics
[wiki]: https://github.com/yourname/yourproject/wiki