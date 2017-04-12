---
layout: post
title: vim의 color schemes와 설정 방법
date: 2016-04-12
excerpt: "Vim의 Color scheme 초기 vim에서의 코딩은..."
tags: [vim, vimrc, Color_scheme, How to]
comments: true
---

## Vim의 Color scheme

초기 vim에서의 코딩은 별로 유쾌하지가 않습니다. 가독성이 떨어지기 때문이죠. 소스에 색깔을 입히면 보기도 편하고 이해하기가 쉽습니다. vim에는 여러 Color scheme들이 있지만 어떤 Color scheme를 선택하는지는 개개인의 취향입니다.

 어떤 Color scheme를 사용할지 고민하다가 구글링을 통해 선택에 도움을 주는 <a href="http://www.vimninjas.com/2012/08/26/10-vim-color-schemes-you-need-to-own/">사이트</a>를 찾았습니다. 많이 사용되는 10가지의 Vim Color schemes에 대해 요약해둔 사이트입니다. 웹 프로그래밍을 하신다면 Guardian이나 Distinguished 테마를 추천합니다.
 
### Color scheme 적용 방법
 보통 vim에 관한 설정파일은 `/usr/share/vim/vim7*`에 들어 있습니다. (제 경우엔 vim이 74버전이라 `/usr/share/vim/vim74`라는 파일에 있습니다.) 해당 경로에 여러 디렉토리들이 있지만 Color scheme에 관한 설정이므로 `/usr/share/vim/vim7*/colors`라는 디렉토리로 들어가 다운받은 컬러스키마를 저장합니다.

 이후 최상위 디렉토리에서 `.vimrc`파일을 편집하여 하위디렉토리에도 적용하게 합니다.(없으신 분들은 생성해도 됩니다.) 적용방법은 편집기를 통해 `.vimrc`를 열어 아래의 코드를 삽입합니다.
{% raw %}
	colorscheme 'colorscheme이름'
    

터미널을 종료하고 다시 시작하면 아래와 같이 Color scheme이 적용되는 모습을 확인 할 수 있습니다.

<img src="https://nine-hundred.github.io/Blog/assets/vimColorScheme.jpg">

