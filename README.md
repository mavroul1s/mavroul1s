# Nikolaos Mavros

Fifth-year Electrical and Computer Engineering student at the **University of Thessaly**, Volos.
I work on deep learning for remote sensing and computer vision, with a side interest in the
mathematics underneath it — gradient flow, optimisation geometry, and why training runs behave
the way they do.

The thing I care about most in a project is whether the result survives an audit. Most of the
repositories below report mean ± standard deviation over repeated seeds, publish the failure
cases alongside the wins, and state plainly what the method does *not* do.

---

## Current work

**[DeepFire-Forecaster](https://github.com/mavroul1s/DeepFire-Forecaster)** (BurnBench) — wildfire
remote sensing on the TS-SatFire dataset. Manuscript under review at *MDPI Sensors*.

Three contributions:

- **SpaSE-UNet3D**, a spatial squeeze-and-excitation 3D UNet (~32.9M params, spatial-only
  `(1,3,3)` convolutions, SE attention at every encoder stage, ASPP bottleneck, deep supervision).
- A **label-quality audit** of every fire in every split of the source dataset. Substantial
  missing labels were found and documented; training on audited data raised active-fire recall
  from ~0.80 to 0.86.
- The **burned-area label encoding**, which the dataset paper never specified. Band 8 finite
  values are Julian-day or perimeter-ID codes, not a threshold — a prerequisite for any future
  work on that task.

| Task | Model | Test F1 | IoU 
|---|---|---|---|---|
| Active Fire | SpaSE-UNet3D (TS=2) | **0.855** | 0.746  
| Active Fire | SpaSE-UNet3D (TS=1) | 0.854 | 0.745 
| Fire Progression | SpaSE-UNet3D (TS=2) | **0.424** | 0.269 

Every notebook is self-contained and reproduces on a Kaggle T4 inside the 12-hour session limit.

---

## Selected projects

| Project | What it is |
|---|---|
| **[NEOW / neo_tracker](https://github.com/mavroul1s/neo_tracker)** | Heliocentric solar system viewer driven by NASA's near-Earth object feed. Real orbital elements propagated through a Kepler solver verified against independent ground truth — Earth's perihelion to 0.98329 AU, equinox and solstice solar longitudes within 0.4°, convergence to machine precision through e = 0.99. One HTML file, no build step, English and Ελληνικά. |
| **[GridSense](https://github.com/mavroul1s/gridsense)** | Polyglot-persistence power grid platform: Cassandra, Neo4j, MongoDB, PostgreSQL and Redis behind a single FastAPI gateway, 14 endpoints, one `docker compose up`. Each store is chosen for what it is actually good at — time series, topology graphs, schemaless metadata, ACID billing, cache and pub/sub. |
| **[Neural Collaborative Filtering](https://github.com/mavroul1s/ncf-assignment)** | Reproduction of He et al. (WWW 2017) on MovieLens-100K, 10 seeds per experiment. A response-distilled student matches the teacher's HR@10 (0.655 vs 0.649) with 50.7% fewer parameters; feature-based distillation underperforms. MLP depth and pretraining show no mean benefit at this dataset size, contradicting the paper's ML-1M result. |
| **[vit-gradient-flow](https://github.com/mavroul1s/vit-gradient-flow)** | Analytic Jacobian of the self-attention mechanism derived by hand, then verified numerically with `ForwardDiff.jl`. Compares orthogonal against Xavier initialisation on Jacobian conditioning and saliency. Written in Julia. |
| **[Galaxy-Morphology-CNN](https://github.com/mavroul1s/Galaxy-Morphology-CNN)** | Custom VGG-style network predicting 37 probabilistic morphology features on Galaxy Zoo. 0.109 RMSE on blind test data with ~2.6M parameters, through a five-phase ablation pipeline rather than a single lucky run. |
| **[KinetiCore](https://github.com/mavroul1s/KinetiCore)** | Real-time bare-hand computer vision with OpenCV and MediaPipe. Gesture recognition and biometric mapping, entirely local — no network, no API. |

## Coursework

Full write-ups, reports and figures live in each repository.

- **[ECE328 — Information Retrieval](https://github.com/mavroul1s/ir-assignment-2026)** · PageRank and HITS from the eigenvalue side, Zipf's law on Gutenberg text, BPR recommendation over Last.FM and ML-1M
- **[ECE418 — Neuro-Fuzzy Computing](https://github.com/mavroul1s/ECE418-Coursework)** · LMS and ADALINE performance surfaces, conjugate gradient, Adadelta on rotated loss landscapes, convolution as Toeplitz matrix multiplication, GRU/LSTM on autoregressive series
- **[ECE443 — Speech and Audio Processing](https://github.com/mavroul1s/ECE443-Coursework)** · narrowband and wideband spectrograms, F0 and formant estimation, LPC analysis-synthesis with robot and whisper reconstruction
- **[ECE457 — Computer Vision](https://github.com/mavroul1s/ECE457-Coursework)** · Otsu thresholding, spatial filter comparison by PSNR, Sobel/Prewitt/Laplacian/Canny, frequency-domain edge detection
- **[GMM Music Genre Recognition](https://github.com/mavroul1s/GMM-Music-Genre-Recognition)** · MFCC features, k-means initialisation, Expectation-Maximization written from scratch rather than called from a toolbox

---

## Tools

**Daily** — Python, PyTorch, NumPy, MATLAB
**Comfortable** — Julia, FastAPI, Docker, OpenCV, TensorFlow, Git
**Data** — Cassandra, Neo4j, MongoDB, PostgreSQL, Redis
**Domains** — remote sensing and geospatial rasters, 3D segmentation, recommender systems, DSP and speech, information retrieval

---

## Background

**Certifications** — Qualcomm Wireless Academy 5G Introductory Level (2024) · MathWorks Machine Learning Onramp (2025), MATLAB Fundamentals (2025), MATLAB Onramp (2024) · ECCE Certificate of Competency in English, B2, University of Michigan

**Conferences** — 3rd Emerging Tech Conference: Edge Intelligence, Volos 2024 · ECESCON 14, Volos 2023

---

## Elsewhere

[LinkedIn](https://www.linkedin.com/in/nikos-mavros-37a94a259/) · [Kaggle](https://www.kaggle.com/nmavros) · [Instagram](https://www.instagram.com/mavroul1s/) · [nick.black.4416@gmail.com](mailto:nick.black.4416@gmail.com)

Open to research collaborations and internships in machine learning and computer vision.
