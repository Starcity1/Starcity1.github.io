---
title: "About me!"
layout: splash
permalink: /about/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/About/header-img.jpeg
  caption: "A Happy Moment. Photo credit: [**Martin Marek**](https://www.instagram.com/martin174115/)"
excerpt:
    "<p style='fontsize: 20px; color:white;width:50%;'>Please be a traveler, not a tourist. Try new things, meet new people, and look beyond what's right in front of you. Those are the keys to understanding this amazing world we live in.</p>
    <br/>
    - Andrew Zimmerman"
intro: 
  - excerpt: 'I am not too much of someone who really likes sharing *everything* about themselves. But it is the minimum I can do to you, dear reader. As I believe it is important to know a bit about the author whilst reading some of their content.'
feature_row:
  - image_path: assets/images/about/family.jpg
    alt: "Family"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: /assets/images/About/me.jpeg
    alt: "Me as an Aggie"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: assets/images/about/friends.jpg
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
feature_row2:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Left Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row3:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Right Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row4:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row layout="center" caption="test"%}

{% include feature_row id="feature_row2" type="left" %}

{% include feature_row id="feature_row3" type="right" %}

{% include feature_row id="feature_row4" type="center" %}