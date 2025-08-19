---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

Hi, I'm a second year graduate student at ShanghaiTech University. My current research focus in Deep Generative Models, such as Diffusion Bridge and Flow Matching.

I am a National Master of Sport in Chess, certified by the Chinese Chess Association.


<div style="display: flex; align-items: flex-start; margin: 20px 0; padding: 20px; background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%); border-radius: 15px; box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);">
  <div style="flex: 0 0 300px; margin-right: 30px;">
    <img src="images/zhu.png" alt="Chess Position" style="width: 100%; height: auto; border-radius: 10px; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);">
  </div>
  <div style="flex: 1; padding-left: 20px;">
    <h3 style="color: #2c3e50; margin-bottom: 15px; font-family: 'Georgia', serif;">♛ Featured Chess Analysis</h3>
    <div style="background: rgba(255, 255, 255, 0.9); padding: 15px; border-radius: 10px; box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.1);">
      <h4 style="color: #34495e; margin-bottom: 10px;">Move Sequence:</h4>
      <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(80px, 1fr)); gap: 8px; font-family: 'Courier New', monospace;">
        <span style="background: #3498db; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">1. Ne5</span>
        <span style="background: #e74c3c; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">d5</span>
        <span style="background: #3498db; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">2. exd5</span>
        <span style="background: #e74c3c; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">Bxe5</span>
        <span style="background: #3498db; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">3. dxc6</span>
        <span style="background: #e74c3c; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">Qh6</span>
        <span style="background: #3498db; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">4. Qe7</span>
        <span style="background: #e74c3c; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">Ng4</span>
        <span style="background: #3498db; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">5. Bg2</span>
        <span style="background: #e74c3c; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">Kg1</span>
        <span style="background: #3498db; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">6. Qc5</span>
        <span style="background: #e74c3c; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">Qe3</span>
        <span style="background: #3498db; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">7. Qxe3</span>
        <span style="background: #e74c3c; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">Nxe3</span>
        <span style="background: #3498db; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">8. Be4</span>
        <span style="background: #e74c3c; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">Bxg7</span>
        <span style="background: #3498db; color: white; padding: 4px 8px; border-radius: 5px; text-align: center; font-weight: bold;">9. Kxg7</span>
      </div>
      <p style="margin-top: 15px; color: #7f8c8d; font-style: italic; font-size: 14px;">
        ♔ White moves | ♚ Black moves
      </p>
    </div>
  </div>
</div>



<!-- My research interest includes neural machine translation and computer vision. I have published more than 100 papers at the top international AI conferences with total <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'>google scholar citations <strong><span id='total_cit'>260000+</span></strong></a> (You can also use google scholar badge <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>). -->


# 🔥 News
- 2025.05: Our paper **UniDB++: Fast Sampling of Unified Diffusion Bridge** is submitting.
- 2025.05: Our paper **UniDB: A Unified Diffusion Bridge Framework via Stochastic Optimal Control** accepted by **ICML 2025** as a **Spotlight**!🎉🎉
- 2025.04: Our paper **UniDB** won **Outstanding Paper Award** of ICLR 2025 DeLTa Workshop!🎉🎉
- 2025.04: Our paper **AffordDP: Generalizable Diffusion Policy with Transferable Affordance** accepted by **CVPR 2025**!🎉🎉

# 📝 Publications 

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Arxiv</div><img src='images/unidb++.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**UniDB++: Fast Sampling of Unified Diffusion Bridge**

 Mokai Pan, **Kaizhen Zhu**, Yuexin Ma, Yanwei Fu, Jingyi Yu, Jingya Wang, Ye Shi\*

[[**paper**]](https://arxiv.org/abs/2505.21528)
[[**code**]](https://github.com/2769433owo/UniDB-plusplus)

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICML 2025 Spotlight</div><img src='images/UniDB.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**UniDB: A Unified Diffusion Bridge Framework via Stochastic Optimal Control, <span style="color:red;">ICML 2025 Spotlight.</span>**


**Kaizhen Zhu\#**, Mokai Pan\#, Yuexin Ma, Yanwei Fu, Jingyi Yu, Jingya Wang, Ye Shi\*

[[**paper**]](https://arxiv.org/abs/2502.05749)
[[**project**]](https://unidb-soc.github.io/UniDB_page)
[[**code**]](https://github.com/UniDB-SOC/UniDB)

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">CVPR 2025</div><img src='images/AffordDP.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**AffordDP: Generalizable Diffusion Policy with Transferable Affordance,	CVPR 2025.**

Shijie Wu\#, Yihang Zhu\#, Yunao Huang, **Kaizhen Zhu**, Jiayuan Gu, Jingyi Yu, Ye Shi\*, Jingya Wang\*

[[**paper**]](https://arxiv.org/abs/2412.03142)
[[**project**]](https://afforddp.github.io/)
[[**code**]](https://github.com/SshiJwu/AffordDP)

</div>
</div>


# 🎖 Honors and Awards
- *2023.6* First Prize, Zhejiang Provincial Mathematics Competition 2023.
- *2022.11* National First Prize, China Undergraduate Mathematical Contest in Modeling (CUMCM) 2022.
- *2022.8* Second Prize, National Undergraduate Electronic Design Contest (NUEDC) 2022.

# 📖 Educations
<div class='paper-box'><div class='paper-box-image'><div><img src='images/skd.png' alt="sym" width="95%"></div></div>
<div class='paper-box-text' markdown="1">

<span style="font-size:18px;">**ShanghaiTech University**</span>

*2024.09 - now*

School of Information Science and Technology

Major: M.S. in **Computer Science**

MoE Key Laboratory of Intelligent Perception and Human Machine Collaboration, VDI Center, YesAI Lab
</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><img src='images/hangdian.jpg' alt="sym" width="95%"></div></div>
<div class='paper-box-text' markdown="1">

<span style="font-size:18px;">**Hangzhou Dianzi University**</span>

*2020.09 - 2024.06*

School of Electronic Information

Major: B.E. in **Electronic Science and Technology**

</div>
</div>

<!-- # 💬 Invited Talks
- *2021.06*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.03*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  \| [\[video\]](https://github.com/) -->

<!-- # 💻 Internships
- *2019.05 - 2020.02*, [Lorem](https://github.com/), China. -->
