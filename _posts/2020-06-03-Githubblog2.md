---
layout: post
title: Github를 이용한 블로그 만들기 No.2
category: github blog
---

지난 포스트는 Github의 Repository 생성부터 jekyll server를 설치하고 구동 시켜보는 것 까지 진행 했었다. 이번 포스트는 jekyll theme를 적용하는 것을 다루어 보려고 한다.  jekyll은  특색있는 테마들로 블로그를 꾸밀 수 있는데, 대부분 무료로 사용할 수 있는 테마들이 많이 있다.  필자는 jekyll의 많은 블로그 테마 중 [hyde](https://github.com/poole/hyde) 테마를 적용하였고 이를 적용한 방법을 기록 하려고 한다.  
~~jekyll 엔 hyde가 딱이야 !~~ 



**jekeyll theme 관련 사이트**

* [jekyllthemes.org](http://jekyllthemes.org/)
* [Free Jekyll Themes](https://jekyllthemes.io/free)

테마를 고르는데 몇 가지 팁이 있다면 가장 먼저 모바일 기기를 지원하는지 확인 하는 것이고 사이드바가 존재하는지 확인 하는 것이다.   사이드바가 없는 테마도 추가를 할 수 있지만 작업을 하다보면 정신건강에 해로울 수 있다. 



### 1. hyde 테마 Download

* [hyde Github](https://github.com/poole/hyde) 에서 Clone
* [hyde Demo](https://hyde.getpoole.com/) 에서 Download를 클릭해서 zip 파일을 다운로드 
위의 두 가지중 편한 것을 진행하여 앞서 만들었던 id.github.io 폴더에 저장한다. 

![사진](https://bearshub.github.io/assets/img/github/github_blog_6.png) 





### 2. _config.yml 파일 수정 

+ Markdown Dependancy 수정 

  + Github Page가 2019년 5월 부터 Markdown 형식을 ```kramdown``` 만 지원하는 것으로 정했다. 그래서 기존에 사용하던 ```redcarpet``` 방식에서 ```kramdown``` 으로 변경 해줘야 한다.  

+ relative_permalinks 삭제
  
+ relative_permalinks : true 라고 되어 있는 항목을 삭제 한다. 
  
+ Plug in 설치 및  추가
  + jekyll -paginate 와 jekyll-gist 를 설치 해준다.  (gem list 명령어로 설치 확인)
	```jekyll
	$ gem install jekyll-gist
	$ gem install jekyll-paginate
	```
  + 이 부분을 _config.yml 마지막 부분에 추가 해 준다. 
	```
	plugins:
	- jekyll-paginate
	- jekyll-gist
	```
  + Kramdown은 기존에 설치가 됐던 것으로 기억한다. 혹시라도 없으면 설치해 주시라.. 
  
+ jekyll 테마마다 필요한 plugin이나 방법들이 다소 다를 수 있으니 주의 ! 

  

### 3. Jekyll 구동
```jekyll
$ jekyll serve 
```

서버가 뜨는것을 확인 하고 [localhost:4000](http://localhost:4000)으로 접속하면 hyde 테마가 적용된 표준 페이지가 출력될 것이다!  

hyde 테마의 페이지가 출력된 것을 확인 했다면 이제 원하는대로 커스터이징을 진행 하면 된다.


다음 포스트에는 _include와 _layout등의 폴더 구조에 대해 다뤄 볼 예정이다. 



























































