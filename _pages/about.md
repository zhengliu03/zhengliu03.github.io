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

<head>
    <link rel="stylesheet" href="bootstrap.min.css">
    <style>
	:root {
	  --theme-color: #1F3A5F;
	  --venue-bg-color: rgb(108, 149, 181);
	}
	    
	g {
		color: #aaaaaa
	}

	 pt {
		color: var(--title-color);
		font-weight: 500;
	}

	 em {
		font-style: italic;
	}

	 venue {
		background-color: #1F3A5F;
		color: #ffffff;
		font-size: 70%;
		font-weight: bold;
		line-height: 170%;
		margin-right: 0.25em;
		width: 5em;
		display:inline-block;
		text-align: center;
		border-width: 0px;
		border-style: none;
		border-radius: 0.1rem;
		height: 1.7em;
		vertical-align:text-bottom;
		margin-bottom: 0.1em;
	}

	 venue1 {
		background-color: var(--venue-bg-color);
		color: #ffffff;
		font-size: 70%;
		font-weight: bold;
		line-height: 170%;
		margin-right: 0.25em;
		width: 5em;
		display:inline-block;
		text-align: center;
		border-width: 0px;
		border-style: none;
		border-radius: 0.1rem;
		height: 1.7em;
		vertical-align:text-bottom;
		margin-bottom: 0.1em;
	}
 
	.filter {
		color: var(--color);
		background-color: #fff;
		border: var(--border);
		border-style: solid;
		border-radius: 0.2rem;
		border-width: 1.5px;
		transition: all .3s;
		touch-action: manipulation;
		font-size: 80%;
		line-height: 120%;
	}
	
	.filter:focus {
		color: #171e29;
	}
	  
	  .filter:hover {
		border-color: var(--theme-color);
		color: white;
		background-color: var(--theme-color);
		fill: var(--theme-color);
	  }
	  
	  .filter:active {
		border-color: var(--theme-color);
		color: var(--theme-color);
		fill: var(--theme-color);
	  }
	  
	.button-59 {
	  align-items: center;
	  background-color: #fff;
	  border: 1px solid #dadada;
	  box-sizing: border-box;
	  color: #000000;
	  cursor: pointer;
	  display: inline-block;
	  fill: #000;
	  font-family: 'Nunito';
	  font-size: 0.7rem;
	  height: 1.1rem;
	  justify-content: center;
	  line-height: 1.3;
	  min-width: 60px;
	  outline: 0;
	  padding: 0 10px;
	  text-align: center;
	  text-decoration: none;
	  transition: color .3s, background-color .3s, border-color .3s;
	  user-select: none;
	  -webkit-user-select: none;
	  touch-action: manipulation;
	  margin-right: 0.2em;
	  border-radius: 0.2rem;
	}
	
	.button-59:hover {
	  border-color: var(--theme-color);
	  color: #fff;
	  fill: var(--theme-color);
	  background-color: var(--theme-color);
	  text-decoration: none;
	}
	
	.button-59:active {
	  border-color: var(--theme-color);
	  color: #fff;
	  fill: var(--theme-color);
	  background-color: var(--theme-color);
	}
	
	@media (min-width: 768px) {
	  .button-59 {
	    padding-left: 5px;
	    padding-right: 5px;
	  }
	}
    </style>
    <script>
        function checkFilter(type, li) {
            if (type == "All") {
                return true
            }
            else if (type == "First-authored") {
                res = li.getAttribute("first_authored")
                return res
            }
            else {
                cate = li.getAttribute("category")
                if (!cate) {
                    return false
                }
                items = cate.split(',')
                for (j = 0; j < items.length; j++) {
                    if (type.toUpperCase() == items[j].toUpperCase()) {
                        return true
                    }
                }
                return false
            }
        }

        function filterPub(type) {
            ul = document.getElementById("publications")
            li = ul.getElementsByTagName("li")
            for (i = 0; i < li.length; i++) {
                if (!checkFilter(type, li[i])) {
                    li[i].style.display = "none";
                }
                else {
                    li[i].style.display = ""
                }
            }
            bts = document.getElementsByClassName("filter")
            for (k = 0; k < bts.length; k++) {
                if (bts[k].textContent == type) {
                    bts[k].style.setProperty("--color", "#000")
                    bts[k].style.setProperty("--border", "#000")
                }
                else {
                    bts[k].style.setProperty("--color", "#a0a0a0")
                    bts[k].style.setProperty("--border", "#d3d3d3")
                }
            }
        }
    </script>
</head>

<span class='anchor' id='about-me'></span>

# 👤 Biography

I am a first-year master student at **[Peking University](https://cs.pku.edu.cn/)**, where I am supervised by [**Prof. Wentao Zhang**](https://zwt233.github.io/) and [**Prof. Bin Cui**](https://cuibinpku.github.io/) at the School of Computer Science. I obtained my B.S. degree from [**Nanjing University**](https://cs.nju.edu.cn/), ranking **1st out of 210** students (GPA: 4.62/5.0).

Previously, I had a wonderful time at [**OpenDataLab, Shanghai AI Laboratory**](https://opendatalab.com/), serving as a research intern supervised by [Dr. Conghui He](https://conghui.github.io/) and [Dr. Lijun Wu](https://apeterswu.github.io/). I contributed to the open-source project [**MinerU**](https://github.com/opendatalab/MinerU) (⭐ 54K+ GitHub Stars).

My research interests include **Vision-Language Models**, **Multimodal Reasoning**, **Document Parsing**, and **Synthetic Data**. Feel free to drop me an email for any form of communication or collaboration!

<div class="highlight-blocks">
  <div class="highlight-block">
    <h3>🔬 AI Researcher</h3>
    <ul>
      <li><strong>Vision-Language Models</strong>: Build efficient and deeply integrated multimodal architectures for cross-modal understanding.</li>
      <li><strong>Multimodal Reasoning</strong>: Enhance reasoning capabilities of VLMs through RL-based optimization and scalable data synthesis.</li>
      <li><strong>Document Parsing</strong>: OCR-free high-resolution document understanding with decoupled VLM pipelines.</li>
    </ul>
  </div>

  <div class="highlight-block">
    <h3>☎️ Contact Info</h3>
    <ul>
      <li><strong>Address:</strong> School of Computer Science, Peking University, Beijing, China</li>
      <li><strong>Email:</strong> <email>2501213330[AT]stu.pku.edu.cn</email></li>
      <li><strong>GitHub:</strong> <a href="https://github.com/starriver030515">starriver030515</a></li>
      <li><strong>WeChat:</strong> lz030515123 </li>
    </ul>
  </div>
</div>

# 🎓 Educations
- <img src="images/pku.png" style="width: 20px;height: auto;display: inline-block;vertical-align: middle"> **Peking University** (2025.09 - 2028.07) M.S. in Computer Science, supervised by Prof. Wentao Zhang and Prof. Bin Cui
- <img src="images/nju.jpg" style="width: 20px;height: auto;display: inline-block;vertical-align: middle"> **Nanjing University** (2021.09 - 2025.07) B.S. in Computer Science, GPA: 4.62/5.0, Rank: 1/210
<br>

# 🔥 News
<div id="news" class="w3-container w3-margin-top-2 w3-cursive">
	  <div style="height:200px; width:100%; overflow:auto;">
	    <p>[01.2026] 🎉 One paper <strong>FLARE</strong> was accepted by <strong>ICLR 2026</strong>!</p>
	    <p>[09.2025] 🎓 I joined <strong>Peking University</strong> and started pursuing my master's degree.</p>
      <p>[07.2025] 🎉 One paper <strong>SynthVLM</strong> was accepted by <strong>ACM MM 2025</strong>!</p>
      <p>[10.2024] 🏆 Awarded <strong>National Scholarship</strong> (Top 1), Nanjing University.</p>
	    <p>[09.2024] 🎉 Started research internship at <strong>Shanghai AI Lab</strong>.</p>
	    <p>[05.2024] 🏆 <strong>Gold Award</strong>, 20th Programming Competition, Nanjing University.</p>
	    <p>[10.2023] 🏆 Awarded <strong>GuoXieBirong Scholarship</strong> (Top 2), Nanjing University.</p>
	  </div>
	</div>

<br>

# 📝 Publications

_(\* denotes equal contribution)_

## 📒 Selected Publications

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICLR'2026</div><img src='images/flare.png' alt="FLARE" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**FLARE: Fully Integration of Vision-Language Representations for Deep Cross-Modal Understanding**

- **Zheng Liu**, Mengjie Liu, Jingzhou Chen, Jingwei Xu, Bin Cui, Conghui He, Wentao Zhang
- International Conference on Learning Representations, 2026.
- [[Paper]](https://arxiv.org/pdf/2504.09925) [[Code, 100+ Stars🌟]](https://github.com/starriver030515/FLARE)
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ACMMM'2025</div><img src='images/synthvlm.png' alt="SynthVLM" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**SynthVLM: Towards High-Quality and Efficient Synthesis of Image-Caption Datasets for Vision-Language Models**

- **Zheng Liu\***, Hao Liang\*, Bozhou Li, Wentao Xiong, Chong Chen, Conghui He, Wentao Zhang, Bin Cui
- ACM International Conference on Multimedia, 2025.
- [[Paper]](https://arxiv.org/pdf/2407.20756) [[Code, 100+ Stars🌟]](https://github.com/starriver030515/SynthVLM)
</div>
</div>

## 📄 Preprints & Under Review

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ACL'2026</div><img src='images/hapo.png' alt="HAPO" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**From Uniform to Heterogeneous: Tailoring Policy Optimization to Every Token's Nature**

- **Zheng Liu\***, Mengjie Liu\*, Siwei Wen, Mengzhang Cai, Bin Cui, Conghui He, Wentao Zhang
- Under review at ACL 2026.
- [[Paper]](https://arxiv.org/pdf/2509.16591) [[Code]](https://github.com/starriver030515/HAPO)
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ACL'2026</div><img src='images/chartverse.png' alt="ChartVerse" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**ChartVerse: Scaling Chart Reasoning via Reliable Programmatic Synthesis from Scratch**

- **Zheng Liu\***, Honglin Lin\*, Chonghan Qin, ..., Bin Cui, Conghui He, Lijun Wu, Wentao Zhang
- Under review at ACL 2026.
- [[Paper]](https://arxiv.org/pdf/2505.14671?) [[Homepage]](https://chartverse.github.io/)
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ACL'2026</div><img src='images/sisbench.png' alt="SISBench" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Scientific Image Synthesis: Benchmarking, Methodologies, and Downstream Utility**
- Honglin Lin\*, **Zheng Liu\***, Chonghan Qin\*, Qizhi Pei, Yu Li, Zhanping Zhong, ..., Conghui He, Lijun Wu. 
- Under review at ACL 2026.
- [[Paper]](https://arxiv.org/pdf/2601.17027) [[Homepage]](https://scigenbench.github.io)
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ECCV'2026</div><img src='images/mmfinereason.png' alt="MMFineReason" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**MMFineReason: Closing the Multimodal Reasoning Gap via Open Data-Centric Methods**

- Honglin Lin\*, **Zheng Liu\***, Yun Zhu\*, Chonghan Qin, Xiaoran Shang, Conghui He, Wentao Zhang, Lijun Wu
- Under review at ECCV 2026.
- [[Paper]](https://arxiv.org/pdf/2601.21821) [[Homepage]](https://mmfinereason.github.io)
</div>
</div>

<br>

# 💻 Projects

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">MinerU</div><img src='images/mineru.png' alt="MinerU" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**MinerU2.5: A Decoupled Vision-Language Model for Efficient High-Resolution Document Parsing**

- Junbo Niu\*, **Zheng Liu\***, Zhuangcheng Gu\*, Bin Wang\*, ..., Bowen Zhou, Dahua Lin, Wentao Zhang, Conghui He
- [[Paper]](https://arxiv.org/pdf/2509.22186) [[GitHub, 54K+ Stars🌟]](https://github.com/opendatalab/MinerU)
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">OpenDataArena</div><img src='images/opendataarena.png' alt="OpenDataArena" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**OpenDataArena: A Fair and Open Arena for Benchmarking Post-Training Dataset Value**

- Mengzhang Cai\*, Xin Gao\*, Yu Li\*, Honglin Lin\*, **Zheng Liu\***, ..., Dahua Lin, Conghui He, Lijun Wu.
- [[Paper]](https://arxiv.org/abs/2512.14051) [[Homepage]](https://opendataarena.github.io/)
</div>
</div>

<br>

# 🏢 Experience
- *2025.09 - 2026.02*, **Research Intern**, [OpenDataLab, Shanghai AI Laboratory](https://opendatalab.com/), supervised by [Dr. Lijun Wu](https://apeterswu.github.io/). Working on Multimodal LLM Reasoning, Scientific Image Understanding, Reasoning Data Synthesis.
- *2024.09 - 2025.08*, **Research Intern**, [OpenDataLab, Shanghai AI Laboratory](https://opendatalab.com/), supervised by [Dr. Conghui He](https://conghui.github.io/). Working on Multimodal LLM Understanding, OCR-Free Visual Understanding.

<br>

# 🥇 Honors and Awards
- *(2024)*: &nbsp;**National Scholarship**, Nanjing University (Top 1)
- *(2024)*: &nbsp;**Gold Award**, 20th Programming Competition, Nanjing University
- *(2023)*: &nbsp;**GuoXieBirong Scholarship**, Nanjing University (Top 2)

<br>

# 🛠️ Skills
- **Programming**: C, C++, Python
- **Frameworks & Tools**: [PyTorch](https://github.com/pytorch/pytorch), [Transformers](https://github.com/huggingface/transformers), [LLaVA](https://github.com/haotian-liu/LLaVA), [Verl](https://github.com/verl-project/verl), [LLaMA-Factory](https://github.com/hiyouga/LlamaFactory)

# 😄 Miscellaneous
<!-- <div class="highlight-blocks">
  <div class="highlight-block">
    <h3>❤️ Family</h3>
    <ul>
      <img src="images/qiaoqiao.jpg" alt="family Image" style="display: block; margin: auto; max-width: 100%; height: auto;">
     <br>
	    <li>I have a beautiful girlfriend, <a href='https://scholar.google.com/citations?user=G_BypiwAAAAJ&hl=zh-CN&oi=ao'>Ziqi Qiao</a>, who is also a Ph.D. student at Peking University. We also own an adorable cat 🐱 named QiuQiu. He brings us tremendous fun and happiness.</li>
    </ul>
  </div>
  
  <div class="highlight-block">
    <h3>🧑‍🤝‍🧑 Friends</h3>
    <ul>
	<img src="images/friends.png" alt="friend Image" style="display: block; margin: auto; max-width: 100%; height: auto;">
      <br>
	    <li>Here are some of my closest academic friends: <a href='https://liujiaming1996.github.io/'>Jiaming Liu</a>, <a href='https://scholar.google.com/citations?user=SgeV4NkAAAAJ&hl=zh-CN&oi=ao'>Yulin Luo</a>, <a href='https://gumpest.github.io/'>Yuan Zhang</a>, and Gaole Dai from PKU; <a href='https://scholar.google.com/citations?hl=zh-CN&user=Vl1X_-sAAAAJ'>Xiaowei Chi</a> from HKUST; <a href='https://wuchenrui.github.io/'>Chenrui Wu</a> from ZJU&SFU; <a href='https://yilijin.github.io/'>Yili Jin</a> from McGill.</li>
    </ul>
  </div>
  
  <div class="highlight-block">
    <h3>😄 Hobbies</h3>
    <ul>
	<img src="images/football_new.png" alt="hobby Image" style="display: block; margin: auto; max-width: 100%; height: auto;">
      <br>
	    <li>I am a crazy basketball 🏀 & football ⚽️ fan. I enjoy the games of Kevin Durant 🕷️ and Kyrie Irving 🧙. I also wholeheartedly pledge my allegiance to Chelsea Football Club, KTBFFH! 💙</li>
    </ul>
  </div>
</div>

<br> -->

<!-- <div style="text-align: center;"> -->
<div style="width: 20%; position:relative; left:40%">
  <script type="text/javascript" id="clstr_globe" src="//clustrmaps.com/globe.js?d=TexC6zB_7AOUKNMMshe4U4igIY-rca8pyS5kiQ7N6C8"></script>
    <!-- 地图小部件代码结束 -->
</div>