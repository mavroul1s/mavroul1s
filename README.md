<div align="center">

```
 ███╗   ███╗ █████╗ ██╗   ██╗██████╗  ██████╗ ██╗   ██╗██╗      ██╗███████╗
 ████╗ ████║██╔══██╗██║   ██║██╔══██╗██╔═══██╗██║   ██║██║     ███║██╔════╝
 ██╔████╔██║███████║██║   ██║██████╔╝██║   ██║██║   ██║██║     ╚██║███████╗
 ██║╚██╔╝██║██╔══██║╚██╗ ██╔╝██╔══██╗██║   ██║██║   ██║██║      ██║╚════██║
 ██║ ╚═╝ ██║██║  ██║ ╚████╔╝ ██║  ██║╚██████╔╝╚██████╔╝███████╗ ██║███████║
 ╚═╝     ╚═╝╚═╝  ╚═╝  ╚═══╝  ╚═╝  ╚═╝ ╚═════╝  ╚═════╝ ╚══════╝ ╚═╝╚══════╝
```

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=20&duration=3200&pause=1000&color=10B981&center=true&vCenter=true&width=720&lines=ECE+undergrad+at+the+University+of+Thessaly;computer+vision+%C2%B7+deep+learning+%C2%B7+touchdesigner;building+things+that+see%2C+listen%2C+and+learn.)](https://git.io/typing-svg)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nikos-mavros-37a94a259/)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=flat-square&logo=instagram&logoColor=white)](https://www.instagram.com/mavroul1s/)
[![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=flat-square&logo=kaggle&logoColor=white)](https://www.kaggle.com/nmavros)

</div>

---

## About

```yaml
name        : Nikos Mavros
handle      : mavroul1s
role        : Electrical & Computer Engineering — Undergraduate
university  : University of Thessaly, Volos, Greece
fields      : computer vision · deep learning · generative networks
interests   : CNN / ViT architectures, gradient flow, wildfire
              forecasting, audio DSP, live visuals & installations
stack       : python · pytorch · tensorflow · opencv · mediapipe
              matlab · julia · touchdesigner
```

---

## Stack

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" />
  <img src="https://img.shields.io/badge/MediaPipe-00B0FF?style=for-the-badge&logo=google&logoColor=white" />
  <img src="https://img.shields.io/badge/MATLAB-0076A8?style=for-the-badge&logo=mathworks&logoColor=white" />
  <img src="https://img.shields.io/badge/Julia-9558B2?style=for-the-badge&logo=julia&logoColor=white" />
  <img src="https://img.shields.io/badge/TouchDesigner-111?style=for-the-badge" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" />
  <img src="https://img.shields.io/badge/LaTeX-008080?style=for-the-badge&logo=latex&logoColor=white" />
</p>

---

```
   ┌─────────────────────────────────────────────────────────────────┐
   │                    F E A T U R E D   W O R K                    │
   └─────────────────────────────────────────────────────────────────┘
```

### [KinetiCore](https://github.com/mavroul1s/KinetiCore)

```
                        _ _ _ _
                       | | | | |
                       | | | | |      bare hands.
                       | | | | |      no mouse.
                     __| | | | |__    no keyboard.
                    |             |
                    |   palm.map  |
                    |_____________|
                           |
                         /_|_\
                     ───'     '───
                        [ cam ]
```

An experimental sandbox for low-latency computer vision — bare-hand spatial manipulation and biometric mapping. Standalone Python experiments: hand-gesture control, half-face tracking, interactive molecule manipulation, index-cube spatial input, screen mirroring, custom dithering filters. Just a camera and the graph.

```
  [cam] ──▶ MediaPipe ──▶ gesture graph ──▶ render loop
    │                                           │
    └── biometric map ◀── dithering/FX ◀────────┘
```

`python`  ·  `opencv`  ·  `mediapipe`  ·  `real-time-cv`

---

### [DeepFire-Forecaster](https://github.com/mavroul1s/DeepFire-Forecaster) — *NovHyT*

```
                 )             (
              (    )     )         )
          )   (       )      (         )
            )     )     (        )
          (   (     )       )        )
            )    )    (    (     )
          (     )    )    )   (
         _|_____|_____|_____|_____|_
        /                           \
       /    wildfire   forecaster    \
      /_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _\
         VIIRS · LULC · day_t-n..t
```

Spatiotemporal fire-spread prediction via hybrid **CNN–Transformer** on multi-spectral satellite imagery. CNN spatial encoder + custom Spatiotemporal Transformer with temporal attention + generative decoder on transposed convolutions. Trained with a **Masked Focal–Dice Loss** engineered for the severe class imbalance of wildfire data. Academic project under ECE452 (Applied Mathematics).

```
  VIIRS thermal  ─┐
  ESRI LULC      ─┼─▶ [CNN encoder] ─▶ [Spatiotemporal ViT] ─▶ [Temporal Attn] ─▶ fire map
  day_t-n..t     ─┘
```

`pytorch`  ·  `vision-transformer`  ·  `remote-sensing`  ·  `research`

---

### [Galaxy-Morphology-CNN](https://github.com/mavroul1s/Galaxy-Morphology-CNN)

```
            .     .  *    .   *      .  .       *    .
      .   *    .         .       .     .       .  .
         .   .       _.-""""-._      .        .   .
          .      _.-'  *  .  * '-._      .      .     *
      .    *   /  .     .      .  \   .     .       .
               | *   .   .    *   |      *     .   .
          .    \ .   *       .  ./   .      .
            .   '-.__  *  ___.-'    *      .     *
         .         '""""""'    *      .      .
               .    *     .     *   .     *    .
```

Custom **VGG-style CNN** on the Galaxy Zoo dataset — 37 probabilistic morphological labels per galaxy. Lightweight (~2.6M params), hitting **0.109 RMSE on the blind Kaggle test set** of 79,975 galaxies. Transparent 5-phase experimental pipeline isolating architectural decisions, interpretability via learned-filter visualization (edge detectors + center-surround blobs). IEEE-formatted report included.

```
  ┌──────────────┬──────────────┬──────────────┬───────────────┐
  │   Results    │ Val RMSE     │ Test RMSE    │  Inference    │
  ├──────────────┼──────────────┼──────────────┼───────────────┤
  │    value     │   0.104      │   0.109      │   57.3 ms     │
  └──────────────┴──────────────┴──────────────┴───────────────┘
```

`tensorflow`  ·  `cnn`  ·  `astro-ml`  ·  `kaggle`

---

### [vit-gradient-flow](https://github.com/mavroul1s/vit-gradient-flow)

```
        (o)       (o)       (o)       (o)
       /|\       /|\       /|\       /|\
      / | \     / | \     / | \     / | \
     o  o  o   o  o  o   o  o  o   o  o  o
      \ | /     \ | /     \ | /     \ | /
       \|/       \|/       \|/       \|/
        x─────────x─────────x─────────x
           ∂L/∂W   .   .   .  jacobian
        ─────────────────────────────────
                 self-attention
```

Investigating gradient flow and sensitivity in **Vision Transformers** — formally, via matrix calculus. Derives the explicit Jacobian of the self-attention mechanism, then empirically validates in **Julia** using automatic differentiation. Compares **Orthogonal** vs **Xavier/Glorot** initialization for Jacobian conditioning on MNIST-as-patches. Research project under ECE452.

```
  ∂L/∂W  :  orthogonal_init ( Wᵀ W = I )  vs  xavier/glorot
  verify :  julia + ForwardDiff.jl  ⟺  hand-derived jacobians
  output :  saliency maps · condition numbers · flow plots
```

`julia`  ·  `forwarddiff`  ·  `vit`  ·  `matrix-calculus`

---

### [GMM-Music-Genre-Recognition](https://github.com/mavroul1s/GMM-Music-Genre-Recognition)

```
          ___           ___           ___
         /   \         /   \         /   \
        | BLU |       | REG |       | CLS |
         \___/         \___/         \___/
           |             |             |
      ╭────┴─────────────┴─────────────┴────╮
      │ ▁▂▃▅▇▆▅▃▂▁▁▂▃▅▇▆▅▃▂▁▁▂▃▅▇▆▅▃▂▁     │  mfcc stream
      ╰─────────────────────────────────────╯
                        |
                      [ EM ]     hand-rolled, no toolbox
                        |
                      GMM ──▶ MAP ──▶ decision
```

Blues · Reggae · Classical — distinguished at **100% accuracy** using hand-rolled EM + MFCC. Not a toolbox wrapper: Expectation–Maximization manually implemented for GMM training, K-Means for robust parameter initialization, MAP classification. ECE443 Speech & Audio Processing.

```
  wav ──▶ 20ms windows ──▶ MFCC ──▶ CMS + energy-drop ──▶ K-Means init ──▶ EM ──▶ GMM ──▶ MAP
```

`matlab`  ·  `gmm`  ·  `em-algorithm`  ·  `mfcc`  ·  `speech-processing`

---

```
   ┌─────────────────────────────────────────────────────────────────┐
   │                      C O U R S E W O R K                        │
   └─────────────────────────────────────────────────────────────────┘
```

### [ECE418-Coursework](https://github.com/mavroul1s/ECE418-Coursework) — *Neuro-Fuzzy Computing*

```
         input        hidden        output
          o  ─────▶    o   ─────▶    o
          o  ─────▶    o   ─────▶    o
          o  ─────▶    o   ─────▶    o
             w₁           w₂
         ───────── backpropagation ─────────▶
```

ADALINE / LMS, backpropagation from scratch, conjugate gradient, Adadelta optimizer, Toeplitz-matrix convolution, RNN / LSTM time-series prediction. `MATLAB` · `Python`

---

### [ECE443-Coursework](https://github.com/mavroul1s/ECE443-Coursework) — *Speech & Audio Processing*

```
   amp │    ▂▃▅▇▆▅▃▂      narrowband  ━━━━━━━━━━━
       │   ▁       ▁     wideband    ━ ━ ━ ━ ━ ━
       │ ▁           ▁▂▃▅▇▆▅▃▂▁
       └──────────────────────────▶ t
         add   ·   cats   ·   apa   ·   robot   ·   whisper
```

STFT spectrograms (narrowband / wideband F0 analysis), time-domain segmentation, and a deep dive into **Linear Predictive Coding** — source/filter separation, Levinson-Durbin recursion, synthetic impulse-train excitation for robot-voice synthesis, white-noise excitation for whispers. Plus a presentation on the history of electronic synthesizers (Theremin → Moog → DX7). `MATLAB`

---

### [ECE457-Coursework](https://github.com/mavroul1s/ECE457-Coursework) — *Computer Vision*

```
    ┌──────┐     ┌──────┐     ┌──────┐     ┌──────┐
    │ img  │ ──▶  blur    ──▶  grad  ──▶   edge 
    └──────┘     └──────┘     └──────┘     └──────┘
                  Gaussian     Sobel /      Canny
                  Median       Prewitt      output
```

Otsu binarization, spatial filters (Gaussian / Median → PSNR 26.31 dB), Sobel / Prewitt / Laplacian / Canny edge detection, FFT high-pass filtering in the frequency domain. `Python` · `OpenCV`

---

```
   ┌─────────────────────────────────────────────────────────────────┐
   │                         S T A T S                               │
   └─────────────────────────────────────────────────────────────────┘
```

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=mavroul1s&show_icons=true&theme=transparent&hide_border=true&title_color=10B981&icon_color=10B981" height="160" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=mavroul1s&layout=compact&theme=transparent&hide_border=true&title_color=10B981" height="160" />

<img src="https://github-readme-streak-stats.herokuapp.com/?user=mavroul1s&theme=transparent&hide_border=true&ring=10B981&fire=10B981&currStreakLabel=10B981" height="160" />

</div>

---

<div align="center">

*<sub>"the gradient is just a direction — the interesting thing is what happens along the way."</sub>*

</div>
