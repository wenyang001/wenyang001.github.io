---
layout: about
title: 关于
permalink: /zh/
subtitle: >
  计算机视觉 · 多模态 AI · 工业视觉感知 ·
  <a href="https://www.ntu.edu.sg" target="_blank">南洋理工大学</a>
  <a class="lang-toggle" href="/">English</a>
contact_line: >
  <a class="contact-item" href="mailto:wenyang001@e.ntu.edu.sg"><i class="fa-solid fa-envelope" aria-hidden="true"></i><span>wenyang001@e.ntu.edu.sg</span></a>
  <span class="contact-item"><i class="fa-solid fa-location-dot" aria-hidden="true"></i><span>新加坡</span></span>
  <a class="contact-item" href="/assets/pdf/LIU_WENYANG_CV.pdf" target="_blank" rel="noopener noreferrer"><i class="fa-solid fa-file-pdf" aria-hidden="true"></i><span>CV</span></a>
  <a class="contact-item" href="https://www.linkedin.com/in/wenyangliu"><i class="fa-brands fa-linkedin-in" aria-hidden="true"></i><span>LinkedIn</span></a>
  <a class="contact-item" href="https://scholar.google.com/citations?user=gksRZlMAAAAJ"><i class="ai ai-google-scholar" aria-hidden="true"></i><span>Scholar</span></a>
nav: false
intro: |
  我目前在南洋理工大学 Hyundai–NTU–A*STAR Corporate Lab 担任 **Research Fellow**，与 [Assoc. Prof. Wai Kin (Adams) Kong](https://personal.ntu.edu.sg/AdamsKong/) 合作开展研究。当前研究聚焦面向工业感知的视觉基础模型、计算机视觉与多模态 AI，包括少样本/零样本异常检测、开放词汇检测与分割、6D 位姿估计和机器人抓取。

  在**重庆大学**获得硕士和学士学位后，我在**南洋理工大学**获得电气与电子工程博士学位，导师为 [Prof. Lap-Pui Chau](https://www.polyu.edu.hk/eee/people/academic-staff-and-teaching-staff/prof-chau-lap-pui/)（IEEE Fellow）和 [Assoc. Prof. Kim-Hui Yap](https://dr.ntu.edu.sg/entities/person/Yap-Kim-Hui)。博士研究围绕退化或不完整数据下的稳健视觉学习，涵盖受损媒体恢复、轻量化图像超分辨率和文件碎片理解，并为当前的工业与机器人感知研究奠定基础。我已发表 **21 篇论文**，获 **340+ 次引用**（h-index 8），包括四篇 CCF-A 第一作者论文。

research_tags:
  - 计算机视觉
  - 多模态 AI
  - 视觉语言模型
  - 视觉内容理解
  - 应用机器学习

project_experience_label: 科研项目
project_experience:
  - period: 2025年11月 – 至今
    title: 面向工业视觉感知的基础模型
    organization: Hyundai–NTU–A*STAR Corporate Lab
    output: ACM MM 2026 · 已申请专利
    current: true
  - period: 2025年6月 – 2025年11月
    title: 多模态人机交互
    organization: Schaeffler–NTU Corporate Lab · Phase III
    output: 3D 人体姿态重定向
  - period: 2024年12月 – 2025年6月
    title: 图像水印与多媒体安全
    organization: DSO National Laboratories, Singapore
    output: JVCIR 2025
  - period: 2024年3月 – 2024年12月
    title: 开放词汇工业视觉
    organization: Schaeffler–NTU Corporate Lab · Phase II
    output: EMNLP · ACM MM · KBS
  - period: 2021年1月 – 2024年3月
    title: 受损存储中的图像与视频恢复
    organization: 新加坡国家研究基金会（NRF）
    output: CVPR · NeurIPS · IEEE TMM
  - period: 2017年9月 – 2020年7月
    title: 高效视频处理与 AI 加速
    organization: 重庆大学
    output: ICPADS · DATE

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false

selected_papers: true
selected_papers_label: 精选论文
social: false

announcements:
  enabled: false
  scrollable: false

latest_posts:
  enabled: false
---

{% include about_home_style.html %}

<div class="section-label">最新消息</div>

<div class="zh-news-list">
  {% assign sorted_news = site.news | sort: "date" | reverse %}
  {% for item in sorted_news limit: 4 %}
  <p class="zh-news-item">
    <span class="zh-news-date">{{ item.date | date: "%Y年%-m月%-d日" }}</span>
    <span class="zh-news-text">
      {% if item.zh %}
        {{ item.zh | markdownify | remove: '<p>' | remove: '</p>' | strip }}
      {% else %}
        {{ item.content | strip_html | strip }}
      {% endif %}
    </span>
  </p>
  {% endfor %}
</div>
