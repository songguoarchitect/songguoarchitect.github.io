---
layout: page
title: Design
permalink: /design/
description: Paticipated design projects as main contributor; My own artworks
nav: true
nav_order: 4
---

## Architectural Projects

<div class="container">
  <div class="row">

    <!-- 示例 1｜图片缩略图 + Website 按钮 -->
    <div class="col-md-6 col-lg-4 mb-4">
      <div class="card shadow-sm">
        <a href="/assets/img/design/mccourt_thumb.jpg" target="_blank" rel="noopener">
          <img src="/assets/img/design/mccourt_thumb.jpg" class="card-img-top" alt="McCourt School of Public Policy">
        </a>
        <div class="card-body">
          <h5 class="card-title">McCourt School of Public Policy</h5>
          <p class="card-text">Georgetown University · RAMSA<br/>Conceptual Design</p>
          <a class="btn btn-sm btn-outline-primary" href="https://www.ramsa.com/projects/project/mccourt-school-public-policy" target="_blank" rel="noopener">Website</a>
        </div>
      </div>
    </div>

    <!-- 示例 2｜视频缩略图（mp4/webm，静音循环，点击可全屏）+ Website -->
    <div class="col-md-6 col-lg-4 mb-4">
        <div class="card shadow-sm">
            <div class="embed-responsive embed-responsive-16by9">
            <iframe
                class="embed-responsive-item"
                src="https://player.bilibili.com/player.html?bvid=BV1Y24y1P7KP&p=1&autoplay=0&high_quality=1&danmaku=0"
                title="Yuanbo Building video"
                allow="accelerometer; clipboard-write; encrypted-media; picture-in-picture; web-share"
                allowfullscreen
                loading="lazy">
            </iframe>
            </div>
            <div class="card-body">
            <h5 class="card-title">Yuanbo Building, BNU Zhuhai</h5>
            <p class="card-text">THAD · Landscape Design</p>
            <a class="btn btn-sm btn-outline-primary" href="https://www.archdaily.cn/cn/1025626/bei-jing-shi-fan-da-xue-zhu-hai-xiao-qu-yuan-bai-lou-qing-hua-da-xue-jian-zhu-she-ji-yan-jiu-yuan" target="_blank" rel="noopener">Website</a>
            </div>
        </div>
        </div>
    

    <!-- 示例 4｜视频缩略图（无控制条，悬停播放）-->
    <div class="col-md-6 col-lg-4 mb-4">
        <div class="card shadow-sm">
            <div class="embed-responsive embed-responsive-16by9">
            <video class="embed-responsive-item" muted loop playsinline controls
                    poster="/assets/img/design/southlake_lab_poster.jpg">
                <source src="https://www.dropbox.com/scl/fi/hr5h17z3yw9450kujkxn7/southlake_lab.mp4?rlkey=jewyf1mvrw1eoxwxy1t0ee5la&raw=1" type="video/mp4">
                <!-- 也可用 dl.dropboxusercontent.com 域名的直链 -->
                <!-- <source src="https://dl.dropboxusercontent.com/scl/fi/hr5h17z3yw9450kujkxn7/southlake_lab.mp4?rlkey=jewyf1mvrw1eoxwxy1t0ee5la" type="video/mp4"> -->
                Your browser does not support HTML5 video.
            </video>
            </div>
            <div class="card-body">
            <h5 class="card-title">South Lake Life Sciences Laboratory (Phase I)</h5>
            <p class="card-text">Jiaxing · THAD · Conceptual &amp; Landscape Design</p>
            <a class="btn btn-sm btn-outline-primary" href="http://www.archina.com/index.php?g=works&m=index&a=show&id=16325" target="_blank" rel="noopener">Website</a>
            </div>
        </div>
        </div>


    <!-- BUCM Library (Image only) -->
    <div class="col-md-6 col-lg-4 mb-4">
        <div class="card shadow-sm">
            <a href="/assets/img/design/bucm_library_large.jpg" target="_blank" rel="noopener">
            <img
                src="/assets/img/design/bucm_library_large.jpg"
                class="card-img-top"
                alt="Library of Beijing University of Chinese Medicine"
                loading="lazy"
                style="aspect-ratio:16/9; object-fit:cover;">
            </a>
            <div class="card-body">
                <h5 class="card-title">Library of Beijing University of Chinese Medicine</h5>
                <p class="card-text">THAD · Conceptual &amp; Schematic Design</p>
                <!-- <a class="btn btn-sm btn-outline-primary" href="#" target="_blank" rel="noopener">Website</a> -->
            </div>
        </div>
        </div>



    <!-- 示例 5｜图片缩略图 -->
    <div class="col-md-6 col-lg-4 mb-4">
      <div class="card shadow-sm">
        <a href="/assets/img/design/wenzhou_expo_large.jpg" target="_blank" rel="noopener">
          <img src="/assets/img/design/wenzhou_expo_large.jpg" class="card-img-top" alt="Wenzhou Garden Expo Park · Main Pavilion">
        </a>
        <div class="card-body">
          <h5 class="card-title">Wenzhou Garden Expo Park · Main Pavilion</h5>
          <p class="card-text">THAD · Competition</p>
          <!-- <a class="btn btn-sm btn-outline-primary" href="#" target="_blank" rel="noopener">Website</a> -->
        </div>
      </div>
    </div>

    <!-- 示例 6｜图片缩略图 -->
    <div class="col-md-6 col-lg-4 mb-4">
      <div class="card shadow-sm">
        <a href="/assets/img/design/jinan_stem_museum_large.jpg" target="_blank" rel="noopener">
          <img src="/assets/img/design/jinan_stem_museum_large.jpg" class="card-img-top" alt="Jinan Science & Technology Museum">
        </a>
        <div class="card-body">
          <h5 class="card-title">Jinan Science &amp; Technology Museum</h5>
          <p class="card-text">THAD · Competition — First Prize</p>
          <!-- <a class="btn btn-sm btn-outline-primary" href="#" target="_blank" rel="noopener">Website</a> -->
        </div>
      </div>
    </div>

  </div>
</div>

<!-- 可选：悬停自动播放/移出暂停（仅对 class="hover-play" 的视频生效） -->
<script>
  document.addEventListener('DOMContentLoaded', function () {
    var vids = document.querySelectorAll('video.hover-play');
    vids.forEach(function(v){
      v.addEventListener('mouseenter', function(){ v.play().catch(()=>{}); });
      v.addEventListener('mouseleave', function(){ v.pause(); });
      // 为了移动端初次静音自动播放（部分浏览器限制自动播放）
      v.addEventListener('canplay', function(){ if(v.muted){ v.play().catch(()=>{}); } }, {once:true});
    });
  });
</script>

<hr/>

## Artwork

<div class="container">
  <div class="row">

    <!-- Artwork 1 -->
    <div class="col-md-6 col-lg-4 mb-4">
      <div class="card shadow-sm">
        <a href="/assets/img/artwork/Character.jpg" target="_blank" rel="noopener">
          <img src="/assets/img/artwork/Character.jpg" class="card-img-top" alt="Stoneware Bowl">
        </a>
        <div class="card-body">
          <h5 class="card-title">Plate</h5>
          <p class="card-text mb-1"><strong>Medium:</strong> Ceramic (High-fire)</p>
          <p class="card-text mb-1"><strong>Year:</strong> 2023</p>
          <p class="card-text"><strong>Size:</strong> Ø 16 cm</p>
        </div>
      </div>
    </div>

    <!-- Artwork 2 -->
    <div class="col-md-6 col-lg-4 mb-4">
      <div class="card shadow-sm">
        <a href="/assets/img/artwork/cake.jpg" target="_blank" rel="noopener">
          <img src="/assets/img/artwork/cake.jpg" class="card-img-top" alt="Watercolor · Cityscape">
        </a>
        <div class="card-body">
          <h5 class="card-title">City After Rain</h5>
          <p class="card-text mb-1"><strong>Medium:</strong> Watercolor on paper</p>
          <p class="card-text mb-1"><strong>Year:</strong> 2020</p>
          <p class="card-text"><strong>Size:</strong> 26 × 18 cm</p>
        </div>
      </div>
    </div>

    <!-- Artwork 3 -->
    <div class="col-md-6 col-lg-4 mb-4">
      <div class="card shadow-sm">
        <a href="/assets/img/artwork/FreedomMorning.jpg" target="_blank" rel="noopener">
          <img src="/assets/img/artwork/FreedomMorning.jpg" class="card-img-top" alt="Photography · Bridge">
        </a>
        <div class="card-body">
          <h5 class="card-title">Morning Mist</h5>
          <p class="card-text mb-1"><strong>Medium:</strong> Photography (Digital)</p>
          <p class="card-text mb-1"><strong>Year:</strong> 2024</p>
          <p class="card-text"><strong>Size:</strong> 6000 × 4000 px</p>
        </div>
      </div>
    </div>

    <!-- Artwork 4 -->
    <div class="col-md-6 col-lg-4 mb-4">
      <div class="card shadow-sm">
        <a href="/assets/img/artwork/color.jpg" target="_blank" rel="noopener">
          <img src="/assets/img/artwork/color.jpg" class="card-img-top" alt="Porcelain Vase">
        </a>
        <div class="card-body">
          <h5 class="card-title">Porcelain Vase</h5>
          <p class="card-text mb-1"><strong>Medium:</strong> Porcelain (Blue & White)</p>
          <p class="card-text mb-1"><strong>Year:</strong> 2023</p>
          <p class="card-text"><strong>Size:</strong> Ø 5 × H 8 cm</p>
        </div>
      </div>
    </div>

    <!-- Artwork 5 -->
    <div class="col-md-6 col-lg-4 mb-4">
      <div class="card shadow-sm">
        <a href="/assets/img/artwork/courtyard.jpg" target="_blank" rel="noopener">
          <img src="/assets/img/artwork/courtyard.jpg" class="card-img-top" alt="Watercolor · Courtyard">
        </a>
        <div class="card-body">
          <h5 class="card-title">Quiet Courtyard</h5>
          <p class="card-text mb-1"><strong>Medium:</strong> Watercolor on paper</p>
          <p class="card-text mb-1"><strong>Year:</strong> 2020</p>
          <p class="card-text"><strong>Size:</strong> 29 × 21 cm</p>
        </div>
      </div>
    </div>

    <!-- Artwork 6 -->
    <div class="col-md-6 col-lg-4 mb-4">
      <div class="card shadow-sm">
        <a href="/assets/img/artwork/CapeAnn.jpg" target="_blank" rel="noopener">
          <img src="/assets/img/artwork/CapeAnn.jpg" class="card-img-top" alt="Photography · Night street">
        </a>
        <div class="card-body">
          <h5 class="card-title">Sailing</h5>
          <p class="card-text mb-1"><strong>Medium:</strong> Photography (Film)</p>
          <p class="card-text mb-1"><strong>Year:</strong> 2024</p>
          <p class="card-text"><strong>Location:</strong> Cape Ann, U.S. px</p>
        </div>
      </div>
    </div>

  </div>
</div>
