---
title: "Recent Reads"
layout: archive
permalink: /recent-reads/
entries_layout: list

articles:
  - vibe_coding:
    title: Not all AI-assisted programming is vibe coding (but vibe coding rocks).
    image_path: /assets/images/Recent-Reads/Article-Page/vibe-coding.png
    desc: A really cool article that perfectly aligns with my views on the current misuse of AI tools for software development. It portrays how misusing tools such as ChatGPT, Claude, Gemini and other LLMs for coding can hinder the development process of a project. If anything, I believe that this article misses on another important aspect for young SWEs who are starting their career paths like me - the learning aspect.
    link: https://simonwillison.net/2025/Mar/19/vibe-coding/
  - google_map_reduce:
    title: Map Reduce - Simplified Data Processing on Large Clusters
    image_path: /assets/images/Recent-Reads/Article-Page/google_map_reduce.png
    desc: Map Reduce is Google's approach on big data processing and within Google's technological context. Within this context, fault-tolerance over commodity machinery was a priority. Therefore, MapReduce is great for data processing over a distributed cluster. Great read for a real-life application of distributed system concepts such as quorum, synchronization, etc.
    link: https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf
  - google_gfs:
    title: The Google File System
    image_path: /assets/images/Recent-Reads/Article-Page/google_gfs.png
    desc: An approach on one of the more complex topic on distribution systems - distributed file systems (DFS). The discussion in this paper is Google's approach on creating a DFS which hundreds of users could access at the same time. GFS uses an advanced lock service Google first developed known as Chubby. Great paper to better understand how DFS function.
    link: https://static.googleusercontent.com/media/research.google.com/en//archive/gfs-sosp2003.pdf
  - google_bigtable:
    title: Bigtable - A Distributed Storage System for Structured Data
    image_path: /assets/images/Recent-Reads/Article-Page/google_bigtable.png
    desc: Bigtable is Google's attempt on a distributed storage system which is highly reliable, scalable, and available. With a very unique approach and schema on mapping structured data. In addition, Google uses its own environment and technologies such as GFS, Chubby and others to be able to create Bigtable's schema. A great read to get involved into Distributed Systems.
    link: https://static.googleusercontent.com/media/research.google.com/en//archive/bigtable-osdi06.pdf
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
  - dist-systems-textbook:
    title: Distributed Systems
    image_path: /assets/images/Recent-Reads/Book-covers/Distributed_Systems.png
    desc: A great introductory book into the highly complex world of distributed systems. The textbook describes into high detail all the building blocks on creating a highly reliable, scalable, and fault-tolerant distributed system.
    link: https://www.amazon.com/Distributed-Systems-Maarten-van-Steen/dp/1543057381
  - no-longer-human: 
    title: No Longer Human
    image_path: /assets/images/Recent-Reads/Book-covers/longer-human-cover.jpg
    desc: A total existentialist book who follows the live of a person who never felt to really fit or understand human thoughts and actions. Providing a very unique perspective on how society functions.
    link: "https://www.amazon.com/No-Longer-Human-Osamu-Dazai/dp/0811204812"
  - poh: 
    title: Pursuit of Happiness
    image_path: /assets/images/Recent-Reads/Book-covers/poh-cover.jpg
    desc: A beautiful book about the search for happiness. Depicting a 'classic' rags to riches story of a single-dad broker into a enterpreneur. Discussions like family trauma and crisis are unforgettable. Must read!
    link: "https://www.amazon.com/Pursuit-Happyness-Chris-Gardner/dp/0060744871"

---

<center style="font-size: 18px">
Outside of coding, I enjoy a lot of reading. Fictional, non-fictional, technical, any book or article I think it looks interesting I read. This page is so I can share what cool papers I have recently read. I will try my best to keep it as up-to-date as possible.
</center>

{% assign max_items = 10 %}
{% assign articles_to_display = page.articles | slice: 0, max_items %}
{% assign books_to_display = page.books | slice: 0, max_items %}

# Papers

{% for article in articles_to_display %}
  <div style="display: flex; margin: 10px 0; justify-content: space-between; padding: 10px;">
  <div style="max-width: 70%;">
    <h5>{{ article.title }}</h5>
    <div style="font-size: 14px">
      <p>{{ article.desc }}</p>
      <a href="{{ article.link }}" target="_blank" style="display: inline-block; padding: 10px 20px; background-color: #6c757d; color: white; text-decoration: none; border-radius: 5px;">Read</a>
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

{% for book in books_to_display %}
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

