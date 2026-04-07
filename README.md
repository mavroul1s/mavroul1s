<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a0a0a,50:003300,100:00ff41&height=130&section=header&text=mavroul1s&fontSize=52&fontColor=00ff41&animation=fadeIn&fontAlignY=68&desc=signal%20through%20noise&descSize=14&descAlignY=86&descColor=33ff66" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Share+Tech+Mono&size=16&duration=2200&pause=900&color=00FF41&center=true&vCenter=true&width=650&lines=computer+vision+%2F%2F+deep+learning;image+segmentation+%2F%2F+blob+tracking;datamoshing+%2F%2F+gradient+flow;ViT+%2F%2F+CNN+%2F%2F+GMM+%2F%2F+MFCC;ECE+undergrad+%40+university+of+thessaly" alt="Typing SVG" />

</div>

---

```
 ▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄
 █                                                        █
 █   ███╗   ███╗ █████╗ ██╗   ██╗██████╗  ██████╗ ██╗   █
 █   ████╗ ████║██╔══██╗██║   ██║██╔══██╗██╔═══██╗██║   █
 █   ██╔████╔██║███████║██║   ██║██████╔╝██║   ██║██║   █
 █   ██║╚██╔╝██║██╔══██║╚██╗ ██╔╝██╔══██╗██║   ██║██║   █
 █   ██║ ╚═╝ ██║██║  ██║ ╚████╔╝ ██║  ██║╚██████╔╝███████╗
 █   ╚═╝     ╚═╝╚═╝  ╚═╝  ╚═══╝  ╚═╝  ╚═╝ ╚═════╝╚══════╝
 █                                                        █
 ▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀
  [ ECE undergrad :: University of Thessaly :: Volos, GR ]
```

---

<div align="center">

```
// > whoami
```

</div>

```
  ┌─────────────────────────────────────────────────────────┐
  │  nick   :  mavroul1s                                    │
  │  field  :  electrical & computer engineering            │
  │  loc    :  volos, greece                                │
  │  status :  undergraduate                                │
  │                                                         │
  │  research vectors:                                      │
  │    -> computer vision                                   │
  │    -> deep learning / image segmentation                │
  │    -> blob tracking                                     │
  │    -> datamoshing / glitch aesthetics                   │
  │    -> gradient flow in transformers                     │
  └─────────────────────────────────────────────────────────┘
```

---

<div align="center">

```
// > scan --mode=deep --target=interests
```

</div>

```
                     COMPUTER VISION

            .  '  .  '  .  '  .  '  .  '  .
         '        ,--.                       '
        .        /    \    .  .  .           .
       '        | LENS |  _/\/\/\_           '
        .        \    /  |        |          .
         '        `--'   |________|         '
            .  '  .  '  .  '  .  '  .  '  .

    [ pixel space ]---[ feature space ]---[ latent ]
         raw       conv/attn blocks      repr.

  segment  ->  track  ->  classify  ->  generate
```

---

```
                      GRADIENT FLOW

    input  ->  [ attention ]  ->  [ MLP ]  ->  output
               /           \
    Q  K  V   /             \   residual
     \_______|               |_________/
      softmax(QK^T/sqrt(d))V
                 ||
         jacobian analysis
                 ||
     cond(J) < epsilon  =>  stable
     cond(J) > threshold =>  VANISH / EXPLODE
```

---

<div align="center">

```
// > ls -la ./projects
```

</div>

| repo | what it does | stack |
|---|---|---|
| [DeepFire-Forecaster](https://github.com/mavroul1s/DeepFire-Forecaster) | wildfire prediction pipeline | Python / DL |
| [Galaxy-Morphology-CNN](https://github.com/mavroul1s/Galaxy-Morphology-CNN) | VGG-CNN on Galaxy Zoo — 0.109 RMSE blind test | Python / PyTorch |
| [vit-gradient-flow](https://github.com/mavroul1s/vit-gradient-flow) | jacobian analysis + orthogonal init in ViTs | Julia / ForwardDiff |
| [ECE457-Coursework](https://github.com/mavroul1s/ECE457-Coursework) | binarization, noise reduction (PSNR), frequency-domain edge detection | Python / CV |
| [ECE418-Coursework](https://github.com/mavroul1s/ECE418-Coursework) | CNNs, RNNs, fuzzy logic, optimization algorithms | Python / Jupyter |
| [GMM-Music-Genre-Recognition](https://github.com/mavroul1s/GMM-Music-Genre-Recognition) | GMM + MFCC audio classifier with custom EM | MATLAB |

---

<div align="center">

```
// > cat ./stack.txt
```

</div>

```
  ╔══════════════════════════════════════════════════════╗
  ║                                                      ║
  ║  languages  ::  python  julia  matlab  bash          ║
  ║  dl libs    ::  pytorch  keras  sklearn              ║
  ║  cv tools   ::  opencv  pillow  scikit-image         ║
  ║  math       ::  numpy  scipy  forwarddiff.jl         ║
  ║  env        ::  jupyter  latex  git                  ║
  ║                                                      ║
  ╚══════════════════════════════════════════════════════╝
```

---

<div align="center">

```
// > ping --visual --glitch
```

</div>

```
  b l o b   t r a c k i n g

  frame_0001  ....O......................
  frame_0002  .....O.....................
  frame_0003  ......O....................
  frame_0004  .....░▓█▓░.................   <- detection
  frame_0005  ......░▓█▓░................
  frame_0006  .......▓█▓.................
  frame_0007  ........O..................   <- re-id


  d a t a m o s h i n g

  i-frame  | BBBBBBBBBBBBBBBBBBBBBBB |
  p-frame  | BB▒▒▒░░░###BBB###░░░▒▒ |   <- corrupt
  p-frame  | ▒▒░░░###░░░▒▒▒░░░BBB▒▒ |   <- smear
  p-frame  | ░░▒▒BBB░░░### BBB░░░▒▒ |   <- bleed
  i-frame  | BBBBBBBBBBBBBBBBBBBBBBB |
```

---

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=mavroul1s&show_icons=true&theme=chartreuse-dark&hide_border=true&bg_color=0d0d0d&title_color=00ff41&icon_color=00cc33&text_color=aaffaa" height="150"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=mavroul1s&layout=compact&theme=chartreuse-dark&hide_border=true&bg_color=0d0d0d&title_color=00ff41&text_color=aaffaa" height="150"/>

</div>

---

```
  ┌──────────────────────────────────────────────────────┐
  │                                                      │
  │          find me :                                   │
  │                                                      │
  │    kaggle   ->  kaggle.com/nmavros                   │
  │    linkedin ->  linkedin.com/in/nikos-mavros-37a94a259│
  │    insta    ->  instagram.com/mavroul1s              │
  │                                                      │
  └──────────────────────────────────────────────────────┘
```

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00ff41,50:003300,100:0a0a0a&height=90&section=footer" width="100%"/>

</div>
