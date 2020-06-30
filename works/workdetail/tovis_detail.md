---
layout: page
title: Project Tovis MES
---

<hr>
<div class="work_outer">
	<div class="swiper-container">
		<div class="swiper-wrapper">
		  <div class="swiper-slide"><img src="/assets/img/tovis/tovis_slide_1.png"></div>
		  <div class="swiper-slide"><img src="/assets/img/tovis/tovis_slide_2.png"></div>
		  <div class="swiper-slide"><img src="/assets/img/tovis/tovis_slide_3.png"></div>
		  <div class="swiper-slide"><img src="/assets/img/tovis/tovis_slide_4.png"></div>
		  <div class="swiper-slide"><img src="/assets/img/tovis/tovis_slide_5.png"></div>
		</div>
		<div class="swiper-button-next"></div>
		<div class="swiper-button-prev"></div>
	</div>
</div>

<!-- Swiper JS -->

<script src="/assets/scripts/swiper.min.js"></script>

<!-- Initialize Swiper -->
<script>
	var swiper = new Swiper('.swiper-container', {
    navigation: {
		nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
		},
    });
</script>


### TOVIS(Dairen) MES System  
Panel(Display)을 생산하는 MES (생산관리시스템) 으로써,  제조 업무 효율을 극대화 하여 이윤 추구를 목표로 한다.  처음부터 MES가 존재 하지 않았기 때문에 성공적인 도입과 안정적인 운영이 필요한 곳이었다. 

* 기준정보를 표준화 하여 통합 관리 할 수 있는 시스템
* 생산 및 품질을 실시간으로 모니터링 하고 관리 할 수 있는 시스템 
* 안정적이며 유연한 시스템 

### Project Issue
* Communicate with Equipment 
  * 설비와 통신이 필요한 부분이 있었는데, 소스 내에 설비와 통신하기 위한 Servlet을 추가로 생성하였고 Json을 통해서 성공적으로 통신 할 수 있었다.  (설비가 Json을 활용한 통신이 가능한지가 먼저 확인되어야 한다. )

* Factory Monitoring Board
  * 설비에서 올라오는 통신 상태 및 On/Off 신호 데이터를 이용하여 실시간으로 설비상태를 모니터링 할 수 있는 시스템을 개발하였다.  (위의 1번 슬라이드 이미지)

* Server Infra
  * WAS가 다운되는 현상이 자주 발견되어 (아마 설비 통신간의 과부화로 추정) Apache Tomcat 서버를 이중화 하여 분산처리 해야 하는 Issue가 발생하였다. 해당 내용은 블로그에 작성하여서 내용을 공유할 예정이다. 

### Project Structure
* UI Client
  * <i>HTML, Java Script, jqGrid and Highchart(Open Source)</i>
  
* Server and Framework
  * <i>Java, Spring Framework</i>
  
* DataBase
  * <i>Oracle 12c</i>
  
* Project Period
  * <i>2019.11 ~ 2020.03</i>

    
  
  
	




