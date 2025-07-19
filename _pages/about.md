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
    <div>
    - <span class="primary-gradient-text">WiFi Sensing</span>
    - <span class="primary-gradient-text">Federated Learning</span>
    - <span class="primary-gradient-text">Wireless Communication</span>
    </div>
</div>


<div class="highlight-blocks">
  <div class="highlight-block floating-card">
    <h3><i class="fas fa-microscope"></i> Research Interests</h3>
    <ul>
      <li>Research focus on <span class="accent-text">Federated Learning</span></li>
      <li>Seasoned with a dash of <span class="primary-gradient-text">Wireless Communication</span></li>
      <li>Topped off with a dollop of <span class="primary-gradient-text">WiFi Sensing</span></li>
      </ul>
  </div>
  
  <div class="highlight-block floating-card">
    <h3><i class="fas fa-pen-fancy"></i> Main Experiences</h3>
    <ul>
      <li>Publications at <span class="accent-text">TWC</span>, <span class="accent-text">TCCN</span>, <span class="accent-text">IoTJ</span></li>
      <li>As a <span class="accent-text">reviewer </span> for several flagship journals and conferences </li>
      <li> Participated in multiple <span class="accent-text">well-known international conferences </span></li>
    </ul>
  </div>
  </div>

# 📖 Educations
- *2020.09 - 2025.03*: &nbsp;Doctor of Philosophy in the College of Electronics and Information Engineering, <span class="primary-gradient-text">Tongji University</span>.
- *2017.09 - 2020.06*: &nbsp;Master of Science at the School of Computer and Information, <span class="primary-gradient-text">Anhui Normal University</span>.

# 🔥 News
- *2025.07*: &nbsp;🎉🎉 One paper “A Heterogeneity-Aware Federated Edge Learning Framework with RIS-empowered Wireless Aggregation
” is submitted to International Journal of Dynamics and Control. 

# 📝 Publications 

<div class="publication-box">
  <div class="publication-image">
    <div class="publication-badge">TWC 2022</div>
    <img src="images/onebit.png" alt="TWC Paper">
  </div>
  <div class="publication-content">
    <h3 class="publication-title">One Bit Aggregation for Federated Edge Learning With Reconfigurable Intelligent Surface: Analysis and Optimization</h3>
    <div class="publication-authors">
      <strong>H. Li</strong>, R. Wang*, W. Zhang, J. Wu
    </div>
    <div class="publication-venue">
      IEEE Transactions on Wireless Communications
    </div>
    <div class="publication-links">
      <a href="https://doi.org/10.1109/TWC.2022.3198881" class="publication-link">
        <i class="fas fa-file-pdf"></i> Paper
      </a>
      <a href="https://scholar.google.com.hk/citations?view_op=view_citation&hl=zh-CN&user=ay-NKfsAAAAJ&citation_for_view=ay-NKfsAAAAJ:qjMakFHDy7sC" class="publication-link">
        <strong>Project</strong>
      </a>
      <strong><span class='show_paper_citations' data='ayNKfsAAAAJ:qjMakFHDy7sC'></span></strong>
      </div>
  </div>
</div>

<div class="publication-box">
  <div class="publication-image">
    <div class="publication-badge">TWC 2023</div>
    <img src="images/scsi.png" alt="TWC Paper">
  </div>
  <div class="publication-content">
    <h3 class="publication-title">
      <a href="https://doi.org/10.1109/TWC.2023.3334250">Reconfigurable Intelligent Surface Empowered Federated Edge Learning With Statistical CSI</a>
    </h3>
    <div class="publication-authors">
      <strong>H. Li</strong>, R. Wang*, W. Zhang, J. Wu, I. Soto
    </div>
    <div class="publication-venue">
      IEEE Transactions on Wireless Communications
    </div>
    <div class="publication-links">
      <a href="https://doi.org/10.1109/TWC.2023.3334250" class="publication-link">
        <i class="fas fa-file-pdf"></i> Paper
      </a>
      <a href="https://scholar.google.com.hk/citations?view_op=view_citation&hl=zh-CN&user=ay-NKfsAAAAJ&citation_for_view=ay-NKfsAAAAJ:ufrVoPGSRksC" class="publication-link">
        <strong>Project</strong>
      </a>
      <strong><span class='show_paper_citations' data='ayNKfsAAAAJ:ufrVoPGSRksC'></span></strong>
    </div>
  </div>
</div>

<div class="publication-box">
  <div class="publication-image">
    <div class="publication-badge">TCCN 2025</div>
    <img src="images/admm.png" alt="TCCN Paper">
  </div>
  <div class="publication-content">
    <h3 class="publication-title">
      <a href="https://doi.org/10.1109/TCCN.2025.3578472">Efficient Federated Edge Learning with ADMM Over RIS Empowered Wireless Channels</a>
    </h3>
    <div class="publication-authors">
      <strong>H. Li</strong>, R. Wang*, J. Wu, J. Liu, Y. Li
    </div>
    <div class="publication-venue">
      IEEE Transactions on Cognitive Communications and Networking
    </div>
    <div class="publication-links">
      <a href="https://doi.org/10.1109/TCCN.2025.3578472" class="publication-link">
        <i class="fas fa-file-pdf"></i> Paper
      </a>
      <a href="https://scholar.google.com.hk/citations?view_op=view_citation&hl=zh-CN&user=ay-NKfsAAAAJ&citation_for_view=ay-NKfsAAAAJ:Se3iqnhoufwC" class="publication-link">
        <strong>Project</strong>
      </a>
      <strong><span class='show_paper_citations' data='ayNKfsAAAAJ:Se3iqnhoufwC'></span></strong>
    </div>
  </div>
</div>

<div class="publication-box">
  <div class="publication-image">
    <div class="publication-badge">IoTJ 2025</div>
    <img src="images/star.png" alt="IoTJ Paper">
  </div>
  <div class="publication-content">
    <h3 class="publication-title">
      <a href="https://doi.org/10.1109/JIOT.2025.3565698">STAR-RIS Empowered Heterogeneous Federated Edge Learning With Flexible Aggregation</a>
    </h3>
    <div class="publication-authors">
      <strong>H. Li</strong>, R. Wang*, M. Jiang, J. Liu
    </div>
    <div class="publication-venue">
      IEEE Internet of Things Journal
    </div>
    <div class="publication-links">
      <a href="https://doi.org/10.1109/JIOT.2025.3565698" class="publication-link">
        <i class="fas fa-file-pdf"></i> Paper
      </a>
      <a href="https://scholar.google.com.hk/citations?view_op=view_citation&hl=zh-CN&user=ay-NKfsAAAAJ&citation_for_view=ay-NKfsAAAAJ:roLk4NBRz8UC" class="publication-link">
        <strong>Project</strong>
      </a>
      <strong><span class='show_paper_citations' data='ayNKfsAAAAJ:roLk4NBRz8UC'></span></strong>    </div>
  </div>
</div>

<div class="publication-box">
  <div class="publication-image">
    <div class="publication-badge">WCL2025</div>
    <img src="images/wcl.png" alt="Paper Image">
  </div>
  <div class="publication-content">
    <h3 class="publication-title">
      <a href="https://doi.org/10.1109/LWC.2025.3557016">Latency Minimization for RIS Empowered Covert Federated Learning</a>
    </h3>
    <div class="publication-authors">
      <strong>H. Li</strong>, R. Wang*
    </div>
    <div class="publication-venue">
      IEEE Wireless Communications Letters
    </div>
    <div class="publication-links">
      <a href="https://doi.org/10.1109/LWC.2025.3557016" class="publication-link">
        <i class="fas fa-file-pdf"></i> Paper
      </a>
    </div>
  </div>
</div>

<div class="publication-box">
  <div class="publication-image">
    <div class="publication-badge">Access2019</div>
    <img src="images/access.png" alt="Paper Image">
  </div>
  <div class="publication-content">
    <h3 class="publication-title">
      <a href="https://doi.org/10.1109/ACCESS.2019.2948102">Wi-Motion: A Robust Human Activity Recognition Using WiFi Signals</a>
    </h3>
    <div class="publication-authors">
      <strong>H. Li</strong>, X. He*, X. Chen, Y. Fang, Q. Fang
    </div>
    <div class="publication-venue">
      IEEE Access
    </div>
    <div class="publication-links">
      <a href="https://doi.org/10.1109/ACCESS.2019.2948102" class="publication-link">
        <i class="fas fa-file-pdf"></i> Paper
      </a>
    </div>
  </div>
</div>

<div class="publication-box">
  <div class="publication-image">
    <div class="publication-badge">SY2025</div>
    <img src="images/sy.png" alt="Paper Image">
  </div>
  <div class="publication-content">
    <h3 class="publication-title">
      <a href="https://doi.org/10.3390/sym17071115">A Novel Heterogeneous Federated Edge Learning Framework Empowered with SWIPT</a>
    </h3>
    <div class="publication-authors">
      Y. Fang, S. Shu, Y. Zhu, <strong>H. Li*</strong>, K. Rui
    </div>
    <div class="publication-venue">
      Symmetry
    </div>
    <div class="publication-links">
      <a href="https://doi.org/10.3390/sym17071115" class="publication-link">
        <i class="fas fa-file-pdf"></i> Paper
      </a>
    </div>
  </div>
</div>

<div class="publication-box">
  <div class="publication-content">
    <h3 class="publication-title">
      <a href="https://doi.org/10.1109/GLOBECOM48099.2022.10001550">Federated Edge Learning via Reconfigurable Intelligent Surface with One-Bit Quantization</a>
    </h3>
    <div class="publication-authors">
      <strong>H. Li</strong>, R. Wang*, W. Zhang, J. Wu
    </div>
    <div class="publication-venue">
      <strong>GLOBECOM 2022</strong>
    </div>
    <div class="publication-links">
      <a href="https://doi.org/10.1109/GLOBECOM48099.2022.10001550" class="publication-link">
        <i class="fas fa-file-pdf"></i> Paper
      </a>
    </div>
  </div>
</div>

<div class="publication-box">
  <div class="publication-content">
    <h3 class="publication-title">
      <a href="https://doi.org/10.1109/ICCC57788.2023.10233543">RIS-Aided Federated Edge Learning Exploiting Statistical CSI</a>
    </h3>
    <div class="publication-authors">
      <strong>H. Li</strong>, R. Wang*, J. Wu, W. Zhang, I. Soto
    </div>
    <div class="publication-venue">
      <strong>2023 IEEE/CIC International Conference on Communications in China</strong>
    </div>
    <div class="publication-links">
      <a href="https://doi.org/10.1109/ICCC57788.2023.10233543" class="publication-link">
        <i class="fas fa-file-pdf"></i> Paper
      </a>
    </div>
  </div>
</div>


# <i class="fas fa-laptop-code"></i> Beyond Academics
I like <span class="primary-gradient-text">singing</span>, <span class="primary-gradient-text">dancing</span>, <span class="primary-gradient-text">rapping</span> and <span class="primary-gradient-text">playing basketball.
