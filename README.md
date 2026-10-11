# Computer-Vision-Basics

Interactive, browser-based demos for learning the fundamentals of computer vision.
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


