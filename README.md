<div align="center">

<!-- ══════════════════ ANIMATED HEADER ══════════════════ -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:003300,100:00ff41&height=200&section=header&text=NIKOS%20MAVROS&fontSize=52&fontColor=00ff41&fontAlignY=38&desc=ECE%20Undergrad%20%7C%20Deep%20Learning%20%7C%20Earth%20Observation%20%7C%20Volos%2C%20Greece%20%F0%9F%87%AC%F0%9F%87%B7&descAlignY=58&descSize=14&descColor=8b949e&animation=fadeIn" />

<!-- ══════════════════ TYPING BANNER ══════════════════ -->
[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=15&duration=2800&pause=900&color=00FF41&center=true&vCenter=true&multiline=false&width=700&lines=%3E+Building+NovHyT+%E2%80%94+CNN-Transformer+for+wildfire+prediction+%F0%9F%94%A5%F0%9F%9B%B0%EF%B8%8F;%3E+Galaxy+Zoo+%7C+VGG-CNN+%7C+RMSE+0.109+on+blind+test+%F0%9F%8C%8C;%3E+Computer+Vision+%7C+Signal+Processing+%7C+ViT+Research+%F0%9F%94%AC;%3E+ECE+%40+University+of+Thessaly+%7C+Volos%2C+Greece+%F0%9F%87%AC%F0%9F%87%B7;%3E+always+training%2C+always+learning...+%E2%96%88)](https://git.io/typing-svg)

</div>

---

## `> cat about.py`

```python
class NikosMavros:
    name       = "Nikos Mavros"
    handle     = "mavroul1s"
    degree     = "Electrical & Computer Engineering (ECE)"
    university = "University of Thessaly 🎓  —  Volos, Greece 🇬🇷"
    
    research   = {
        "flagship"    : "NovHyT — Spatiotemporal Fire Prediction via CNN-Transformer 🔥🛰️",
        "domains"     : ["Deep Learning", "Computer Vision", "Earth Observation",
                         "Signal Processing", "Audio ML", "Astrophysical ML"],
        "best_result" : "Galaxy Zoo — 0.109 RMSE on blind test 🌌",
        "approach"    : "Attention mechanisms meet satellite imagery",
    }
    
    currently  = "ECE452 · Applying ViT temporal attention to VIIRS wildfire data"
    kaggle     = "kaggle.com/nmavros"
    vibe       = "Building models that explain the Earth — one epoch at a time 🚀"
```

---

## `> ls -la ./projects --verbose`

<table>
<tr>
<td width="50%" valign="top">

### 🔥 [DeepFire-Forecaster](https://github.com/mavroul1s/DeepFire-Forecaster)

[![ECE452](https://img.shields.io/badge/ECE452-Research-00ff41?style=flat-square&logo=academia&logoColor=black&labelColor=0d1117)](https://github.com/mavroul1s/DeepFire-Forecaster)
[![PyTorch](https://img.shields.io/badge/PyTorch-Hybrid_CNN--ViT-EE4C2C?style=flat-square&logo=pytorch&logoColor=white&labelColor=0d1117)](https://github.com/mavroul1s/DeepFire-Forecaster)

**NovHyT** — A hybrid CNN-Transformer architecture for spatiotemporal wildfire spread prediction.

- **Spatial Encoder** · CNN extracts VIIRS thermal + ESRI LULC features
- **Spatiotemporal Transformer** · ViT variant with temporal attention over day sequences
- **Temporal Attention Pooling** · Dynamically weights the most critical time steps
- **Generative Decoder** · Transposed convolutions reconstruct fire probability maps
- **Masked Focal-Dice Loss** · Custom objective for severe class imbalance

`Python` `PyTorch` `ViT` `VIIRS` `Geospatial` `83 commits`

</td>
<td width="50%" valign="top">

### 🌌 [Galaxy-Morphology-CNN](https://github.com/mavroul1s/Galaxy-Morphology-CNN)

[![RMSE](https://img.shields.io/badge/Blind_Test_RMSE-0.109-a855f7?style=flat-square&labelColor=0d1117)](https://github.com/mavroul1s/Galaxy-Morphology-CNN)
[![Galaxy Zoo](https://img.shields.io/badge/Galaxy_Zoo-Challenge-7c3aed?style=flat-square&labelColor=0d1117)](https://github.com/mavroul1s/Galaxy-Morphology-CNN)

Custom **VGG-CNN** implementation for astrophysical morphology classification.

- 5-phase experimental pipeline (preprocessing → training → ablation → eval)
- **0.109 RMSE** on blind holdout test set
- Galaxy Zoo dataset · multi-class morphology prediction
- Custom augmentation + class weighting strategies

`Python` `CNN` `VGG` `Astrophysics` `Kaggle`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 👁️ [ECE457 — Computer Vision](https://github.com/mavroul1s/ECE457-Coursework)

[![CV](https://img.shields.io/badge/Computer_Vision-From_Scratch-38bdf8?style=flat-square&labelColor=0d1117)](https://github.com/mavroul1s/ECE457-Coursework)

Python CV pipeline built from the ground up — no black boxes.

- Custom image **binarization** algorithms
- Noise reduction with **PSNR analysis**
- Frequency-domain **edge detection** (Fourier / filter design)
- Full pipeline from raw pixel to processed output

`Python` `OpenCV` `NumPy` `Signal Processing` `Fourier`

</td>
<td width="50%" valign="top">

### 🧠 [ECE418 — Deep Learning](https://github.com/mavroul1s/ECE418-Coursework)

[![DL](https://img.shields.io/badge/Deep_Learning-Fall_2025-F37626?style=flat-square&labelColor=0d1117)](https://github.com/mavroul1s/ECE418-Coursework)

Neural networks built from first principles — Fall 2025.

- **CNNs & RNNs** implemented and trained from scratch
- **Optimization algorithms** — gradient descent variants, adaptive methods
- **Fuzzy Logic systems** for soft decision making
- Jupyter-based experiments with full analysis

`Python` `PyTorch` `CNNs` `RNNs` `Fuzzy Logic`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🎵 [GMM-Music-Genre-Recognition](https://github.com/mavroul1s/GMM-Music-Genre-Recognition)

[![MATLAB](https://img.shields.io/badge/MATLAB-GMM+MFCC-e02020?style=flat-square&labelColor=0d1117)](https://github.com/mavroul1s/GMM-Music-Genre-Recognition)

Audio ML from scratch — no deep learning, pure probabilistic modelling.

- **MFCC feature extraction** from raw audio
- **Gaussian Mixture Models** for genre classification
- **Custom EM algorithm** — implemented without toolboxes
- Full MATLAB pipeline from waveform to decision

`MATLAB` `GMM` `MFCC` `EM Algorithm` `Audio ML`

</td>
<td width="50%" valign="top">

### 🔬 [vit-gradient-flow](https://github.com/mavroul1s/vit-gradient-flow)

[![ViT](https://img.shields.io/badge/Vision_Transformer-Gradient_Analysis-a855f7?style=flat-square&labelColor=0d1117)](https://github.com/mavroul1s/vit-gradient-flow)

Research into the internal dynamics of Vision Transformers.

- Probing **gradient flow** through attention layers
- Stability analysis across transformer depths
- Connects to NovHyT architecture choices
- Experimental Jupyter notebooks

`Python` `ViT` `Transformers` `Interpretability`

</td>
</tr>
</table>

---

## `> tech_stack --verbose`

<div align="center">

**// Languages**

[![Skills](https://skillicons.dev/icons?i=python,matlab&theme=dark)](https://skillicons.dev)

**// Deep Learning & ML**

[![Skills](https://skillicons.dev/icons?i=pytorch,tensorflow&theme=dark)](https://skillicons.dev)

**// Tools & Platforms**

[![Skills](https://skillicons.dev/icons?i=git,linux,jupyter,github&theme=dark)](https://skillicons.dev)

</div>

<div align="center">

![Python](https://img.shields.io/badge/Python-0d1117?style=for-the-badge&logo=python&logoColor=00FF41)
![MATLAB](https://img.shields.io/badge/MATLAB-0d1117?style=for-the-badge&logo=mathworks&logoColor=EE4C2C)
![PyTorch](https://img.shields.io/badge/PyTorch-0d1117?style=for-the-badge&logo=pytorch&logoColor=EE4C2C)
![TensorFlow](https://img.shields.io/badge/TensorFlow-0d1117?style=for-the-badge&logo=tensorflow&logoColor=FF6F00)
![scikit-learn](https://img.shields.io/badge/sklearn-0d1117?style=for-the-badge&logo=scikitlearn&logoColor=F7931E)
![OpenCV](https://img.shields.io/badge/OpenCV-0d1117?style=for-the-badge&logo=opencv&logoColor=5C3EE8)
![NumPy](https://img.shields.io/badge/NumPy-0d1117?style=for-the-badge&logo=numpy&logoColor=4FC3F7)
![Pandas](https://img.shields.io/badge/Pandas-0d1117?style=for-the-badge&logo=pandas&logoColor=150458)
![Jupyter](https://img.shields.io/badge/Jupyter-0d1117?style=for-the-badge&logo=jupyter&logoColor=F37626)
![Kaggle](https://img.shields.io/badge/Kaggle-0d1117?style=for-the-badge&logo=kaggle&logoColor=20BEFF)
![Git](https://img.shields.io/badge/Git-0d1117?style=for-the-badge&logo=git&logoColor=F05032)
![Linux](https://img.shields.io/badge/Linux-0d1117?style=for-the-badge&logo=linux&logoColor=FCC624)

</div>

---

## `> git log --stats mavroul1s`

<div align="center">

<img height="165em" src="https://github-readme-stats.vercel.app/api?username=mavroul1s&show_icons=true&count_private=true&bg_color=0d1117&border_color=00ff41&title_color=00ff41&icon_color=00ff41&text_color=c9d1d9&ring_color=00ff41" />
<img height="165em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=mavroul1s&layout=compact&bg_color=0d1117&border_color=00ff41&title_color=00ff41&text_color=c9d1d9&hide_border=false" />

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=mavroul1s&theme=terminal&background=0d1117&border=00FF41&ring=00FF41&fire=FF4500&currStreakLabel=00FF41&sideLabels=8b949e&dates=8b949e)](https://git.io/streak-stats)

</div>

<div align="center">

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=mavroul1s&bg_color=0d1117&color=00ff41&line=00ff41&point=ffffff&area=true&hide_border=false&border_color=00ff41)](https://github.com/ashutosh00710/github-readme-activity-graph)

</div>

<div align="center">

[![Trophies](https://github-profile-trophy.vercel.app/?username=mavroul1s&theme=matrix&no-frame=false&no-bg=true&margin-w=8&column=6)](https://github.com/ryo-ma/github-profile-trophy)

</div>

---

## `> cat current_mission.log`

```
╔══════════════════════════════════════════════════════════╗
║  STATUS: ACTIVE                                          ║
╠══════════════════════════════════════════════════════════╣
║                                                          ║
║  [🔥] NovHyT — ECE452 Research                          ║
║       CNN-Transformer hybrid for wildfire prediction     ║
║       VIIRS thermal · ESRI LULC · Masked Focal-Dice Loss ║
║                                                          ║
║  [🌌] Galaxy Morphology · 0.109 RMSE (blind test)        ║
║       VGG-CNN · 5-phase experimental pipeline            ║
║                                                          ║
║  [🔬] ViT Gradient Flow — attention layer analysis       ║
║       Understanding how transformers see the world       ║
║                                                          ║
╚══════════════════════════════════════════════════════════╝
```

---

## `> ping --all-channels`

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-mavroul1s-0d1117?style=for-the-badge&logo=github&logoColor=white)](https://github.com/mavroul1s)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Nikos_Mavros-0d1117?style=for-the-badge&logo=linkedin&logoColor=0A66C2)](https://www.linkedin.com/in/nikos-mavros-37a94a259/)
[![Kaggle](https://img.shields.io/badge/Kaggle-nmavros-0d1117?style=for-the-badge&logo=kaggle&logoColor=20BEFF)](https://www.kaggle.com/nmavros)
[![Instagram](https://img.shields.io/badge/Instagram-mavroul1s-0d1117?style=for-the-badge&logo=instagram&logoColor=E4405F)](https://www.instagram.com/mavroul1s/)

</div>

---

<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:00ff41,50:003300,100:0d1117&height=100&section=footer&text=ECE%20%40%20UTH%20%C2%B7%20always%20training%2C%20always%20learning&fontSize=13&fontColor=8b949e&fontAlignY=65&animation=fadeIn" />

![Visitor Count](https://visitor-badge.laobi.icu/badge?page_id=mavroul1s.mavroul1s&left_color=black&right_color=green&left_text=visitors)

</div>
