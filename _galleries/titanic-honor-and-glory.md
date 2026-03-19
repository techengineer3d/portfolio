---
enabled: true
heading:
name: Titanic Honor and Glory
title: Titanic Honor and Glory 
subtitle: RebrightFX Sample
image_path: /images/galleries/rebrightfx/games/titanic-hg/cover/rebrightfx-images/1440p/2026-03-18/titanic-title-screen-01-02-RC1-2026-03-18-RebrightFX-UHD-Dynamic-Sharp-Luma-Bright-04-Chroma-Vibrant.jpg
importance: 1
category: games
related_publications: true
gallery_root_: /images/galleries
before_folder: /original-images
after_folder: /rebrightfx-images
image_size_folder: /1440p
thumbnails_folder: /thumbnails
publish_date_folder: /2026-03-18
banner_folder: /banner
cover_folder: /cover
feature_folder: /feature
gallery:
  name: rebrightfx
  category: games
  album: titanic-hg
  main_folder: /images/galleries/rebrightfx/games/titanic-hg
  subfolders: [/first-class-ii]
  enable_separate_galleries: false
  cover:
    image: 
      before: /cover/original-images/1440p/titanic-title-screen-01-01-original.jpg
      after: /cover/rebrightfx-images/1440p/2026-03-18/titanic-title-screen-01-02-RC1-2026-03-18-RebrightFX-UHD-Dynamic-Sharp-Luma-Bright-04-Chroma-Vibrant.jpg
    folder: 
      before: /cover/original-images/1440p
      after: /cover/rebrightfx-images/1440p/2026-03-18
  banner:
    image: 
      before: 
      after: 
    folder: 
      before: /banner/original-images/1440p
      after: /banner/rebrightfx-images/1440p/2026-03-18
  feature:
    image:
      before: /feature/original-images/1440p/titanic-first-class-ii-09-01-original.jpg
      after: /feature/rebrightfx-images/1440p/2026-03-18/titanic-first-class-ii-09-02-rc1-2026-03-18-rebrightfx-uhd-dynamic-sharp-luma-bright-04-chroma-vibrant.jpg
    folder: 
      before: /feature/original-images/1440p
      after: /feature/rebrightfx-images/1440p/2026-03-18

author_staff_member: techengineer3d

id: titanic-hg

images:
  photoswipe: false
  swiperjs: false
  img-compare: true
  twentytwenty: false
  lightbox2: false
  fancybox: false
  fancyapps: true
---

{% comment %}
BANNER IMAGE: display banner image if available
{% endcomment %}

{% if page.gallery.banner.image.after %}{% assign banner_image = page.gallery.banner.image.after %}
{% elsif page.gallery.banner.image.before %}{% assign banner_image = page.gallery.banner.image.before %}
{% endif %}
{% if banner_image %}
![]({{site.baseurl}}{{page.gallery.main_folder}}{{banner_image}})
{% endif %}

<!-- image lighting, shadow and color intensity of rebrightfx image displays slightly differently when using the ImgComparisonSlider
<div>
<img-comparison-slider id=myImgComparisonSlider>
  <figure slot="first" class="before">
    <img width="100%" src="{{site.baseurl}}{{page.gallery.main_folder}}{{page.gallery.banner.image.before}}">
    <figcaption>Original</figcaption>
  </figure>
  <figure slot="second" class="after">
    <img width="100%" src="{{site.baseurl}}{{page.gallery.main_folder}}{{page.gallery.banner.image.after}}">
    <figcaption>RebrightFX</figcaption>
  </figure>
</img-comparison-slider>
</div>
-->

<br/>

## {{page.title}}

{% comment %}
FEATURE IMAGE: display before/after feature image if available
{% endcomment %}

{% if page.gallery.feature.image.after %}
{% assign feature_image_after = page.gallery.feature.image.after %}
{% endif %}
{% if page.gallery.feature.image.before %}
{% assign feature_image_before = page.gallery.feature.image.before %}
{% endif %}
{% if feature_image_before and feature_image_after %}
### Feature Image

<div>
<img-comparison-slider id=myImgComparisonSlider>
  <figure slot="first" class="before">
    <img width="100%" src="{{site.baseurl}}{{page.gallery.main_folder}}{{feature_image_before}}">
    <figcaption>Original</figcaption>
  </figure>
  <figure slot="second" class="after">
    <img width="100%" src="{{site.baseurl}}{{page.gallery.main_folder}}{{feature_image_after}}">
    <figcaption>RebrightFX</figcaption>
  </figure>
</img-comparison-slider>
</div>

<br/>
{% endif %} <!--if before and after feature images -->

{% comment %}
GALLERY IMAGES: display before/after gallery images if available
{% endcomment %}

<!-- automatic gallery image file loader -->
{% assign beforeFolder = page.before_folder %}
{% assign afterFolder = page.after_folder %}
{% assign imageSizeFolder = page.image_size_folder %}
{% assign publishDateFolder = page.publish_date_folder %}
{% assign galleryFolder = page.gallery.main_folder %}
{% assign subFolderList = page.gallery.subfolders %}

{% assign __empty_array = '' | split: ',' %}
{% assign all_files = __empty_array %}

{% assign all_images = site.static_files | where: "image", true %}

{% comment %}
GALLERY MAIN FOLDER: load gallery images from main folder
{% endcomment%}

{% assign beforeFolderPath = galleryFolder %}
{% assign beforeFolderPath = beforeFolderPath | append: beforeFolder %}
{% assign beforeFolderPath = beforeFolderPath | append: imageSizeFolder %}

{% assign afterFolderPath = galleryFolder %}
{% assign afterFolderPath = afterFolderPath | append: afterFolder %}
{% assign afterFolderPath = afterFolderPath | append: imageSizeFolder %}
{% assign afterFolderPath = afterFolderPath | append: publishDateFolder %}

{% assign beforeImages = site.static_files | where_exp: "item", "item.path contains beforeFolderPath" %}
{% assign afterImages = site.static_files | where_exp: "item", "item.path contains afterFolderPath" %}    
{% assign all_files = all_files | concat: beforeImages %}
{% assign all_files = all_files | concat: afterImages %}

{% comment %}
GALLERY SUBFOLDERS: load gallery images from specified subfolders
{% endcomment%}

{% for subfolder in subFolderList %}

  {% assign beforeFolderPath = galleryFolder %}
  {% assign beforeFolderPath = beforeFolderPath | append: subfolder %}
  {% assign beforeFolderPath = beforeFolderPath | append: beforeFolder %}
  {% assign beforeFolderPath = beforeFolderPath | append: imageSizeFolder %}

  {% assign afterFolderPath = galleryFolder %}
  {% assign afterFolderPath = afterFolderPath | append: subfolder %}
  {% assign afterFolderPath = afterFolderPath | append: afterFolder %}
  {% assign afterFolderPath = afterFolderPath | append: imageSizeFolder %}
  {% assign afterFolderPath = afterFolderPath | append: publishDateFolder %}
  
  {% comment %}
  {% assign beforeImages = __empty_array %}
  {% assign afterImages = __empty_array %}
  start image loop search<br/>
  {% for image in all_images %}
    {% if image.path contains beforeFolderPath %}
    {% assign beforeImages = beforeImages | push: image %}
    {% endif %}
    {% if image.path contains afterFolderPath %}
    {% assign afterImages = afterImages | push: image %}
    {% endif %}
  {% endfor %}
 end image loop search<br/>
 {% endcomment %}
  
  {% assign beforeImages = site.static_files | where_exp: "item", "item.path contains beforeFolderPath" %}
  {% assign afterImages = site.static_files | where_exp: "item", "item.path contains afterFolderPath" %}
    
  {% assign all_files = all_files | concat: beforeImages %}
  {% assign all_files = all_files | concat: afterImages %}
  
{% endfor %} <!--for subfolder in subfolderlist-->

{% if all_files %}

### Gallery Slider

<span class="font-weight-bold">
Images are best viewed full screen in order to clearly see the enhanced ultra high definition details.<br/>
Click on the image preview window below to switch to the larger image viewer.<br/>
Then use the toolbar to toggle full screen mode, hide the thumbnails, and start a slideshow.<br/>
</span>

{% assign sorted_files = all_files | sort: 'name' %}

<div class="f-carousel" id="fancyCarousel2">
  <div class="f-carousel__viewport">
{% for file in sorted_files %}
  {% if file.extname == '.jpg' %}
    <div
    class="f-carousel__slide"
    data-fancybox="ff7"
    data-src="{{ site.baseurl }}/{{ file.path }}"
    data-thumb-src="{{ site.baseurl }}/{{ file.path }}"
    >
    <img
        data-lazy-src="{{ site.baseurl }}/{{ file.path }}"
        width="100%"
        height="100%"
        alt="Original"
    />
    </div>
  {% endif %}
{% endfor %}
  </div>
</div>

<br/>

{% endif %} <!--if all_files-->



