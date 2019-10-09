---
layout: post
title: 'GitHub Page 만들기'
date: 2019-10-09 11:00
categories: blog
---



# GitHub Page 만들기
깃허브에서 블로그 페이지를 제공한다.

깃허브는 소스관리 도구이다. 개발자들에게 필요한 도구다. 개발을 하면 소스를 복사해서 붙여넣는 기능을 많이 사용한다. 직접 키보드로 타이핑하는 것보다 동작하고 있는 코드를 복사해서 붙여 넣는 방법을 좋아한다. 문서를 작성할 때도 원본 내용을 복사해서 사용할 수 있는 일반 에디터를 좋아한다. 에버노트가 인기있던 이유이기도 하다.

몇가지 장점이 있다.
* 깃허브의 레포지터리를 이용한다. - {username}.github.io
* markdown(.md) 파일을 _posts에 올리면 블로그에 보여준다.

물론 불편한 점도 있다. 
* 문서의 원본파일이 그대로 공개된다. - 블로그 파일 전체를 복사해서 가져올 수 있다.(깃허브의 장점이긴 하다)
* 깃허브 사이트를 이용할 수도 있으나 일반적으로 git 을 사용해야 한다. - 일반 블로그보다 어렵다
* markdown 파일로 작성하므로 문서 디자인에 한계가 있다.

알아야할 내용
* GitHub Pages
* Jekyll - ruby, wsl(windows 10)
* Markdown

작성 순서
* GitHub Page 설정 - https://pages.github.com/
  - {username}.github.io 레로지토리 생성
  - public repository
  - GitHub Page로 지정 - master branch
  - index.html 파일을 올려서 동작 확인
* jekyll-new 레포지토리 복사(클론)
  - _config.yml 수정
* Jekyll Theme 적용 - https://help.github.com/en/articles/setting-up-a-github-pages-site-with-jekyll
  - [질문] local 컴퓨터에 jekyll을 설치해야 하는 것인가? 설치하거나 설치된 레포지토리를 클론해야 함.
  - jekyll new로 생성되는 블로그를 레포지토리에 등록했음.

추가 정보
* 윈도우에 jekyll 설치하기
  - jekyll을 설치하려면 ruby가 필요한데 윈도우즈는 공식적으로 지원하지 않음. rubyinstaller 이용하거나 WSL을 이용
  - rubyinstaller 이용
  - windows 10에서 지원하는 wsl 이용 - 개발자라면 - https://docs.microsoft.com/ko-kr/windows/wsl/wsl2-install
    - powershell 명령어 실행 - 관리자모드, 재부팅
    - wsl ubuntu 설치
    - wsl 2로 업그레이드 하려고 했으나 현재 지원 안함 - insider에서 지원 
  - windows 10 wsl에서 설치(jekyll home) - https://jekyllrb.com/docs/installation/windows/#installation-via-bash-on-windows-10
    - ruby2.5와 ruby2.5-dev 설치 - 현재 2.6까지 나와있음
  - windows 10 wsl에서 설치(rvm 이용) https://scottdorman.blog/2019/02/27/running-jekyll-on-wsl/ 
    - rvm 설치 -> ruby 설치(2.6.3)