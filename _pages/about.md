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
  /* ================================================= */
  /* Research Card Styles (Top Section)                */
  /* ================================================= */
  
  /* 卡片容器本身 - 需要相对定位来约束伪元素 */
  .research-card {
    position: relative; /* 关键：为伪元素提供定位锚点 */
    overflow: hidden; /* 防止装饰条意外溢出 */
    transition: background-color 0.3s ease; /* 保留背景色过渡效果 */
  }

  /* 默认状态的顶部装饰条 (使用 ::before 伪元素创建) */
  .research-card::before {
    content: ''; /* 伪元素必需 */
    position: absolute; /* 绝对定位于卡片内部 */
    top: 0;
    left: 50%;
    transform: translateX(-50%); /* 水平居中 */
    width: 60%; /* 装饰条宽度，可自行调整 */
    height: 4px; /* 默认的“细边框”厚度 */
    background-color: #7A0019; /* 你的主题红色 */
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
    transition: height 0.3s ease;
  }

  /* 悬停时卡片的变化 (只改变背景色) */
  .research-card:hover {
    background-color: rgba(122, 0, 25, 0.05) !important; /* 保留极其淡的红色填充 */
  }

  /* 悬停时装饰条的变化 (加粗) */
  .research-card:hover::before {
    height: 7px; /* 悬停时加粗后的厚度 */
  }


  /* ================================================= */
  /* Publication Card Styles (New Addition & Edits)    */
  /* ================================================= */

  /* 论文卡片容器 - 需要相对定位 */
  .publication-card {
    position: relative;
    transition: background-color 0.3s ease;
	margin-bottom: 32px; /* 新增：为每个卡片添加32px的底部间距 */
  }

  /* 默认状态的左侧装饰条 */
  .publication-card::before {
    content: '';
    position: absolute;
    left: 0;
    top: 50%;
    transform: translateY(-50%); /* 垂直居中 */
    height: 60%; 
    width: 5px;  
    background-color: #7A0019; /* 已更正为红色 */
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
    transition: width 0.3s ease;
  }

  /* 悬停时卡片的变化 (只改变背景色) */
  .publication-card:hover {
    background-color: rgba(122, 0, 25, 0.05); /* 保留极其淡的红色填充, !important 在这里非必需 */
  }

  /* 悬停时装饰条的变化 (加粗) */
  .publication-card:hover::before {
    width: 7px; /* 悬停时加粗后的厚度 */
  }
  
  /* 修改：调整论文卡片内部的留白 */
  .paper-box.publication-card {
    padding-top: 10px;
    padding-bottom: 15px;
    padding-left: 20px;  /* 修改：在左侧推出空间，避免内容遮挡 */
    padding-right: 15px; /* 修改：右侧也增加一点空间，让左右对称 */
	border-radius: 12px; /* 新增：与 Research Highlights 卡片统一圆角 */
  }
  
  /* 新增：进一步压缩卡片内文字元素的间距 */
  .publication-card .paper-box-text > * {
    margin-top: 8px;
    margin-bottom: 8px;
  }

  /* 新增：缩小 Highlights 部分列表项的字体大小 */
  .publication-card .paper-box-text ul li {
    font-size: 0.9em;
  }

  /* 新增：为所有 .paper-box 元素添加阴影，保持与 Research Highlights 一致 */
  .paper-box {
    box-shadow: 0 4px 12px rgba(0,0,0,0.08);
  }


  /* 新增：为 Publication 子标题设计的“胶囊”样式 */
  .publication-subheading {
    display: inline-block; /* 让容器宽度自适应文字内容 */
    background-color: #4A708B; /* 使用主标题的蓝色 */
    color: white;
    padding: 8px 20px;
    border-radius: 999px; /* 创建完美的胶囊形状 */
    font-size: 1.1em;
    font-weight: bold;
    margin-top: 40px;
    margin-bottom: 25px;
  }
  /* 第一个子标题的上边距可以小一些 */
  .publication-subheading:first-of-type {
    margin-top: 30px;
  }

</style>




{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}


<span class='anchor' id='about-me'></span>
# 🙋‍♂️ <font color="#0056b3">About Me</font>

<p style="text-align: center; font-size: 1.2em; font-weight: bold; color: #7A0019; margin-bottom: 25px;">
A Problem-Solver Applying AI to Innovate in Complex Physical Systems.
</p>


I recently graduated with a **Master of Science in Artificial Intelligence** from the [China University of Petroleum (Beijing)](https://www.cup.edu.cn/), where I was advised by [Prof. Jin Yang](https://faculty.cup.edu.cn/yangjin/) and [Prof. Yu Song](https://www.cup.edu.cn/cupai/szdw/jsml/8dffb1d273ce495f8fbf8ac08cc014de.htm). My research focuses on building robust, intelligent systems to solve critical engineering challenges, with a special emphasis on the **three core themes highlighted below**.

During my Master's, I published **over 10 papers** in top-tier journals and conferences (**6 as first author/primary contributor**) and was honored to be selected for the **"List of 100 Exemplary Graduate Student Winners"** nationwide for the National Scholarship. I have also gained practical industry experience through engagements with CNOOC <img src="images/CNOOC Limited.svg" alt="CNOOC Logo" style="height:1em; vertical-align:-0.15em;">, CNPC <img src="images/CNPC.svg" alt="CNPC Logo" style="height:1em; vertical-align:-0.15em;">, and Kingsoft Cloud <img src="images/Kingsoft Cloud.svg" alt="Kingsoft Cloud Logo" style="height:1em; vertical-align:middle;">.

If you are interested in any aspect of my work, I am always open to discussions and collaborations. Feel free to reach out to me at - **zehuasong2000@outlook.com**.


<span class='anchor' id='Research-Highlights'></span>
# 🎯 <font color="#0056b3">Research Highlights</font>

My research is organized into three core themes.

<div style="display: flex; justify-content: space-around; flex-wrap: wrap; gap: 20px; margin-top: 25px;">

  <div class="research-card" style="flex: 1; min-width: 300px; max-width: 32%; border-radius: 12px; padding: 25px 25px 5px 25px; text-align: center; box-shadow: 0 4px 12px rgba(0,0,0,0.08); transition: all 0.3s ease; display: flex; flex-direction: column; justify-content: space-between;">
    <div>
      <h3 style="margin-top: 0px; color: #7A0019;">Predictive Modeling & Analysis</h3>
      <h4 style="font-style: italic; color: #555; margin-top: 5px; margin-bottom: 20px; font-weight: normal; border-top: 1px solid #eee; border-bottom: 1px solid #eee; padding: 8px 0;">Physics-Informed & Bayesian ML</h4>
      <p style="text-align: left; font-size: 0.95em;">My work on the <strong>HBPINN</strong> framework, which fuses PDEs with Bayesian Inference to create robust, uncertainty-aware digital twins.</p>
    </div>
    <div style="margin-top: 20px;">
      <p style="text-align: left; font-size: 0.9em; color: #666;"><strong>Keywords:</strong> PINNs, Digital Twins, Probabilistic Assessment</p>
      <p style="text-align: right; margin-top: 20px;">
        <a href="{{ "/images/Rh1.mp4" | relative_url }}" style="font-size: 0.9em; color: #0056b3; font-weight: bold; text-decoration: none;">「Link 1」</a>
      </p>
    </div>
  </div>

  <div class="research-card" style="flex: 1; min-width: 300px; max-width: 32%; border-radius: 12px; padding: 25px 25px 5px 25px; text-align: center; box-shadow: 0 4px 12px rgba(0,0,0,0.08); transition: all 0.3s ease; display: flex; flex-direction: column; justify-content: space-between;">
    <div>
      <h3 style="margin-top: 0px; color: #7A0019;">Model Adaptation & Refinement</h3>
      <h4 style="font-style: italic; color: #555; margin-top: 5px; margin-bottom: 20px; font-weight: normal; border-top: 1px solid #eee; border-bottom: 1px solid #eee; padding: 8px 0;">Sim-to-Real Adaptation</h4>
      <p style="text-align: left; font-size: 0.95em;">My two-stage framework for model adaptation, using <strong>DANN</strong> for initial transfer and <strong>Online Learning</strong> for continuous improvement.</p>
    </div>
    <div style="margin-top: 20px;">
      <p style="text-align: left; font-size: 0.9em; color: #666;"><strong>Keywords:</strong> DANN, Online Learning, Evergreen Models</p>
      <p style="text-align: right; margin-top: 20px;">
        <a href="{{ "/images/Rh2-2.mp4" | relative_url }}" style="font-size: 0.9em; color: #0056b3; font-weight: bold; text-decoration: none;">「Link 1」</a>
        <a href="{{ "/images/Rh2-1.mp4" | relative_url }}" style="font-size: 0.9em; color: #0056b3; font-weight: bold; text-decoration: none; margin-left: 15px;">「Link 2」</a>
      </p>
    </div>
  </div>

  <div class="research-card" style="flex: 1; min-width: 300px; max-width: 32%; border-radius: 12px; padding: 25px 25px 5px 25px; text-align: center; box-shadow: 0 4px 12px rgba(0,0,0,0.08); transition: all 0.3s ease; display: flex; flex-direction: column; justify-content: space-between;">
    <div>
      <h3 style="margin-top: 0px; color: #7A0019;">Intelligent Optimization & Control</h3>
      <h4 style="font-style: italic; color: #555; margin-top: 5px; margin-bottom: 20px; font-weight: normal; border-top: 1px solid #eee; border-bottom: 1px solid #eee; padding: 8px 0;">Deep Reinforcement Learning</h4>
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





<span class='anchor' id='News'></span>
# 🔥 <font color="#0056b3">News</font>

<div style="font-size: 0.92em;" markdown="1">
- ***2025.05*** &nbsp;🎉🎉 Humbled to be selected as one of 100 National Representatives for the National Scholarship, an honor featured in the **People's Daily**.
- ***2024.11*** &nbsp;🎉🎉 Our research on DRL for riser jetting, published in **Ocean Engineering**, was featured on **CCTV-10's "Ocean Strategy"** program!
- ***2022.07*** &nbsp;🎉🎉 Honored to be invited to join the **Deep-Sea Engineering Innovation Team** at my university.
</div>

<span class='anchor' id='Publications'></span>
# 📝 <font color="#0056b3">Publications</font>

<h3 style="margin-top: 30px; margin-bottom: 20px; padding-left: 15px; border-left: 5px solid #4A708B;">Under Review</h3>

<div class='paper-box publication-card'>
  <div class='paper-box-image'><div><div class="badge">Reliability Engineering & System Safety</div><img src='images/paper5.svg' alt="sym" width="100%"></div></div>
  <div class='paper-box-text'>
    <p><a >Hierarchical Bayesian Physics-Informed Network Model for Open-Hole Wellbore Instability: From Parameter Uncertainty to Reliability Assessment</a></p>
    <p><strong>Zehua Song</strong>, Yu Song, Jin Yang, Kejin Chen, Jianqiao Zhang, Xing Wang</p>
    <p><a ><strong>Highlights</strong></a></p>
    <ul>
      <li>A Hierarchical Bayesian Physics-Informed Network for Coupled Multi-Physics Systems.</li>
      <li>Fusing PINN-based Prediction with Bayesian Inference for Robust Uncertainty Quantification.</li>
      <li>Providing a Dynamic "Earliest Failure Time Profile" for Operational Decision Support.</li>
    </ul>
  </div>
</div>

<div class='paper-box publication-card'>
  <div class='paper-box-image'><div><div class="badge">International Journal of Rock Mechanics and Mining Sciences</div><img src='images/paper6.svg' alt="sym" width="100%"></div></div>
  <div class='paper-box-text'>
    <p><a >Intelligent Prediction and Optimization of Open-Hole Wellbore Multiphysics Stability: A Synergistic PINN-DRL Approach</a></p>
    <p>Yu Song, <strong>Zehua Song</strong>, Jin Yang, Kejin Chen, Kun Jiang, Jizhou Tang</p>
    <p><a ><strong>Highlights</strong></a></p>
    <ul>
      <li>A Synergistic PINN-DRL Framework for Integrated Prediction and Control.</li>
      <li>Establishing a Physics-Informed Digital Twin for High-Speed, Physically-Consistent State Prediction.</li>
      <li>DRL-Driven Optimization of Drilling Fluid Parameters, Achieving a 32.33% Average Delay in Instability Onset.</li>
    </ul>
  </div>
</div>


<div class='paper-box publication-card'>
  <div class='paper-box-image'><div><div class="badge">Acta Petrolei Sinica (石油学报)</div><img src='images/Asia.svg' alt="sym" width="100%"></div></div>
  <div class='paper-box-text'>
    <p><a >A Parzen-Estimator-Enhanced Bayesian Optimization Framework for Deepwater Conductor Jetting</a></p>
    <p>Yu Song, Jin Yang, <strong>Zehua Song</strong></p>
    <p><a ><strong>Highlights</strong></a></p>
    <ul>
      <li>A Phased Bayesian Optimization Framework Combining Global Search and Local Refinement.</li>
      <li>Achieving a 12.78% Reduction in Total Installation Time by Optimizing the Trade-off Between Drilling and Soaking Phases.</li>
    </ul>
  </div>
</div>


<h3 style="margin-top: 40px; margin-bottom: 20px; padding-left: 15px; border-left: 5px solid #4A708B;">Published</h3>


<div class='paper-box publication-card'>
  <div class='paper-box-image'><div><div class="badge">Reliability Engineering & System Safety</div><img src='images/RESS-1.svg' alt="sym" width="100%"></div></div>
  <div class='paper-box-text'>
    <p><a href="papers/RESS.pdf">Enhancing energy efficiency and sustainability in offshore drilling through real-time multi-objective optimization: Considering lag effects and formation variability</a></p>
    <p>Yu Song, <strong>Zehua Song</strong>, Jin Yang, Kejin Chen, Jizhou Tang</p>
    <p><a href="https://www.sciencedirect.com/science/article/abs/pii/S0951832025003394"><strong>Highlights</strong></a></p>
    <ul>
      <li>AI-Enhanced Framework Addressing Formation Variability in Offshore Drilling.</li>
      <li>Mitigating Lag Effects for Enhanced Formation Perception and Safety.</li>
      <li>Empirical Validation Highlighting Efficiency Gains and Sustainability.</li>
    </ul>
  </div>
</div>



<div class='paper-box publication-card'>
  <div class='paper-box-image'><div><div class="badge">Geoenergy Science and Engineering</div><img src='images/JPSE-1.svg' alt="sym" width="100%"></div></div>
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

<div class='paper-box publication-card'>
  <div class='paper-box-image'><div><div class="badge">ISOPE 2024</div><img src='images/ISOPE 2024-1.svg' alt="sym" width="100%"></div></div>
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

<div class='paper-box publication-card'>
  <div class='paper-box-image'><div><div class="badge">Ocean Engineering</div><img src='images/OE1.svg' alt="sym" width="100%"></div></div>
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

<div class='paper-box publication-card'>
  <div class='paper-box-image'><div><div class="badge">ISOPE 2023</div><img src='images/ISOPE 2023-1.svg' alt="sym" width="100%"></div></div>
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
- <span style="background-color: #133599; color: white; padding: 1px 4px; font-size: 0.85em; line-height: 1;">Process Safety and Environmental Protection</span> <a href="https://www.sciencedirect.com/science/article/abs/pii/S0957582025001119">Deep learning based early warning methodology for gas kick of deepwater drilling using pilot-scale rig data</a>, Qishuai Yin, Qikang Zhu, <strong>Zehua Song</strong>, et al.
- <span style="background-color: #133599; color: white; padding: 1px 4px; font-size: 0.85em; line-height: 1;">GOTECH 2023</span> <a href="papers/GOTECH 2023-Xu.pdf">Research on Pore Pressure Prediction Technology of HTHP Wells in South China Sea Based on Machine Learning</a>, Dongsheng Xu, Jin Yang, ..., <strong>Zehua Song</strong>, et al.
- <span style="background-color: #133599; color: white; padding: 1px 4px; font-size: 0.85em; line-height: 1;">OTC 2023</span> <a href="papers/OTC 2023-Chen.pdf">Digital Twin: Hybrid Virtual Simulation and Physical Monitoring Strategy...</a>, Kejin Chen, Jin Yang, ..., <strong>Zehua Song</strong>, et al.
- <span style="background-color: #133599; color: white; padding: 1px 4px; font-size: 0.85em; line-height: 1;">ISOPE 2024</span> <a href="papers/ISOPE 2024-Gao.pdf">Deep Ocean Hydrographic Element Acquisition Device Based on Edge Computing...</a>, Bingzhen Gao, Jin Yang, ..., <strong>Zehua Song</strong>, et al.
</div>

<h3 style="margin-top: 40px; margin-bottom: 20px; padding-left: 15px; border-left: 5px solid #4A708B;">In Preparation</h3>

<div class='paper-box publication-card'>
  <div class='paper-box-image'><div><div class="badge">SPE Journal</div><img src='images/SPEJ.svg' alt="sym" width="100%"></div></div>
  <div class='paper-box-text'>
    <p>Adaptive Drilling Decision-Making Framework for Extended-Reach Wells under Multiple Objectives</p>
    <p>Yu Song, <strong>Zehua Song</strong>, ……</p>
  </div>
</div>





<span class='anchor' id='Honors-and-Awards'></span>
# 🏆️ <font color="#0056b3">Honors and Awards</font>

<div style="font-size: 0.99em;">
<table style="width: 100%; border: none; border-collapse: collapse;">
  <tbody>
    <tr style="border: none;">
      <td style="border: none; padding: 5px 10px 5px 0; text-align: left;">
        <span style="color: #7A0019; font-weight: bold;">One of 100 Exemplary Graduate Student Winners</span> (Featured in the People's Daily)
      </td>
      <td style="border: none; padding: 5px 0; text-align: left; width: 15%;"><em>2025</em></td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 5px 10px 5px 0; text-align: left;">
        <span style="color: #7A0019; font-weight: bold;">Beijing Outstanding Graduate</span> (A top honor awarded by the Beijing Government)
      </td>
      <td style="border: none; padding: 5px 0; text-align: left; width: 15%;"><em>2025</em></td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 5px 10px 5px 0; text-align: left;">
        <span style="font-weight: bold;">Professional Practice Excellence Award</span> (Top 1%)
      </td>
      <td style="border: none; padding: 5px 0; text-align: left; width: 15%;"><em>2025</em></td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 5px 10px 5px 0; text-align: left;">
        <span style="color: #7A0019; font-weight: bold;">National Scholarship for Postgraduates</span> (Top 1% Nationwide)
      </td>
      <td style="border: none; padding: 5px 0; text-align: left; width: 15%;"><em>2024</em></td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 5px 10px 5px 0; text-align: left;">
        <span style="color: #7A0019; font-weight: bold;">First Prize, National College Students Data Analysis Competition</span>
      </td>
      <td style="border: none; padding: 5px 0; text-align: left; width: 15%;"><em>2022</em></td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 5px 10px 5px 0; text-align: left;">
        <span style="font-weight: bold;">Second Prize, National Finals of China Ocean Engineering Design Competition</span>
      </td>
      <td style="border: none; padding: 5px 0; text-align: left; width: 15%;"><em>2022</em></td>
    </tr>
     <tr style="border: none;">
      <td style="border: none; padding: 5px 10px 5px 0; text-align: left;">
        <span style="font-weight: bold;">First-Class Scholarship</span> (Awarded for 5 consecutive years)
      </td>
      <td style="border: none; padding: 5px 0; text-align: left; width: 15%;"><em>2020 - 2024</em></td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 5px 10px 5px 0; text-align: left;">
        <span style="font-weight: bold;">United Energy Outstanding Student Scholarship</span> (Top 1%)
      </td>
      <td style="border: none; padding: 5px 0; text-align: left; width: 15%;"><em>2019</em></td>
    </tr>
  </tbody>
</table>
</div>


<span class='anchor' id='Education'></span>
# 📖 <font color="#0056b3">Education</font>

<div style="font-size: 0.99em;">
<table style="width: 100%; border: none; border-collapse: collapse;">
  <tbody>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <strong>M.Sc. in Artificial Intelligence</strong><br>
        <small style="color: #555;">China University of Petroleum (Beijing) (Project 211, Double First-Class)</small>
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%; font-style: italic; color: #555;">2022.09 - 2025.06</td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <strong>B.Eng. in Artificial Intelligence</strong><br>
        <small style="color: #555;">China University of Petroleum (Beijing)</small>
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%; font-style: italic; color: #555;">2019.12 - 2022.07</td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <strong>B.Eng. in Oil and Gas Storage and Transportation Engineering</strong><br>
        <small style="color: #7A0019;">*Selected for the highly competitive Integrated Bachelor's-Master's Program in AI.*</small>
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%; font-style: italic; color: #555;">2018.09 - 2019.12</td>
    </tr>
  </tbody>
</table>
</div>


<span class='anchor' id='Oral-Presentations'></span>
# 💬 <font color="#0056b3">Oral Presentations</font>

<div style="font-size: 0.99em;">
<table style="width: 100%; border: none; border-collapse: collapse;">
  <tbody>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <strong>International Society of Offshore and Polar Engineers 2024 Conference</strong><br>
        <small style="color: #555;"><em>A Real-Time Inversion Framework for Carbon Equivalent Emissions Based on Vision Transformer</em></small>
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%; font-style: italic; color: #555;">Rhodes, Greece<br>2024.06</td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <strong>International Society of Offshore and Polar Engineers 2023 Conference</strong><br>
        <small style="color: #555;"><em>Early Warning of Deep-Water Drilling Influx Based on Machine Learning</em></small>
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%; font-style: italic; color: #555;">Vancouver, Canada<br>2023.06</td>
    </tr>
  </tbody>
</table>
</div>


<span class='anchor' id='Industry-Experience'></span>
# 💻 <font color="#0056b3">Industry Experience</font>

<div style="font-size: 0.99em;">
<table style="width: 100%; border: none; border-collapse: collapse;">
  <tbody>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <strong>Visiting Student Researcher, CNOOC Ltd. (Hainan & Shenzhen)</strong><br>
        <small style="color: #555;">Focused on offshore engineering operations and the architecture of real-time data acquisition systems.</small>
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%; font-style: italic; color: #555;">2023</td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <strong>Data Science Intern, Kingsoft Cloud</strong><br>
        <small style="color: #555;">Worked on cloud computing infrastructure and data processing pipelines for enterprise-level clients.</small>
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%; font-style: italic; color: #555;">2021.07 - 2021.09</td>
    </tr>
    <tr style="border: none;">
      <td style="border: none; padding: 8px 10px 8px 0; text-align: left;">
        <strong>Field Engineering Intern, CNPC Xinjiang Oilfield</strong><br>
        <small style="color: #555;">Acquired foundational experience in oil & gas field operations and data collection protocols.</small>
      </td>
      <td style="border: none; padding: 8px 0; text-align: left; width: 15%; font-style: italic; color: #555;">2019.07 - 2019.08</td>
    </tr>
  </tbody>
</table>
</div>


<span class='anchor' id='Visitor-Map'></span>
# 🌏️ <font color="#0056b3">Visitor Map</font>

<div id="clustrmaps-container" style="width: 250px; height: 250px; margin: 0 auto;">

  <script type="text/javascript" id="clstr_globe" src="//clustrmaps.com/globe.js?d=2a65RVkDQtsNVgLvnJPUt-6ACnWUxt8CSOdNZ81OM1A"></script>

</div>