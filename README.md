# Nikos Mavros — Personal Brief

Context document for building a personal portfolio website. Everything here is verified from
his GitHub repositories, certificates, and profile. Do not invent metrics, dates, or claims
beyond what appears below — see **Guardrails** at the end.

---

## 1. Identity

| Field | Value |
|---|---|
| Name | Nikos Mavros (Νίκος Μαύρος) — formally Nikolaos Mavros |
| Role | Fifth-year student, Electrical and Computer Engineering |
| Institution | University of Thessaly (UTh), Dept. of Electrical and Computer Engineering, Volos, Greece |
| Focus | Deep learning, remote sensing, computer vision, and the applied mathematics beneath them |
| Languages | Greek (native), English (ECCE B2, University of Michigan) |
| Status | Open to research collaborations and internships in ML/CV |

## 2. Contact and links

| Channel | URL |
|---|---|
| Email | nick.black.4416@gmail.com |
| GitHub | https://github.com/mavroul1s |
| LinkedIn | https://www.linkedin.com/in/nikos-mavros-37a94a259/ |
| Kaggle | https://www.kaggle.com/nmavros |
| Instagram | https://www.instagram.com/mavroul1s/ |

GitHub: 16 public repositories. Primary project has 5 stars.

## 3. Positioning

The through-line across his work is **verification over presentation**. Repeatedly, across
unrelated domains, the interesting contribution is not the model — it is auditing the data
everyone else trusted, or checking a solver against independent ground truth, or reporting
mean ± standard deviation over ten seeds when one run would have looked better. His own
README for NEOW states plainly what the project is *not*, and DeepFire's headline finding is
a dataset flaw rather than an architecture.

Useful hero lines (pick or adapt, do not stack all of them):

- "Deep learning for remote sensing. A result that survives an audit, or it does not count."
- "ECE student at the University of Thessaly. I build models, then try to break them."
- "Wildfire segmentation, orbital mechanics, and the gradients in between."

## 4. Flagship project

### DeepFire-Forecaster (BurnBench)
`https://github.com/mavroul1s/DeepFire-Forecaster` · Jupyter/PyTorch · 156 commits · MIT

Wildfire remote sensing on the TS-SatFire dataset (Zhao et al., *Scientific Data*, 2025).
**Manuscript under review at MDPI *Sensors*** — not yet accepted or published.

Three tasks: active fire (AF) detection, burned area (BA) mapping, fire progression (FP) prediction.

**Architecture — SpaSE-UNet3D** (Spatial Squeeze-and-Excitation 3D UNet):
- Encoder channels [64, 128, 256, 512], ~32.9M parameters
- ResBlock3D with spatial-only (1,3,3) convolutions — no temporal mixing across days
- Squeeze-and-Excitation channel attention at every encoder stage
- ASPP bottleneck, dilation rates [1, 6, 12]
- Deep supervision on decoder outputs; Dice + Focal combined loss; OneCycleLR, 80–100 epochs
- One config switch (`TS_LENGTH = 1` or `2`) for clean ablation

**Results:**

| Task | Model | Test F1 | Test IoU |
|---|---|---|---|
| Active Fire | SpaSE-UNet3D (TS=2) | 0.855 | 0.746 |
| Active Fire | SpaSE-UNet3D (TS=1) | 0.854 | 0.745 |
| Fire Progression | SpaSE-UNet3D (TS=2) | 0.424 | 0.269 |

Active fire precision 0.848, recall 0.861; optimal inference threshold 0.20–0.22; test set of
15 verified fires.

**Contributions beyond the model:**
1. **Label-quality audit** across all three tasks and every split. The source paper documents
   no label completeness; substantial missing labels were found (all-NaN label bands) and
   excluded. Training on audited data raised AF recall from ~0.80 to 0.86.
2. **BA label encoding discovery.** The paper never specified the encoding. Band 8 finite
   values are Julian-day or perimeter-ID codes (range 2,119–908,660), so the correct label
   extraction is a finiteness mask, not a value threshold. BA modelling was deliberately
   deferred and the finding published as a standalone data-quality result.

Everything reproduces on a Kaggle T4 inside the 12-hour session limit, no local setup.

## 5. Other projects

**NEOW / neo_tracker** — `https://github.com/mavroul1s/neo_tracker` — three.js, single HTML file
Heliocentric solar system viewer built on NASA's NeoWs near-Earth object feed. Propagates eight
planets, fifteen moons, and every tracked NEO from published osculating elements through a
Kepler solver. Verified against independent ground truth: Earth's perihelion 0.98329 AU and
aphelion 1.01671 AU, equinox and solstice solar longitudes within 0.4°, convergence to machine
precision through e = 0.99, Earth computed twice by unrelated routes agreeing to 44,000 km and
59 arcseconds. Publishes its own scale factors rather than faking scale, shows JPL orbit
uncertainty codes, and explicitly corrects the "potentially hazardous means close now"
misconception. Bilingual English/Ελληνικά. No build step, no dependencies but three.js.
*This is the most visually striking project and the best candidate for a live embed or demo.*

**GridSense** — `https://github.com/mavroul1s/gridsense` — FastAPI, Docker Compose
Polyglot-persistence smart grid analytics prototype. Cassandra (time-series sensor readings),
Neo4j (network topology, fault-impact and restoration-path queries), MongoDB (equipment
metadata), PostgreSQL (ACID billing), Redis (dashboard cache, pub/sub alerts), behind a single
REST gateway. 14 endpoints, one `docker compose up`.

**NCF Reproduction** — `https://github.com/mavroul1s/ncf-assignment` — PyTorch (ECE480)
Reproduction of Neural Collaborative Filtering (He et al., WWW 2017) on MovieLens-100K. Every
experiment repeated 10 times with independent seeds, all results mean ± std. NeuMF best:
HR@10 0.649 ± 0.011, NDCG@10 0.390 ± 0.007 at 107,761 params. A response-based knowledge
distillation student reaches HR@10 0.655 ± 0.010 at 53,177 params — matching the teacher on
50.7% fewer parameters. Feature-based (FitNets-style) distillation underperforms at 0.582.
MLP depth and GMF+MLP pretraining show no mean benefit at this dataset size, contradicting
the paper's MovieLens-1M finding.

**vit-gradient-flow** — `https://github.com/mavroul1s/vit-gradient-flow` — Julia (ECE452)
Derives the explicit Jacobian of the self-attention mechanism using matrix calculus, then
verifies it numerically with `ForwardDiff.jl`. Compares orthogonal initialisation (WᵀW = I)
against Xavier/Glorot on Jacobian conditioning and feature saliency, using MNIST as sequential
patches. 52 commits.

**Galaxy-Morphology-CNN** — `https://github.com/mavroul1s/Galaxy-Morphology-CNN` — TensorFlow
Custom VGG-style CNN predicting 37 probabilistic morphological features on Galaxy Zoo.
0.109 RMSE on blind test data at ~2.6M parameters, 64×64 input, through a five-phase
experimental pipeline isolating each architectural decision. Includes an IEEE-formatted report.

**KinetiCore** — `https://github.com/mavroul1s/KinetiCore` — Python, OpenCV, MediaPipe
Real-time bare-hand computer vision sandbox. Webcam gesture and face tracking, biometric
mapping, standalone demo scripts. Runs entirely locally — no network, no API.

## 6. Coursework repositories

- **ECE328 Information Retrieval** (`ir-assignment-2026`) — PageRank and HITS via eigenvalue
  analysis, Zipf's law on Project Gutenberg text, BPR recommendation on Last.FM and MovieLens-1M.
  10 repetitions with mean ± std, seeded, committed results for rebuild without re-running.
- **ECE418 Neuro-Fuzzy Computing** — optimisation landscapes, ADALINE and LMS weight
  trajectories over MSE performance surfaces, matrix-form backpropagation, conjugate gradient,
  Adadelta on standard vs rotated loss surfaces, convolution as Toeplitz matrix multiplication
  with benchmarking, GRU/LSTM on autoregressive series. MATLAB and Python.
- **ECE443 Speech and Audio Processing** — narrowband/wideband spectrograms, F0 and formant
  estimation, LPC analysis-synthesis producing robot and whisper voices. MATLAB.
- **ECE457 Computer Vision** — Otsu thresholding, spatial filter comparison by PSNR (Gaussian
  26.31 dB vs Box 25.80 dB), Sobel/Prewitt/Laplacian/Canny by edge density, frequency-domain
  edge detection. Python/NumPy/OpenCV.
- **GMM Music Genre Recognition** — MFCC features with cepstral mean subtraction, k-means
  initialisation, Expectation-Maximization implemented from scratch rather than called from a
  toolbox. 100% accuracy on a three-genre test set (blues, reggae, classical). MATLAB.

## 7. Skills

```
Languages     Python, MATLAB, Julia, JavaScript
ML            PyTorch, TensorFlow, scikit-learn; 3D segmentation, CNNs, ViTs,
              knowledge distillation, recommender systems
Data/backend  FastAPI, Docker Compose, Cassandra, Neo4j, MongoDB, PostgreSQL, Redis
CV/DSP        OpenCV, MediaPipe, MFCC/LPC, spectral analysis, classical filtering
Other         three.js, LaTeX, Git, Kaggle GPU workflows, rasterio/geospatial rasters
Domains       wildfire remote sensing, orbital mechanics, astronomy imaging,
              information retrieval, speech and audio
```

## 8. Credentials

- Qualcomm Wireless Academy — 5G Introductory-Level Certification (Dec 2024)
- MathWorks — Machine Learning Onramp (Dec 2025)
- MathWorks — MATLAB Fundamentals (Mar 2025)
- MathWorks — MATLAB Onramp (Mar 2024)
- ECCE Certificate of Competency in English, level B2 — Michigan Language Assessment (2019)

Conferences attended:
- 3rd Emerging Tech Conference: Edge Intelligence — UTh, Volos, Oct 2024
- ECESCON 14 — University of Thessaly, Volos, Apr 2023

## 9. Voice and design direction

**Voice.** Plain, precise, technical, unhurried. States limits as readily as results. No
marketing adjectives, no "passionate about," no exclamation marks. Short declarative sentences.
His own writing does this well — "Not an ephemeris, a risk assessment, or novel research" —
and the site should sound like the same person wrote it.

**Hard constraint: no emojis anywhere.**

**Aesthetic.** Retro-futuristic. CRT terminal, HUD readouts, ASCII, scanlines, wireframe and
perspective grids, monospace type. Palette taken from his own NEOW project:

```
background   #04060b        near-black
surface      #0b1620        panel fill
primary      #35e0f0        cyan, links and active state
primary-lo   #7defff        bright cyan, headings
accent       #ffb347        amber, warnings and secondary data
alert        #ff3d5a        red, glitch layers and hazard states
muted        #3f7d8c        dim cyan, labels and metadata
grid         #12718c        rules and grid lines
```

Typography: monospace throughout, or monospace headings against a neutral sans body. Motion
should be restrained and mechanical — scanline sweeps, typing reveals, blinking cursors, data
pulses travelling along rules, occasional RGB glitch bursts. No bounce, no fade-up-on-scroll,
no parallax.

**Suggested structure:** single page, sections in this order — hero (animated ASCII name,
status rail), current work (DeepFire, given its own block with the results table), selected
projects (cards with real metrics, not adjectives), archive/coursework (compact list),
toolchain, credentials, contact. A live embed of NEOW would carry the whole site if it can be
made to work.

**Existing assets:** an animated HUD banner SVG (`header.svg`) and animated divider SVG
(`divider.svg`) already exist and can be reused or restyled. Project screenshots, training
curves, per-fire prediction maps, spectrograms, and feature-space scatter plots live inside
the respective repositories and can be linked from `raw.githubusercontent.com`.

## 10. Guardrails

- The *Sensors* manuscript is **under review**, not published. Never write "published,"
  "peer-reviewed," or invent a DOI, volume, or citation.
- Every number in this document is taken from his repositories. Do not round, inflate, or
  generate new benchmarks. If a figure is not here, leave it out.
- The 100% GMM accuracy is on a small three-genre coursework test set. Present it as such.
- Coursework repositories are coursework. Do not describe them as research or products.
- He is a student, not a graduate. Do not assign job titles, employers, or years of experience.
- Do not fabricate testimonials, client logos, or download/user counts.
