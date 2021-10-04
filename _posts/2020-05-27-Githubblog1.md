---
layout: post
title: Github를 이용한 블로그 만들기 No.1
category: github blog
---

### 1. Github Repository 생성

가장 먼저  [Github](https://github.com/)에 회원가입을 하고 ID를 생성한다.  
본인이 원하는 ID와 이름, 이메일정보 등을 사용하여 회원가입을 한 후 Repository를 생성한다.   



* New Repository 버튼을 클릭 하면 Repository를 생성하는 페이지로 이동한다.   

![사진](https://bearshub.github.io/assets/img/github/github_blog_1.png)  

  



* Repository name에 본인의 ID.github.io를 입력하여 생성한다.  이  주소가 곧  블로그의  메인 url이 된다. 작성자는  ***Initialize this repository with a README*** 를 체크 한 후에 진행했다.  생성 후에는 url (yourId.github.io)로 접속하여 확인 할 수 있다.   

![사진](https://bearshub.github.io/assets/img/github/github_blog_2.png)  



### 2. Repository Local 저장

생성된 Github의 Repository를 local에 복사 한다. 후에 [Jekyll](https://jekyllrb.com/) 을 이용해서 Local에 Server를 띄우고 작업할 수 있으며, Local에서 작업한 내용을 github에 commit / push 하여 변경이나 추가된 내용을 반영 할 수 있다.   



* Clone or download 버튼을 클릭할때 나오는 url을 복사한다. 

![사진](https://bearshub.github.io/assets/img/github/github_blog_3.png)  




* Repository로 사용하고 싶은 폴더에 들어가서 *shift + 우클릭 ->  '여기에 Powershell 창 열기'* 를 선택하여 커맨드 창을 실행 할 수 있다.   

```github
git clone targetURL
```
위의 명령어를 사용하여 폴더에 Repository가 생성된 것을 확인 할 수 있다. 

![사진](https://bearshub.github.io/assets/img/github/github_blog_5.png)  



### 3. Ruby 설치 

갑자기 Ruby?? 라고 할 수 있지만 Local에서 jekyll을 설치하고 실행하기 위해서는 가장 먼저 Ruby 설치가 필요하다.  jekyll을 설치하면서 'gem' 으로 시작하는 명령어를 사용할 텐데,  그 명령어가 바로 ruby 기반에서 동작 한다.  (ruby의 라이브러리다.)  
[ruby Installer(for windows)](https://rubyinstaller.org/downloads/ ) 를 통해서 다운로드 받을 수 있다.  [(설치 참조 URL)](https://itbellstone.tistory.com/43)  



### 4. jekyll 설치

```ruby
$ gem install jekyll
```

일단 위의 명령어를 입력하는 것 외에 jekyll을 설치하기 위해서 따로 진행 할 것은 없다. jekyll은 정적 웹사이트를 생성해주는 툴이고 그렇기 때문에 간단한 HTML과 CSS 등으로 사이트를 생성하고 운영할 수 있다. 그리고 빠르고 , 가볍다.   
설치한 jekyll server를 테스트 하기 위해서는  아래와 같은 명령어로 확인 할 수 있다. 



```ruby
$ jekyll new myblog
$ cd new myblog
$ jekeyll serve
```



정상적으로 설치 후  http://localhost:4000 으로 접속한다면 아래 그림과 같은 페이지를 확인 할 수 있다. 

![사진](https://bearshub.github.io/assets/img/github/github_blog_4.png)



다음 포스트에서는 [hyde](https://github.com/poole/hyde) 테마를 이용해서 블로그를 생성하는 것을 다루어 보도록 하겠다. 



















































































