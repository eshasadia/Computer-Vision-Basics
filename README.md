# Computer-Vision-Basics

Interactive, browser-based demos for learning the fundamentals of computer vision.

## Demos

| Demo | What it teaches | Link |
|---|---|---|
| Image Normalization | How pixel values are rescaled before training, and how normalization layers work inside networks | [▶](https://claude.ai/artifact/2iqVCoAcJE1hgGuPr7G1fz) |
| ⛰️ Optimizers | How SGD, Adam and the newest optimizers (Lion, Muon, SOAP and more) find the lowest loss | [▶](https://claude.ai/artifact/88JpAr9p9rTgMGad9FZ5Fq) |

---

## Demo: Image Normalization

**[▶ Open the live demo](https://claude.ai/artifact/2iqVCoAcJE1hgGuPr7G1fz)**

See what normalization does to an image, one pixel at a time. Pick a photo, pick a method, then point at any pixel to see the exact arithmetic behind the result.

### What you'll learn

**Pixel normalization methods**

| Method | What it does |
|---|---|
| Scale to 0–1 | Divides every value by 255, so the numbers change but the picture doesn't |
| Min–max | Stretches the darkest value to 0 and the brightest to 1 |
| Percentile clip | Like min–max, but ignores extreme outliers first |
| Z-score | Centers values on 0 with a spread of 1 |
| ImageNet mean/std | The fixed normalization pretrained models expect |
| Histogram equalization | Spreads pixels evenly across all brightness levels |

**Normalization layers in neural networks**

Batch norm, layer norm, instance norm and group norm, shown on a batch of 4 images so you can see exactly which values get averaged together.

### Features

- **Pixel inspector:** point at or tap any pixel to see the before and after values with the full calculation.
- **Live histograms and statistics:** watch the min, max, average and spread change for each color channel.
- **Three explanation levels:** switch between *new to this*, *comfortable with math* and *training models*.
- **Problem images:** fog, a dark night scene, a color cast and a well-exposed photo show where each method helps and where it fails.
- **Use your own photo:** it's processed in your browser and never uploaded anywhere.

---

## Demo: Optimizers

**[▶ Open the live demo](https://claude.ai/artifact/88JpAr9p9rTgMGad9FZ5Fq)**

Watch optimizers race downhill on the same loss landscape, then see why the newest ones treat weights as matrices instead of separate numbers.

### What you'll learn

**Optimizers in the 2-D race**

| Optimizer | Year | Big idea |
|---|---|---|
| SGD | 1951 | Step straight downhill |
| Momentum | 1964 | Build up speed in consistent directions |
| Nesterov | 1983 | Look ahead before stepping, to overshoot less |
| AdaGrad | 2011 | A separate, shrinking step size for each direction |
| RMSprop | 2012 | Step sizes based on recent gradients only |
| Adam | 2014 | Momentum plus per-direction step sizes |
| AdamW | 2017 | Adam with weight decay done right |
| Lion | 2023 | Step by the sign of the momentum only |
| Sophia | 2023 | Uses curvature, with clipped steps |
| Schedule-Free | 2024 | Averaging replaces learning-rate decay |
| ADOPT | 2024 | Reordered Adam that always converges |
| AdEMAMix | 2024 | Mixes a fast and a very slow memory |
| Cautious | 2024 | Skips directions where momentum disagrees with the gradient |

**Matrix-aware optimizers**

Muon, Shampoo and SOAP, shown on a 16×16 weight matrix to explain why they keep learning when SGD and Adam stall.

### Features

- **Four terrains:** a narrow valley, a curved "banana" valley, a saddle point and a bumpy surface with many local minima.
- **Live optimizer internals:** watch the momentum, step-size memory and every update as numbers, step by step.
- **Controls to experiment:** change the learning rate, add noisy gradients like real mini-batches, or click the map to pick a new starting point.
- **Three explanation levels:** the same *new to this*, *comfortable with math* and *training models* switch as the normalization demo.
- **What the research says:** a table of optimizers published from 2023 to 2026, plus links to the original papers.

---

## 🚀 Run it yourself

Each demo is a single self-contained HTML file. To use it offline, download it and open it in any modern browser.
