---
layout: default
title: blog
---
<script src="/assets/scripts/toggle.js"></script>
<script src="/assets/scripts/scrollTop.js"></script>

<div class="page">
	
	<h2 id="categories"><a href="#example" class="toggle">Categories</a></h2>
	<span class="small_desc">Click here to see all categories</span>
	<div class="clearfix"></div>
		<div class="toggle-content" id="example">
			<!--
			<h3 class="category_name_link"><a href="{{site.baseurl}}about">jekyll</a></h3>
			<ul>
			  <li><a href="/jekyll/2018/07/28/introducing-hyde.html">Install Hyde theme on Jekyll version 3</a><span>28 Jul 2018</span></li>
			
			</ul>
			<h3 class="category_name_link"><a href="{{site.baseurl}}blog">web</a></h3>
			<ul>
			  <li><a href="/web/2018/08/23/optimize-site-speed.html">Optimize site speed</a><span>23 Aug 2018</span></li>
			  <li><a href="/web/2018/08/19/deploy-site-on-netlify.html">Deploy a photography portfolio site on Netlify</a><span>19 Aug 2018</span></li>
			  <li><a href="/web/2018/08/06/using-webpack-for-fullstack-app.html">Using webpack for fullstack app</a><span>06 Aug 2018</span></li>
			</ul>
			-->
			
			<!--
			{% for post in site.categories %}
				<h3 class="category_name_link">
					<a href="{{ categories.url }}">
					</a>
				</h3>
			{% endfor %}
			-->
			
			
			
		</div>
	<hr>

	<div class="posts">
	  {% for post in site.posts %}
	  <div class="post">
		<h1 class="post-title">
		  <a href="{{ post.url }}">
			{{ post.title }}
		  </a>
		</h1>

		<span class="post-date">{{ post.date | date_to_string }}</span>
		{{ post.content }}
	  </div>
	  {% endfor %}
	</div>
	
	<!--
	<div class="pagination">
	  {% if paginator.next_page %}
		<a class="pagination-item older" href="{{ site.baseurl }}page{{paginator.next_page}}">Older</a>
	  {% else %}
		<span class="pagination-item older">Older</span>
	  {% endif %}
	  {% if paginator.previous_page %}
		{% if paginator.page == 2 %}
		  <a class="pagination-item newer" href="{{ site.baseurl }}">Newer</a>
		{% else %}
		  <a class="pagination-item newer" href="{{ site.baseurl }}page{{paginator.previous_page}}">Newer</a>
		{% endif %}
	  {% else %}
		<span class="pagination-item newer">Newer</span>
	  {% endif %}
	</div>
	-->
	<a id="back_to_top" onclick="scrollToTop(700)"><i class="icon-up-open"></i></a>
</div>