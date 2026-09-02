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
  我目前在 Hyundai–NTU–A*STAR Corporate Lab 担任 **Research Fellow**，与 [Assoc. Prof. Wai Kin (Adams) Kong](https://personal.ntu.edu.sg/AdamsKong/) 合作开展研究。我的研究将基础模型与多模态学习应用于工业和机器人感知，当前工作涵盖少样本/零样本异常检测、开放词汇检测与分割、6D 位姿估计和机器人抓取。

  我在**南洋理工大学**获得电气与电子工程博士学位，导师为 [Prof. Lap-Pui Chau](https://www.polyu.edu.hk/eee/people/academic-staff-and-teaching-staff/prof-chau-lap-pui/)（IEEE Fellow）和 [Assoc. Prof. Kim-Hui Yap](https://dr.ntu.edu.sg/entities/person/Yap-Kim-Hui)，并拥有**重庆大学**硕士和学士学位。我的研究横跨稳健视觉学习、多媒体理解与真实场景感知。我已发表 **23 篇论文**，获 **340+ 次引用**（h-index 8），包括四篇 CCF-A 第一作者论文。

project_experience_label: 科研项目
project_experience:
  - period: 2025年11月 – 至今
    title: 工业机器人视觉感知
    organization: Hyundai–NTU–A*STAR Corporate Lab
    summary: 构建面向未见工业零件的开放世界检测、分割、6D 位姿估计与抓取生成流程，并开展少样本/零样本异常检测。
    output: ACM MM
    current: true
  - period: 2025年6月 – 2025年11月
    title: 人机协作
    organization: Schaeffler–NTU Corporate Lab · Phase III
    summary: 探索基于 RGB 与深度信息的 3D 人体姿态估计，开展模型评测并开发面向人机协作的动作重定向方法。
  - period: 2024年12月 – 2025年6月
    title: 鲁棒图像水印
    organization: DSO National Laboratories
    summary: 开发鲁棒图像水印与自监督水印去除方法，评估其在 JPEG 压缩、噪声、缩放等真实失真下的稳定性。
    output: JVCIR
  - period: 2024年3月 – 2024年12月
    title: 开放词汇工业视觉
    organization: Schaeffler–NTU Corporate Lab · Phase II
    summary: 开发开放词汇检测与分割方法，并研究有限监督条件下的人-物交互识别。
    output: EMNLP · ACM MM · KBS
  - period: 2021年1月 – 2024年3月
    title: 图像与视频恢复
    organization: 国家研究基金会
    summary: 开发基于学习的损坏图像与视频恢复方法，支持从闪存中可靠地恢复视觉数据。
    output: CVPR · NeurIPS · IEEE TMM
  - period: 2017年9月 – 2020年7月
    title: 视频解码与 AI 加速
    organization: 重庆大学
    summary: 开发带动态电压调节的任务级 H.264 并行解码方法，并参与高能效 CNN 光子加速研究。
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
