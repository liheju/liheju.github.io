---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
<style>
/* 确保网格布局正确显示 */
.blog-grid {
  display: grid !important;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)) !important;
  gap: 1.5rem !important;
  margin: 2rem 0 !important;
}

.blog-card {
  background: #ffffff !important;
  border-radius: 12px !important;
  overflow: hidden !important;
  box-shadow: 0 2px 12px rgba(1, 47, 99, 0.08) !important;
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1) !important;
}

.blog-card:hover {
  transform: translateY(-8px) !important;
  box-shadow: 0 8px 25px rgba(1, 47, 99, 0.15) !important;
}

.blog-card-image {
  position: relative !important;
  width: 100% !important;
  height: 200px !important;
  overflow: hidden !important;
}

.blog-card-image img {
  width: 100% !important;
  height: 100% !important;
  object-fit: cover !important;
  transition: transform 0.3s ease !important;
}

.blog-badge {
  position: absolute !important;
  top: 12px !important;
  left: 12px !important;
  background: linear-gradient(135deg, #FE667B 0%, #ff8599 100%) !important;
  color: white !important;
  padding: 0.4em 0.8em !important;
  border-radius: 20px !important;
  font-size: 0.75em !important;
  font-weight: 600 !important;
  box-shadow: 0 2px 8px rgba(254, 102, 123, 0.3) !important;
  z-index: 10 !important;
}

.blog-card-content {
  padding: 1.2rem !important;
}

.blog-title {
  font-size: 1.1rem !important;
  font-weight: 700 !important;
  color: #012F63 !important;
  margin-bottom: 0.8rem !important;
  line-height: 1.3 !important;
}

.blog-description {
  font-size: 0.9rem !important;
  color: #666 !important;
  line-height: 1.5 !important;
  margin-bottom: 1rem !important;
}

.blog-links {
  display: flex !important;
  gap: 0.6rem !important;
  flex-wrap: wrap !important;
  align-items: flex-end !important;
}

.blog-link {
  display: inline-flex !important;
  align-items: center !important;
  gap: 0.3rem !important;
  padding: 0.4em 0.8em !important;
  background: linear-gradient(135deg, #FE667B 0%, #ff8599 100%) !important;
  color: white !important;
  text-decoration: none !important;
  border-radius: 20px !important;
  font-size: 0.8rem !important;
  font-weight: 500 !important;
  transition: all 0.3s ease !important;
  box-shadow: 0 2px 8px rgba(254, 102, 123, 0.2) !important;
}

.blog-link:hover {
  transform: translateY(-2px) !important;
  box-shadow: 0 4px 12px rgba(254, 102, 123, 0.3) !important;
  color: white !important;
  text-decoration: none !important;
}

/* 响应式设计 */
@media (max-width: 768px) {
  .blog-grid {
    grid-template-columns: 1fr !important;
    gap: 1rem !important;
  }
  
  .blog-card-image {
    height: 180px !important;
  }
}

@media (min-width: 769px) and (max-width: 1024px) {
  .blog-grid {
    grid-template-columns: repeat(2, 1fr) !important;
  }
}

@media (min-width: 1025px) {
  .blog-grid {
    grid-template-columns: repeat(3, 1fr) !important;
  }
}

/* Publications统一设计风格 */
.publication-box {
  display: flex !important;
  background: #ffffff !important;
  border-radius: 12px !important;
  overflow: hidden !important;
  box-shadow: 0 2px 12px rgba(1, 47, 99, 0.08) !important;
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1) !important;
  margin: 1.5rem 0 !important;
  align-items: center !important;
  padding-left: 1.5rem !important;
}

.publication-box:hover {
  transform: translateY(-5px) !important;
  box-shadow: 0 8px 25px rgba(1, 47, 99, 0.15) !important;
}

.publication-image {
  position: relative !important;
  width: 280px !important;
  height: 180px !important;
  flex-shrink: 0 !important;
  overflow: hidden !important;
}

.publication-image img {
  width: 100% !important;
  height: 100% !important;
  object-fit: cover !important;
  transition: transform 0.3s ease !important;
}

.publication-image:hover img {
  transform: scale(1.03) !important;
}

.publication-badge {
  position: absolute !important;
  top: 12px !important;
  left: 0px !important;
  background: linear-gradient(135deg, #FE667B 0%, #ff8599 100%) !important;
  color: white !important;
  padding: 0.4em 0.8em !important;
  border-radius: 20px !important;
  font-size: 0.75em !important;
  font-weight: 600 !important;
  box-shadow: 0 2px 8px rgba(254, 102, 123, 0.3) !important;
  z-index: 10 !important;
}

.publication-content {
  flex: 1 !important;
  padding: 1.8rem 1.8rem 1.8rem 0.8rem !important;
  display: flex !important;
  flex-direction: column !important;
  gap: 0.8rem !important;
}

.publication-title {
  font-size: 1.25rem !important;
  font-weight: 700 !important;
  color: #012F63 !important;
  margin: 0 !important;
  line-height: 1.3 !important;
}

.publication-authors {
  font-size: 1rem !important;
  color: #333 !important;
  line-height: 1.4 !important;
}

.publication-venue {
  font-size: 0.95rem !important;
  color: #666 !important;
  font-style: italic !important;
}

.publication-links {
  display: flex !important;
  gap: 0.8rem !important;
  flex-wrap: wrap !important;
  margin-top: 0.5rem !important;
}

.publication-link {
  display: inline-flex !important;
  align-items: center !important;
  gap: 0.4rem !important;
  padding: 0.5em 1em !important;
  background: linear-gradient(135deg, #FE667B 0%, #ff8599 100%) !important;
  color: white !important;
  text-decoration: none !important;
  border-radius: 20px !important;
  font-size: 0.85rem !important;
  font-weight: 500 !important;
  transition: all 0.3s ease !important;
  box-shadow: 0 2px 8px rgba(254, 102, 123, 0.2) !important;
}

.publication-link:hover {
  transform: translateY(-2px) !important;
  box-shadow: 0 4px 12px rgba(254, 102, 123, 0.3) !important;
  color: white !important;
  text-decoration: none !important;
}

.publication-link i {
  font-size: 0.9em !important;
}

/* 响应式设计 - Publications */
@media (max-width: 768px) {
  .publication-box {
    flex-direction: column !important;
    margin: 1rem 0 !important;
  }
  
  .publication-image {
    width: 100% !important;
    height: 160px !important;
  }
  
  .publication-content {
    padding: 1.2rem !important;
    gap: 0.6rem !important;
  }
  
  .publication-title {
    font-size: 1.1rem !important;
  }
  
  .publication-authors,
  .publication-venue {
    font-size: 0.9rem !important;
  }
}

@media (min-width: 769px) and (max-width: 1024px) {
  .publication-image {
    width: 240px !important;
    height: 160px !important;
  }
  
  .publication-content {
    padding: 1.5rem 1.5rem 1.5rem 0.8rem !important;
  }
  
  .publication-title {
    font-size: 1.15rem !important;
  }
}
</style>






{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

# 🤵🏻 About me
My name is <span class="accent-text">Heju Li</span>. I received the M.S. degree from the School of Computer and Information, <i class="fas fa-university"></i> **Anhui Normal University**, Wuhu, China, in 2020, and the Ph.D. degree from the College of Electronics and Information Engineering, <i class="fas fa-university"></i> **Tongji University**,  Shanghai, China, in 2025. 

<div class="quote-accent">
Most recently, I am interested in the following topics:
- WiFi Sensing
- Federated Learning
- Wireless Communication.
</div>


# 🔥 News
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 

# 📝 Publications 

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TWC 2022</div><img src='images/onebit.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[One Bit Aggregation for Federated Edge Learning With Reconfigurable Intelligent Surface: Analysis and Optimization](https://doi.org/10.1109/TWC.2022.3198881)

**H. Li**, R. Wang*, W. Zhang, J. Wu

[**Project**](https://scholar.google.com.hk/citations?view_op=view_citation&hl=zh-CN&user=ay-NKfsAAAAJ&citation_for_view=ay-NKfsAAAAJ:qjMakFHDy7sC) <strong><span class='show_paper_citations' data='ay-NKfsAAAAJ:qjMakFHDy7sC'></span></strong>
- We propose in this work a novel reconfigurable intelligent surface aided one-bit communication optimization scheme under orthogonal frequency division multiple access to relieve the negative influence of communication error on the SignSGD-based FEEL.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TWC 2023</div><img src='images/scsi.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Reconfigurable Intelligent Surface Empowered Federated Edge Learning With Statistical CSI](https://doi.org/10.1109/TWC.2023.3334250)

**H. Li**, R. Wang*, W. Zhang, J. Wu, I. Soto

[**Project**](https://scholar.google.com.hk/citations?view_op=view_citation&hl=zh-CN&user=ay-NKfsAAAAJ&citation_for_view=ay-NKfsAAAAJ:ufrVoPGSRksC) <strong><span class='show_paper_citations' data='ay-NKfsAAAAJ:ufrVoPGSRksC'></span></strong>
- We investigate in this paper the RIS-aided FEEL system under the realistic supposition where only the statistical CSI is available among devices.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TCCN 2025</div><img src='images/admm.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Efficient Federated Edge Learning with ADMM Over RIS Empowered Wireless Channels](https://doi.org/10.1109/TCCN.2025.3578472)

**H. Li**, R. Wang*, J. Wu, J. Liu, Y. Li

[**Project**](https://scholar.google.com.hk/citations?view_op=view_citation&hl=zh-CN&user=ay-NKfsAAAAJ&citation_for_view=ay-NKfsAAAAJ:Se3iqnhoufwC) <strong><span class='show_paper_citations' data='ay-NKfsAAAAJ:Se3iqnhoufwC'></span></strong>
- We focus in this paper on analyzing the training performance of the ADMM-based FEEL system in the presence of noisy wireless channels, and accordingly deploy the reconfigurable intelligent surface to simultaneously assist both the uplink and the downlink transmission.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">IoTJ 2025</div><img src='images/scsi.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[STAR-RIS Empowered Heterogeneous Federated Edge Learning With Flexible Aggregation](https://doi.org/10.1109/JIOT.2025.3565698)

**H. Li**, R. Wang*, M. Jiang, J. Liu

[**Project**](https://scholar.google.com.hk/citations?view_op=view_citation&hl=zh-CN&user=ay-NKfsAAAAJ&citation_for_view=ay-NKfsAAAAJ:roLk4NBRz8UC) <strong><span class='show_paper_citations' data='ay-NKfsAAAAJ:roLk4NBRz8UC'></span></strong>
- We propose in this paper a novel FEEL framework empowered by simultaneous transmitting and reflecting reconfigurable intelligent surface with flexible aggregation.
</div>
</div>

- <strong>H. Li</strong> and R. Wang*. Latency Minimization for RIS Empowered Covert Federated Learning. <strong>IEEE Wireless Communications Letters</strong> [[Paper]](https://doi.org/10.1109/LWC.2025.3557016)

- <strong>H. Li</strong>, X. He*, X. Chen, Y. Fang and Q. Fang. Wi-Motion: A Robust Human Activity Recognition Using WiFi Signals. <strong>IEEE Access</strong> [[Paper]](https://doi.org/10.1109/ACCESS.2019.2948102)

- <strong>H. Li</strong>, R. Wang*, W. Zhang, and J. Wu. Federated Edge Learning via Reconfigurable Intelligent Surface with One-Bit Quantization. <strong>GLOBECOM 2022</strong> [[Paper]](https://doi.org/10.1109/GLOBECOM48099.2022.10001550)

- <strong>H. Li</strong>, R. Wang*, J. Wu,  W. Zhang and I. Soto. RIS-Aided Federated Edge Learning Exploiting Statistical CSI. <strong>2023 IEEE/CIC International Conference on Communications in China</strong> [[Paper]](https://doi.org/10.1109/TWC.2023.3334250)

- Y. Fang, S. Shu, Y. Zhu, <strong>H. Li*</strong> and K. Rui. A Novel Heterogeneous Federated Edge Learning Framework Empowered with SWIPT. <strong>Symmetry</strong> [[Paper]](https://doi.org/10.3390/sym17071115)

# 🎖 Honors and Awards
- *2021.10* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.09* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 

# 📖 Educations
- *2019.06 - 2022.04 (now)*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2015.09 - 2019.06*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 

# 💬 Invited Talks
- *2021.06*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.03*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  \| [\[video\]](https://github.com/)

# 💻 Internships
- *2019.05 - 2020.02*, [Lorem](https://github.com/), China.