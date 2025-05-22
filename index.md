---
title: Home
layout: default
---
<!--banner-->
<div class="card bg-dark border-0 text-white custom-radius-3">
  <img src="{{ '/Images/banner.jpg' | relative_url }}" class="card-img" alt="Anathema-banner">
  <div class="card-img-overlay pl-5 d-flex align-items-center">
    <div>
      <img class="deco-logo" width="60%" src="./Images/Anathema-Vector.svg">
      <h3 class="card-title fweight-ligth">The Ultimate Guide</h3>
      <p class="card-text">Here you can find all the information about the band, their music and more</p>
      <a href="#"><p class="button-custom-dark card-text">Anathema Discography <i class="fa-solid fa-chevron-right"></i></p></a>
    </div>
  </div>
</div>
<!--cards-->
<div class="row mt-4">
<div class="col-sm mx-width50 p-2">
  <a class="text-white" href="#">
    <div class="card bg-dark border-0 text-white custom-radius-2">
      <img src="{{ '/Images/discography.jpg' | relative_url }}" class="card-img" alt="">
      <div class="card-img-overlay px-2 d-flex align-items-end justify-content-center black-hover">
        <p class="font-weight-bold card-text">Discography</p>
      </div>
    </div>
  </a>
</div>
<div class="col-sm mx-width50 p-2">
  <a class="text-white" href="#">
    <div class="card bg-dark border-0 text-white custom-radius-2">
      <img src="{{ '/Images/albums.jpg' | relative_url }}" class="card-img" alt="">
      <div class="card-img-overlay px-2 d-flex align-items-end justify-content-center black-hover">
        <p class="font-weight-bold card-text">Albums</p>
      </div>
    </div>
  </a>
</div>
<div class="col-sm mx-width50 p-2">
  <a class="text-white" href="#">
    <div class="card bg-dark border-0 text-white custom-radius-2">
      <img src="{{ '/Images/oldTracks.jpg' | relative_url }}" class="card-img" alt="">
      <div class="card-img-overlay px-2 d-flex align-items-end justify-content-center black-hover">
        <p class="font-weight-bold card-text">Old Songs</p>
      </div>
    </div>
  </a>
</div>
<div class="col-sm mx-width50 p-2">
  <a class="text-white" href="#">
    <div class="card bg-dark border-0 text-white custom-radius-2">
      <img src="{{ '/Images/WS.jpg' | relative_url }}" class="card-img" alt="">
      <div class="card-img-overlay px-2 d-flex align-items-end justify-content-center black-hover">
        <p class="font-weight-bold card-text">Weather Systems</p>
      </div>
    </div>
  </a>
</div>       
</div>
<!--buttom jekyll info-->
<div>
  <h1>{{ page.title }}</h1>
  <p><strong>Released:</strong> {{ page.year }}</p>
  <div>
    {{ content }} 
    <ul>
    {% for album in site.albums %}
    <li><a href="{{ site.baseurl }}{{ album.url }}">{{ album.title }}</a> ({{ album.year }})</li>
    {% endfor %}
    </ul>
  </div>
</div>