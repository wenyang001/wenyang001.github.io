---
layout: about
title: 关于
permalink: /zh/
subtitle: >
  计算机视觉 · 多模态 AI · 工业视觉感知 ·
  <a href="https://www.ntu.edu.sg" target="_blank">南洋理工大学</a>
  <a class="lang-toggle" href="/">English</a>
contact_line: >
  <a href="mailto:wenyang001@e.ntu.edu.sg">wenyang001@e.ntu.edu.sg</a> · 新加坡 ·
  <a href="/cv/">CV</a> ·
  <a href="https://www.linkedin.com/in/wenyangliu">LinkedIn</a> ·
  <a href="https://scholar.google.com/citations?user=gksRZlMAAAAJ">Scholar</a>
nav: false

intro: |
  我目前在南洋理工大学 Hyundai–NTU–A*STAR Corporate Lab 担任 **Research Fellow**，与 [Assoc. Prof. Wai Kin (Adams) Kong](https://personal.ntu.edu.sg/AdamsKong/) 合作开展研究。我围绕视觉基础模型、计算机视觉与多模态 AI，研究视觉内容理解和工业场景感知；目前在 HMGICS 开展少样本/零样本异常检测、开放词汇检测与分割、6D 位姿估计和机器人抓取研究。

  我在南洋理工大学获得电气与电子工程博士学位，导师为 [Prof. Lap-Pui Chau](https://www.polyu.edu.hk/eee/people/academic-staff-and-teaching-staff/prof-chau-lap-pui/)（IEEE Fellow）和 [Assoc. Prof. Kim-Hui Yap](https://dr.ntu.edu.sg/entities/person/Yap-Kim-Hui)。博士研究聚焦损坏媒体恢复、轻量化图像超分辨率和文件碎片理解。我已发表 **21 篇论文**，获 **340+ 次引用**（h-index 8），包括四篇 CCF-A 第一作者论文，并申请一项工业视觉专利；同时担任 CVPR、ICCV、ECCV、NeurIPS 和 ACM Multimedia 审稿人。此前在重庆大学获得硕士和学士学位。

research_tags:
  - 计算机视觉
  - 多模态 AI
  - 视觉语言模型
  - 视觉内容理解
  - 应用机器学习

project_experience_label: 科研项目
project_experience:
  - period: 2021年1月 – 2024年3月
    title: 受损存储中的图像与视频恢复
    organization: 新加坡国家研究基金会（NRF）
    output: CVPR · NeurIPS · IEEE TMM
  - period: 2024年3月 – 2024年12月
    title: 工业视觉检测与分析
    organization: Schaeffler–NTU Corporate Lab · Phase II
    output: ICIP · EMNLP · ACM MM · KBS
  - period: 2024年12月 – 2025年6月
    title: 多媒体安全数字水印
    organization: DSO National Laboratories, Singapore
    output: JVCIR 2025
  - period: 2025年6月 – 2025年11月
    title: 人机协作与动作重定向
    organization: Schaeffler–NTU Corporate Lab · Phase III
    output: 3D 姿态基准 · 动作重定向系统
  - period: 2025年11月 – 至今
    title: 面向智能制造的机器人视觉感知
    organization: Hyundai–NTU–A*STAR Corporate Lab
    output: ACM MM 2026 · 已申请专利
    current: true

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false

selected_papers: true
selected_papers_label: 精选论文
social: true

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
