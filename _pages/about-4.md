---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  /* The main flat header style for all sections */
  .flat-header {
    background-color: #4A708B; /* Main theme color */
    color: white;
    padding: 12px 20px;
    border-radius: 8px; /* Slightly rounded corners for a modern feel */
    margin-top: 50px;
    margin-bottom: 30px;
  }
  .flat-header h2 {
    margin: 0;
    font-size: 1.6em;
    color: white !important; /* Force color to be white */
  }
  
  /* The flat card style for Research Highlights */
  .flat-card {
    flex: 1;
    min-width: 300px;
    max-width: 32%;
    border: 2px solid #e8e8e8; /* Clean, light border */
    border-radius: 12px;
    padding: 25px 25px 15px 25px;
    text-align: center;
    transition: border-color 0.3s ease; /* Smooth transition for hover */
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
  .flat-card:hover {
    border-color: #7A0019; /* Highlight color on hover */
  }
  .flat-card h3 {
    margin-top: 0;
    color: #7A0019;
  }
  .flat-card h4 {
    font-style: italic; color: #555; margin-top: 5px; margin-bottom: 20px; font-weight: normal; border-top: 1px solid #eee; border-bottom: 1px solid #eee; padding: 8px 0;
  }

  /* Style for tables to make them cleaner */
  .clean-table tr {
    border-bottom: 1px solid #f0f0f0; /* Very light separator line */
  }
  .clean-table tr:last-child {
    border-bottom: none; /* No line for the last item */
  }
</style>


{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}


<div class="flat-header">
  <h2>🙋‍♂️ About Me</h2>
</div>

<p style="text-align: center; font-size: 1.2em; font-weight: bold; color: #7A0019; margin-bottom: 25px;">
A Problem-Solver Applying AI to Innovate in Complex Physical Systems.
</p>

I recently graduated with a **Master of Science in Artificial Intelligence** from the [China University of Petroleum (Beijing)](https://www.cup.edu.cn/), where I was advised by [Prof. Jin Yang](https://faculty.cup.edu.cn/yangjin/) and [Prof. Yu Song](https://www.cup.edu.cn/cupai/szdw/jsml/8dffb1d273ce495f8fbf8ac08cc014de.htm). My research focuses on building robust, intelligent systems to solve critical engineering challenges, with a special emphasis on the **three core themes highlighted below**.

During my Master's, I published **over 10 papers** in top-tier journals and conferences (**6 as first author/primary contributor**) and was honored to be selected for the **"List of 100 Exemplary Graduate Student Winners"** nationwide for the National Scholarship. I have also gained practical industry experience through engagements with CNOOC <img src="images/CNOOC Limited.svg" alt="CNOOC Logo" style="height:1em; vertical-align:-0.15em;">, CNPC <img src="images/CNPC.svg" alt="CNPC Logo" style="height:1em; vertical-align:-0.15em;">, and Kingsoft Cloud <img src="images/Kingsoft Cloud.svg" alt="Kingsoft Cloud Logo" style="height:1em; vertical-align:middle;">.

If you are interested in any aspect of my work, I am always open to discussions and collaborations. Feel free to reach out to me at - **zehuasong2000@outlook.com**.


<div class="flat-header">
  <h2>🎯 Research Highlights</h2>
</div>

My research is organized into three core themes.

<div style="display: flex; justify-content: space-around; flex-wrap: wrap; gap: 20px; margin-top: 25px;">

  <div class="flat-card">
    <div>
      <h3>Predictive Modeling & Analysis</h3>
      <h4>Physics-Informed & Bayesian ML</h4>
      <p style="text-align: left; font-size: 0.95em;">My work on the <strong>HBPINN</strong> framework, which fuses PDEs with Bayesian Inference to create robust, uncertainty-aware digital twins.</p>
    </div>
    <div style="margin-top: 20px;">
      <p style="text-align: left; font-size: 0.9em; color: #666;"><strong>Keywords:</strong> PINNs, Digital Twins, Probabilistic Assessment</p>
      <p style="text-align: right; margin-top: 20px;">
        <a href="{{ "/images/Rh1.mp4" | relative_url }}" style="font-size: 0.9em; color: #0056b3; font-weight: bold; text-decoration: none;">「Link 1」</a>
      </p>
    </div>
  </div>

  <div class="flat-card">
    <div>
      <h3>Model Adaptation & Refinement</h3>
      <h4>Sim-to-Real Adaptation</h4>
      <p style="text-align: left; font-size: 0.95em;">My two-stage framework for model adaptation, using <strong>DANN</strong> for initial transfer and <strong>Online Learning</strong> for continuous improvement.</p>
    </div>
    <div style="margin-top: 20px;">
      <p style="text-align: left; font-size: 0.9em; color: #666;"><strong>Keywords:</strong> DANN, Online Learning, Evergreen Models</p>
      <p style="text-align: right; margin-top: 20px;">
        <a href="{{ "/images/Rh2_DANN.mp4" | relative_url }}" style="font-size: 0.9em; color: #0056b3; font-weight: bold; text-decoration: none;">「Link 1」</a>
        <a href="{{ "/images/Rh2_Online.mp4" | relative_url }}" style="font-size: 0.9em; color: #0056b3; font-weight: bold; text-decoration: none; margin-left: 15px;">「Link 2」</a>
      </p>
    </div>
  </div>

  <div class="flat-card">
    <div>
      <h3>Intelligent Optimization & Control</h3>
      <h4>Deep Reinforcement Learning</h4>
      <p style="text-align: left; font-size: 0.95em;">My work on the <strong>DN-SAC</strong> agent, which learns an instantaneous optimal policy to control complex systems in a POMDP setting.</p>
    </div>
    <div style="margin-top: 20px;">
      <p style="text-align: left; font-size: 0.9em; color: #666;"><strong>Keywords:</strong> DRL, Optimal Control, World Models</p>
      <p style="text-align: right; margin-top: 20px;">
        <a href="{{ "/images/Rh3.mp4" | relative_url }}" style="font-size: 0.9em; color: #0056b3; font-weight: bold; text-decoration: none;">「Link 1」</a>
      </p>
    </div>
  </div>
</div>


<div class="flat-header">
  <h2>🔥 News</h2>
</div>

<div style="font-size: 1em;" markdown="1">
- ***2025.09*** &nbsp;🎉🎉 Paper on our multi-objective DRL framework for drilling optimization published in **Geoenergy Science and Engineering**!
- ***2025.07*** &nbsp;🎉🎉 Selected as one of 100 National Representatives for the National Scholarship, featured in the **People's Daily**.
- ***2024.06*** &nbsp;🎉🎉 Presented my first-author research on Vision Transformers at **ISOPE 2024** in Rhodes, Greece.
- ***2024.04*** &nbsp;🎉🎉 Our paper on multi-objective optimization was published in **Reliability Engineering & System Safety**.
</div>


<div class="flat-header">
  <h2>📝 Publications</h2>
</div>

<h3 style="margin-top: 30px; margin-bottom: 20px; padding-left: 15px; border-left: 5px solid #4A708B;">Under Review</h3>

<div class='paper-box'>
  <div class='paper-box-image'><div><div class="badge">Reliability Engineering & System Safety</div><img src='images/RESS.svg' alt="sym" width="100%"></div></div>
  <div class='paper-box-text'>
    <p><a href="papers/RESS.pdf">Optimization of Multi-Objective Real-Time Drilling Operations Considering Lag Effects and Formation Variability</a></p>
    <p>Yu Song, <strong>Zehua Song</strong>, Jin Yang, Kejin Chen, Jizhou Tang</p>
    <p><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4937873"><strong>Highlights</strong></a></p>
    <ul>
      <li>AI-Enhanced Framework Addressing Formation Variability in Offshore Drilling.</li>
      <li>Mitigating Lag Effects for Enhanced Formation Perception and Safety.</li>
      <li>Empirical Validation Highlighting Efficiency Gains and Sustainability.</li>
    </ul>
  </div>
</div>


<h3 style="margin-top: 40px; margin-bottom: 20px; padding-left: 15px; border-left: 5px solid #4A708B;">Published</h3>

<div class='paper-box'>
  <div class='paper-box-image'><div><div class="badge">Geoenergy Science and Engineering</div><img src='images/JPSE.svg' alt="sym" width="100%"></div></div>
  <div class='paper-box-text'>
    <p><a href="papers/JPSE.pdf">A Multi-Objective Reinforcement Learning Framework for Real-Time Drilling Optimization Based on Symbolic Regression and Drilling Perception</a></p>
    <p><strong>Zehua Song</strong>, Yu Song, Jin Yang, Baosheng Liu, Bingzhen Gao, Jizhou Tang</p>
    <p><a href="https://www.sciencedirect.com/science/article/pii/S2949891024007620"><strong>Highlights</strong></a></p>
    <ul>
      <li>Integrating Symbolic Regression for Enhanced Drilling Parameter Mapping.</li>
      <li>Advancing Drilling Perception with Real-Time Adaptability.</li>
      <li>Empirical Validation and Broad Applicability in Drilling Optimization.</li>
    </ul>
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'><div><div class="badge">ISOPE 2024</div><img src='images/ISOPE 2024.svg' alt="sym" width="100%"></div></div>
  <div class='paper-box-text'>
    <p><a href="papers/ISOPE 2024.pdf">A Real-Time Inversion Framework for Carbon Equivalent Emissions in Oil and Gas Extraction Based on Vision Transformer</a></p>
    <p><strong>Zehua Song</strong>, Xiaoyang Yu, Yu Song, Jin Yang, Dongsheng Xu, Kejin Chen, Fangfei Huang, Bin Chen, Yanwei Song</p>
    <p><a href="https://onepetro.org/ISOPEIOPEC/proceedings-abstract/ISOPE24/All-ISOPE24/546127"><strong>Highlights</strong></a></p>
    <ul>
      <li>ViT-UNet Framework for Carbon Emission Quantification.</li>
      <li>Spatial Distribution Analysis of Offshore Carbon Emissions.</li>
    </ul>
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'><div><div class="badge">Ocean Engineering</div><img src='images/OE.svg' alt="sym" width="100%"></div></div>
  <div class='paper-box-text'>
    <p><a href="papers/OE.pdf">Multi-Objective Optimization Framework for Deepwater Riser Jetting Installation Parameters Using Deep Reinforcement Learning</a></p>
    <p>Yu Song, <strong>Zehua Song</strong>, Jin Yang, Lei Li</p>
    <p><a href="https://www.sciencedirect.com/science/article/abs/pii/S0029801824017360"><strong>Highlights</strong></a></p>
    <ul>
      <li>Advanced Prediction Model for Conductor Casing Jetting Time.</li>
      <li>Comprehensive Mechanism Analysis and Optimization Framework.</li>
      <li>Reinforcement Learning-Driven Optimization and Practical Validation.</li>
    </ul>
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'><div><div class="badge">ISOPE 2023</div><img src='images/ISOPE 2023.svg' alt="sym" width="100%"></div></div>
  <div class='paper-box-text'>
    <p><a href="papers/ISOPE 2023.pdf">Early Warning of Deep-Water Drilling Influx Based on Machine Learning</a></p>
    <p>Qishuai Yin, <strong>Zehua Song</strong>, Kejin Chen, Xu Zhou, Mayank Tyagi, Li Li</p>
    <p><a href="https://onepetro.org/ISOPEIOPEC/proceedings-abstract/ISOPE23/All-ISOPE23/524254"><strong>Highlights</strong></a></p>
    <ul>
      <li>Enhanced Signal Monitoring with Side-Bypass Pipe Design.</li>
      <li>Integrated Monitoring to Resolve Delays and Inaccuracies.</li>
      <li>Machine Learning Innovations for Gas Kick Early Warning.</li>
    </ul>
  </div>
</div>


<h3 style="margin-top: 40px; margin-bottom: 20px; padding-left: 15px; border-left: 5px solid #4A708B;">Other Co-authored Works</h3>

<div markdown="1" style="font-size: 0.95em; padding-left: 15px;">
- <span style="background-color: #133599; color: white; padding: 1px 4px; font-size: 0.85em; line-height: 1;">GOTECH 2023</span> <a href="papers/GOTECH 2023-Xu.pdf">Research on Pore Pressure Prediction Technology of HTHP Wells in South China Sea Based on Machine Learning</a>, Dongsheng Xu, Jin Yang, ..., <strong>Zehua Song</strong>, et al.
- <span style="background-color: #133599; color: white; padding: 1px 4px; font-size: 0.85em; line-height: 1;">OTC 2023</span> <a href="papers/OTC 2023-Chen.pdf">Digital Twin: Hybrid Virtual Simulation and Physical Monitoring Strategy...</a>, Kejin Chen, Jin Yang, ..., <strong>Zehua Song</strong>, et al.
- <span style="background-color: #133599; color: white; padding: 1px 4px; font-size: 0.85em; line-height: 1;">ISOPE 2024</span> <a href="papers/ISOPE 2024-Gao.pdf">Deep Ocean Hydrographic Element Acquisition Device Based on Edge Computing...</a>, Bingzhen Gao, Jin Yang, ..., <strong>Zehua Song</strong>, et al.
</div>


<h3 style="margin-top: 40px; margin-bottom: 20px; padding-left: 15px; border-left: 5px solid #4A708B;">In Preparation</h3>

<div class='paper-box'>
  <div class='paper-box-image'><div><div class="badge">SPE Journal</div><img src='images/SPEJ.svg' alt="sym" width="100%"></div></div>
  <div class='paper-box-text'>
    <p>Adaptive Drilling Decision-Making Framework for Extended-Reach Wells under Multiple Objectives</p>
    <p>Yu Song, <strong>Zehua Song</strong>, ……</p>
  </div>
</div>


<div class="flat-header">
  <h2>🏆️ Honors and Awards</h2>
</div>

<div style="font-size: 0.99em;">
<table class="clean-table" style="width: 100%; border: none; border-collapse: collapse;">
  <tbody>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <span style="color: #7A0019; font-weight: bold;">One of 100 Exemplary Graduate Student Winners</span> (Featured in the People's Daily)
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%;"><em>2025</em></td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <span style="color: #7A0019; font-weight: bold;">Beijing Outstanding Graduate</span> (A top honor awarded by the Beijing Government)
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%;"><em>2025</em></td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <span style="font-weight: bold;">Professional Practice Excellence Award</span> (Top 1%)
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%;"><em>2025</em></td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <span style="color: #7A0019; font-weight: bold;">National Scholarship for Postgraduates</span> (Top 1% Nationwide)
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%;"><em>2024</em></td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <span style="color: #7A0019; font-weight: bold;">First Prize, National College Students Data Analysis Competition</span>
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%;"><em>2022</em></td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <span style="font-weight: bold;">Second Prize, National Finals of China Ocean Engineering Design Competition</span>
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%;"><em>2022</em></td>
    </tr>
     <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <span style="font-weight: bold;">First-Class Scholarship</span> (Awarded for 5 consecutive years)
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%;"><em>2020 - 2024</em></td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <span style="font-weight: bold;">United Energy Outstanding Student Scholarship</span> (Top 1%)
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%;"><em>2019</em></td>
    </tr>
  </tbody>
</table>
</div>


<div class="flat-header">
  <h2>📖 Education</h2>
</div>

<div style="font-size: 0.99em;">
<table class="clean-table" style="width: 100%; border: none; border-collapse: collapse;">
  <tbody>
    <tr style="border: none;">
      <td style="border: none; padding: 10px 10px 10px 0; text-align: left;">
        <strong>M.Sc. in Artificial Intelligence</strong><br>
        <small style="color: #555;">China University of Petroleum (Beijing) (Project 211, Double First-Class)</small>
      </td>
      <td style="border: none; padding: 10px 0; text-align: left; width: 15%; font-style: italic; color: #555;">2022.09 - 2025.06</td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 10px 10px 10px 0; text-align: left;">
        <strong>B.Eng. in Artificial Intelligence</strong><br>
        <small style="color: #555;">China University of Petroleum (Beijing)</small>
      </td>
      <td style="border: none; padding: 10px 0; text-align: left; width: 15%; font-style: italic; color: #555;">2019.12 - 2022.07</td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 10px 10px 10px 0; text-align: left;">
        <strong>B.Eng. in Oil and Gas Storage and Transportation Engineering</strong><br>
        <small style="color: #7A0019;">*Selected for the highly competitive Integrated Bachelor's-Master's Program in AI.*</small>
      </td>
      <td style="border: none; padding: 10px 0; text-align: left; width: 15%; font-style: italic; color: #555;">2018.09 - 2019.12</td>
    </tr>
  </tbody>
</table>
</div>


<div class="flat-header">
  <h2>💬 Oral Presentations</h2>
</div>

<div style="font-size: 0.99em;">
<table class="clean-table" style="width: 100%; border: none; border-collapse: collapse;">
  <tbody>
    <tr style="border: none;">
      <td style="border: none; padding: 10px 10px 10px 0; text-align: left;">
        <strong>International Society of Offshore and Polar Engineers 2024 Conference</strong><br>
        <small style="color: #555;"><em>A Real-Time Inversion Framework for Carbon Equivalent Emissions Based on Vision Transformer</em></small>
      </td>
      <td style="border: none; padding: 10px 0; text-align: left; width: 20%; font-style: italic; color: #555;">Rhodes, Greece<br>2024.06</td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 10px 10px 10px 0; text-align: left;">
        <strong>International Society of Offshore and Polar Engineers 2023 Conference</strong><br>
        <small style="color: #555;"><em>Early Warning of Deep-Water Drilling Influx Based on Machine Learning</em></small>
      </td>
      <td style="border: none; padding: 10px 0; text-align: left; width: 20%; font-style: italic; color: #555;">Vancouver, Canada<br>2023.06</td>
    </tr>
  </tbody>
</table>
</div>


<div class="flat-header">
  <h2>💻 Industry Experience</h2>
</div>

<div style="font-size: 0.99em;">
<table class="clean-table" style="width: 100%; border: none; border-collapse: collapse;">
  <tbody>
    <tr style="border: none;">
      <td style="border: none; padding: 10px 10px 10px 0; text-align: left;">
        <strong>Visiting Student Researcher, CNOOC Ltd. (Hainan & Shenzhen)</strong><br>
        <small style="color: #555;">Focused on offshore engineering operations and the architecture of real-time data acquisition systems.</small>
      </td>
      <td style="border: none; padding: 10px 0; text-align: left; width: 15%; font-style: italic; color: #555;">2023</td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 10px 10px 10px 0; text-align: left;">
        <strong>Data Science Intern, Kingsoft Cloud</strong><br>
        <small style="color: #555;">Worked on cloud computing infrastructure and data processing pipelines for enterprise-level clients.</small>
      </td>
      <td style="border: none; padding: 10px 0; text-align: left; width: 15%; font-style: italic; color: #555;">2021.07 - 2021.09</td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 10px 10px 10px 0; text-align: left;">
        <strong>Field Engineering Intern, CNPC Xinjiang Oilfield</strong><br>
        <small style="color: #555;">Acquired foundational experience in oil & gas field operations and data collection protocols.</small>
      </td>
      <td style="border: none; padding: 10px 0; text-align: left; width: 15%; font-style: italic; color: #555;">2019.07 - 2019.08</td>
    </tr>
  </tbody>
</table>
</div>


<div class="flat-header">
  <h2>🌏️ Visitor Map</h2>
</div>

<div id="clustrmaps-container" style="width: 250px; height: 250px; margin: 0 auto;">
  <script type="text/javascript" id="clstr_globe" src="//clustrmaps.com/globe.js?d=2a65RVkDQtsNVgLvnJPUt-6ACnWUxt8CSOdNZ81OM1A"></script>
</div>