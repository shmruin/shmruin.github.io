---
layout: single
title: "github.io 블로그 만드는 법"
---

# github.io 블로그 운영
github.io 블로그를 만들고 관리할 수 있는 방법에 대해서 남겨본다.

(정확히는 jekyll, 그 중에서도 [Minimal Mistakes Jekyll Theme](https://github.com/mmistakes/minimal-mistakes) 을 이용하여 만드는 법이 되겠다.)

다른 블로그에도 많이 소개되어 있지만 스스로 확인할 목적으로 중복해서 남긴다.  
[이 블로그](https://pnurep.github.io/blogging/github-page-minimal-mistakes/#remove-the-unnecessary)를 참조했다.

## github 계정 생성
github.io 블로그를 쓰려면 당연히 github 계정이 필요하다.

## minimal-mistake-jekyll 테마 페이지 Fork
테마를 다운로드 하는 방법도 있는 것 같지만 이게 제일 간단하다.

(그리고 테마 업데이트에도 쉽게 대응 가능하다)

그리고 해당 Fork Repo 의 이름을 `유저명.github.io` 로 변경해준다.

이 소스를 로컬에 Clone 하고 적당한 IDE 로 열어주자.

## 최상위 루트 아래 폴더 생성
* **_posts** : 포스트할 파일들을 담는 폴더
* **_pages** : 사용할 기타 페이지를 담는 폴더 (404.md 등)
* **_drafts** : 포스팅의 드래프트를 담는 폴더

## Ruby, Jekyll 및 번들러 설치
* https://rubyinstaller.org/downloads/
  * 맥북이라면 `brew` 로 설치해도 무관하다.
* `gem install jekyll bundler`
* 의존성 인스톨을 위해 로컬 위치에서 `bundle install` 실행

## 로컬 실행
* `bundle exec jekyll server`
* localhost:4000 에서 확인 가능하다.

## 반영하기
* 포스팅 등록 후 Commit 및 Push


## ETC
> 여기까지 설정이 완료되었다면 포스팅을 위해 많은 작업은 필요 없어 보인다.
> 테마에 특별한 욕심이 없다면 포스팅만 잘하면 된다.

### 도움될만한 링크
* [이미지 넣는 법](https://likelionsungguk.github.io/20-12-17/jekyll-Blog%EC%97%90-%ED%8F%AC%EC%8A%A4%ED%8C%85-%ED%95%98%EB%8A%94%EB%B2%95-%EC%9D%B4%EB%AF%B8%EC%A7%80%EB%84%A3%EA%B8%B0)