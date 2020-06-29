---
layout: post
title: Github를 이용한 블로그 만들기 No.3
category: github blog
---

이번 포스트에서는 jekyll 서버를 구성하는 폴더에 구조와 역할에 대해서 알아보려고 한다. 다른 프로젝트와 마찬가지로 jekyll도 프로젝트를 구성하는 구조가 존재한다.  jekyll 공식 홈페이지 에서 제공하는 기본적인 디렉토리 구조는 [여기](https://jekyllrb-ko.github.io/docs/structure/)에서 확인 할 수 있다.   

![사진](https://bearshub.github.io/assets/img/github/structfolder.png)


#### 1. _config.yml
_config.yml은 프로젝트의 설정 값들을 지정하는 파일로서, markdown의 종류 , url 주소, 사용하고 있는 plugin등 다양한 값들을 지정 할 수 있다. 

#### 2. _includes
html 또는 markdown 파일에서 공통적으로 사용하는 부분을 따로 분리 하여 _includes폴더에서 관리 할 수 있다. 작성자는 category와 sidebar, head 부분을 _includes 폴더에서 관리 하고 있다.  
_includes 폴더에 저장 되어 있는 html 파일들은  **Liquid 에서 제공하는 문법을 사용하여 ** ([Liquid 문법 참조](https://goodgid.github.io/What-is-Liquid-Grammer/)) 추가 할 수 있다. .  (html import와 유사한 형태)

#### 3. _layouts
_layouts 폴더에는 컨텐츠를 포함하는 화면 구조와 관련된 파일들이 포함되어 있다. layout의 file들은 화면의 성격이나 활용에 따라 달라질 것이고 includes 폴더에 있는 파일들로 구성될 수도 있다. 작성자는 post, page, category등과 같은 성격으로 분류하여 사용하고 있다. 

#### 4. _posts
_posts 폴더는 블로그 글을 저장하는 폴더이다. posts 폴더에 저장 할때는 파일 이름에 일정한 규칙이 있는데,  **년도-월-일-제목.md** 과 같은 형태를 따라야 한다. 파일명 형식이 맞지 않으면 블로그 리스트에서 글이 뜨지 않을 수 있다. 

#### 5. _site
markdown 도 궁극적으로 html 파일로 컴파일되는데, jekyll 에서 컴파일 된 파일이 저장되는 기본 경로 폴더이다. github을 사용할 때는 .gitignore 파일에 추가하여 git에 업로드를 할때 _site 폴더는 업로드가 되지 않게 사용하기도 한다. 

#### 6. Others 
이 밖에도 다양한 Floder와 file들이 존재하는 것 같다. 사실 굉장히 유연한 프레임워크 이기 떄문에 블로그를 운영하는 사람에 따라서도 구조가 달라질 수 있지만 어떤 테마를 받아서 적용하는지에 따라서도 조금씩 좌우 되는 것 같다. 























