---
title: "Recent Reads"
layout: archive
permalink: /recent-reads/
entries_layout: list

articles:
  - ar-modeling-rq-vae:
    title: Autoregressive Image Generation using Residual Quantization
    image_path: /assets/images/Recent-Reads/Article-Page/ar-modeling-rq-vae.png
    desc: A paper that expands on the common methodology to compress high-dimensional datesets like embeddings into codebooks. They use this new technique called residual quantization which fixes the codebook's to a certain size and recursively quantizes the subsequent feature map in a coarse-to-fine manner.
    link: https://arxiv.org/pdf/2203.01941
  - audio-palm-paper:
    title: AudioPaLM - A Large Language Model That Can Speak and Listen
    image_path: /assets/images/Recent-Reads/Article-Page/audio-palm-paper.png
    desc: A cool paper I found out at random. But a very cool application of NLP to make a audio-audio model. From what I understand this is a foundational model for LLMs which can understand and generate speech. In terms of contemporary research this is a bit old (2023), but foundational nonetheless!
    link: https://arxiv.org/pdf/2306.12925
  - cdf-using-ad:
    title: Accelerating Particle and Fluid Simulations with Differentiable Graph Networks for Solving Forward and Inverse Problems
    image_path: /assets/images/Recent-Reads/Article-Page/cdf-using-ad.png
    desc: A very interesting paper on the applications of Automatic Differentiation outside the domain of machine learning. It is a bit of a hard read, specially for someone a little out of touch on the CDF community. Nevertheless, it is a great read!
    link: https://arxiv.org/pdf/2309.13348
  - autodiff-paper:
    title: Automatic Differentiation in Machine Learning - a Survey
    image_path: /assets/images/Recent-Reads/Article-Page/autodiff-cover.png
    desc: The paper explores the topic of Automatic/Algorithmic Differentiation (AD); an essential technology in contemporary machine learning models. It surveys a variety of methodologies to accomplish such concept and provides useful examples.
    link: https://arxiv.org/pdf/1502.05767
  - attention-paper:
    title: Attention is all you need.
    image_path: /assets/images/Recent-Reads/Article-Page/attention-cover.png
    desc: This revolutionary article pioneers the idea of Attention. One of the many algorithms utilized in the now renowned GPT LLMs OpenAI implements. Great read to understand how a transformer (the 'T' on 'GPT') functions.
    link: https://arxiv.org/pdf/1706.03762

books:
  - no-longer-human: 
    title: No Longer Human
    image_path: /assets/images/Recent-Reads/Book-covers/longer-human-cover.jpg
    desc: A total existential book from what I have heard. Still reading
    link: "https://www.amazon.com/No-Longer-Human-Osamu-Dazai/dp/0811204812"
  - poh: 
    title: Pursuit of Happiness
    image_path: /assets/images/Recent-Reads/Book-covers/poh-cover.jpg
    desc: A beautiful book about the search for happiness. Depicting a 'classic' rags to riches story of a single-dad broker into a enterpreneur. Discussions like family trauma and crisis are unforgettable. Must read!
    link: "https://www.amazon.com/Pursuit-Happyness-Chris-Gardner/dp/0060744871"

---

<center style="font-size: 18px">
Outside of coding, I enjoy a lot of reading. Fictional, non-fictional, technical, any book or article I think it looks interesting I read. This page is so I can share what cool document I have recently read. I will try my best to keep it as up-to-date as possible.
</center>

# Papers

{% for article in page.articles %}
  <div style="display: flex; margin: 10px 0; justify-content: space-between; padding: 10px;">
  <div style="max-width: 70%;">
    <h5>{{ article.title }}</h5>
    <div style="font-size: 14px">
      <p>{{ article.desc }}</p>
      <a href="{{ article.link }}" target="_blank" style="display: inline-block; padding: 10px 20px; background-color: #6c757d; color: white; text-decoration: none; border-radius: 5px;">Get</a>
    </div>
  </div>
  <div style="max-width: 25%; display: flex; align-items: center;">
    <a href="{{ article.link }}" target="_blank">
      <img src="{{article.image_path}}" alt="No image" style="max-width: 135px; max-height: 240px; border-radius: 8px;">
    </a>
  </div>
</div>
{% endfor %}

---

# Books

{% for book in page.books %}
  <div style="display: flex; margin: 10px 0; justify-content: space-between; padding: 10px;">
  <div style="max-width: 70%;">
    <h5>{{ book.title }}</h5>
    <div style="font-size: 14px">
      <p>{{ book.desc }}</p>
      <a href="{{ book.link }}" target="_blank" style="display: inline-block; padding: 10px 20px; background-color: #6c757d; color: white; text-decoration: none; border-radius: 5px;">Get</a>
    </div>
  </div>
  <div style="max-width: 25%; display: flex; align-items: center;">
    <a href="{{ book.link }}" target="_blank">
      <img src="{{book.image_path}}" alt="No image" style="max-width: 135px; max-height: 240px; border-radius: 8px;">
    </a>
  </div>
</div>
{% endfor %}

