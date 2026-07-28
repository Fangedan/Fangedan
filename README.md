<h1 align="center">Hi there! 👋 I'm Andrew Lin</h1>
<p align="center">
🎓 CS @ UT Austin | AI & Machine Learning Research | Full Stack Developer | Competitive Programming | Open to Internships
</p>

<p align="center">
  <a href="https://fangedan.github.io"><img src="https://img.shields.io/badge/🗺️_PORTFOLIO-fangedan.github.io-FF8E3C?style=for-the-badge&labelColor=113560" alt="Portfolio"></a>
  <a href="https://www.linkedin.com/in/andrew-lin-466798328/"><img src="https://img.shields.io/badge/LinkedIn-Andrew_Lin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:alin257274@gmail.com"><img src="https://img.shields.io/badge/Email-alin257274@gmail.com-113560?style=for-the-badge" alt="Email"></a>
</p>

<p align="center">
  <b>🚗 My portfolio has an Explore Mode — drive a probe around a blueprint of my work: <a href="https://fangedan.github.io">fangedan.github.io</a></b>
</p>

---

## 🔹 About Me  
- 🖥 **Computer Science Student** at UT Austin  
- 🔬 Passionate about **AI, computer vision, cybersecurity, and competitive programming**  
- 🎭 **Diverse Interests**: Theater, piano, web development, and tutoring  
- 🌐 **Bilingual**: English & Chinese  

---

## 🚀 Experience & Projects  

### 🔬 **Research & Internships**

- **UTD Machine Learning Research Internship — Prof. Xinfang Jin (2026)**
  - Built a **Python preprocessing pipeline** (`preprocess_dream3d.py`) to convert DREAM.3D PNG exports into 64×64×64 BMP voxel stacks with measured volume fractions, specific surface areas, and label files — replacing an existing MATLAB workflow
  - Extended the preprocessor with production-ready flags: `--multi` (batch-processes multiple DREAM.3D stacks sequentially), `--tile-xy` (spatially tiles large 500×500×500+ volumes into ~49 structures per z-slab instead of downsampling), `--dry-run`, and `--preview`; switched downsampling to block-center sampling to keep categorical phase labels exact
  - **Validated the full pipeline end-to-end on 101 real DREAM.3D microstructures** (first real-data run): generated structures reproduced the real material's **Ni connectivity (S=0.905) and pore connectivity (S=0.872)** in the OK band on the Yu et al. similarity scale — and Ni connectivity was reproduced *without ever being a training target*
  - Diagnosed two bugs causing **pore-phase collapse** in the WGAN-GP (a severed SSA-loss gradient path and a volume-fraction loss computed on softmax instead of argmax), then designed and added a **differentiable connectivity loss** (3D-convolution isolation penalty + face-hinge percolation term) — fixing pore collapse on synthetic data (similarity **0.48→0.90** and **0.59→0.86**, FAIL→OK); a controlled real-data **ablation** then showed the term overshoots where a phase already percolates, isolating *when* a connectivity loss helps versus hurts
  - Built **`4_CNNCT`**, a new analysis module measuring phase percolation, active triple-phase-boundary density, tortuosity (`taufactor`), and Yu et al. distribution-similarity S-values, with a 23-test suite
  - Automated a manual ParaView workflow with **`0_PRV/paraview_slice_export.py`** (`pvpython`), converting DREAM.3D `.vtk` volumes into slice-image stacks — shipped with a ground-truth test harness that caught four silent label-corrupting bugs before handoff
  - Wrote a standalone test suite (`test_preprocess.py`) covering four end-to-end scenarios — resize mode, tile-XY mode, multi-folder mode, and pixel-level phase round-trip — all passing on Windows
  - Built an [interactive 3D SOC electrode simulation](https://fangedan.github.io/GAN-PH) visualizing the electrochemical process with directional particle flows, deployed via GitHub Pages
  - 🔗 **[GAN-PH Repository](https://github.com/Fangedan/GAN-PH)**

- **[UTD Summer Research Internship Program](https://docs.google.com/presentation/d/1SvF_jI_fieUf8khbQ-3sPhu5if0kxnPZ9Vb_lg_QxB4/edit?usp=sharing) (2024)**
  - Studied active speaker detection in **Dr. Yapeng Tian's Computer Vision Lab**  
  - Optimized training techniques (**VGG16, transfer learning, weight freezing**) to maximize **mAP results**  
  - Built a [live in-browser active speaker detection demo](https://fangedan.github.io/CVMC) — per-face lip tracking correlated with microphone energy, deployed via GitHub Pages
  - 🔗 **[CVMC Repository](https://github.com/Fangedan/CVMC)**

- **UTD CAST STEM Bridge Research Lab (2023)**
  - Researched **hybrid manufacturing & CAD modeling** under Dr. Wei Li  
  - Designed, coded, and simulated **milling paths for medical and automation applications**  

### 💻 **Technical & Leadership Roles**

- **President, Merlin Mavens Mentors (CS Tutoring Club)**
  - Guided underclassmen through CS concepts and debugging challenges  
  - Strengthened **mentorship & leadership** skills through weekly tutoring sessions  

- **Computer Science Clubs @ Allen HS**
  - 🏆 **Competitive Coding** (Swift & Python)  
  - 🔐 **Cybersecurity Club** (Competed in **AFA CyberPatriot Nationals**)  
  - 🌐 **CS Honor Society**  

### 🛠 **Notable Projects**

🔹 **[🗺️ Blueprint Portfolio](https://fangedan.github.io)** – This profile, but **drivable**: a zero-dependency interactive portfolio with a canvas-based Explore Mode, custom drift physics, and an animated percolation background — [source on GitHub](https://github.com/Fangedan/Fangedan.github.io)

🔹 **[GAN-PH — SOC Electrode Microstructure Generation](https://github.com/Fangedan/GAN-PH)** – Conditional Wasserstein GAN pipeline for generating 3D porous electrode microstructures, validated on real DREAM.3D data with persistent homology and triple-phase-boundary transport analysis, plus an [interactive simulation](https://fangedan.github.io/GAN-PH)

🔹 **[CS314 Recursion](https://github.com/Fangedan/CS314-Recursion)** – **Recursive problem-solving** in Java, tackling complex algorithmic challenges  

🔹 **[CVMC — Active Speaker Detection](https://github.com/Fangedan/CVMC)** – Two-stream **audio-visual CNN** determining which visible face is speaking, trained on AVA Active Speaker format data — built during the UTD Computer Vision Lab internship and showcased through Freetail Hackers, with a [live in-browser demo](https://fangedan.github.io/CVMC)  

🔹 **[Girlfriend's Website](https://github.com/Fangedan/silly)** – **Silly** website I made to ask my girlfriend to be my girlfriend  

---

## 🛠 Skills & Certifications  
- 💡 **Languages**: Java, Swift, Python, HTML/CSS  
- 🤖 **ML/AI**: PyTorch, CNNs, GANs, persistent homology, scikit-learn, OpenCV  
- ☁ **Certifications**: **AWS Certified Cloud Practitioner**  
- 🛠 **Technologies**: GitHub, Linux, Windows, Cisco, Cybersecurity Tools  

---

## 📫 Let's Connect!  
- 📧 **Email**: alin257274@gmail.com  
- 🌍 **Portfolio**: **[fangedan.github.io](https://fangedan.github.io)** ← drive around it
- 💼 **[LinkedIn](https://www.linkedin.com/in/andrew-lin-466798328/)**
