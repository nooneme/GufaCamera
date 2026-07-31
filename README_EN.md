<p align="center">
  <a href="README.md">简体中文</a> &nbsp;|&nbsp; <b>English</b>
</p>

<h1 align="center">📷 Classic Camera</h1>

<p align="center">
  <em>Full RAW Pipeline · WYSIWYG · LUT Learning System</em>
</p>

---

**Classic Camera** is a minimalist, fully-manual camera app built for creation. It skips the manufacturer's image processing entirely and drives the sensor's **RAW data** directly, returning the purest optical quality to you. Every parameter adjustment is applied to RAW data in real time — what you see is what you get.

## 📱 App Preview

<p align="center">
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053222.jpg" width="19%" alt="Screenshot 1"/>
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053243.jpg" width="19%" alt="Screenshot 2"/>
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053247.jpg" width="19%" alt="Screenshot 3"/>
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053359.jpg" width="19%" alt="Screenshot 4"/>
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053407.jpg" width="19%" alt="Screenshot 5"/>
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053417.jpg" width="19%" alt="Screenshot 6"/>
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053635.jpg" width="19%" alt="Screenshot 7"/>
</p>

## ✨ Key Features

### 1. Full RAW Pipeline · Pure Optical Quality

Completely bypasses the vendor ISP (Image Signal Processor). Starting from the Bayer mosaic data, the entire chain — denoising, white balance, CFA reordering, and tone mapping — is handled by the app itself. **No aggressive sharpening, no over-smoothing — just the light the sensor actually captured.**

### 2. Live RAW Preview · What You See Is What You Get

The viewfinder isn't a preview stream from the vendor ISP — full of algorithms and inconsistent exposure — it's a **real-time, full render of the RAW data**. The light, color, and detail you see on screen are exactly what the shutter delivers. No more guessing how the final image will look from experience.

### 3. Parameters Applied to RAW · Skip the Post-Processing Hassle

Exposure, white balance, color temperature, tone curves, film simulation — every adjustment is **applied directly to the RAW pixels** and shown live in the preview. Finish your creative tuning on the spot, without the tedious "shoot first, edit later" workflow.

### 4. Built-in LUT Learning System · Learn Any Filter With Just 2 Photos

The app ships with a **LUT learning engine**:

- **Learn any filter with as few as 2 photos** (one source image + one with the target filter applied)
- Comes with **35+** high-quality film simulation filters (Fujifilm, Ricoh, Leica, Pentax, Lumix, and more)
- The engine reports coverage / training & validation error visualization so you can assess the quality of what it learned

### 5. Radical Minimalism

No ads, no notifications, no accounts, no community bloat. Just the core ability to shoot: **clean, focused, and fully offline.**

> **Compatibility note:** Currently only tested on the **Samsung Galaxy S23 Ultra**; behavior on other devices may differ.

## 🖼 Sample Gallery

All shots are quick casual captures, straight out of the camera — my photography skills are limited, these are for demonstration only.

<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260722_175518_6.3mm.jpg" width="100%" alt="Sample 1"/></td>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260725_191039_6.3mm.jpg" width="100%" alt="Sample 2"/></td>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_151337_6.3mm.jpg" width="100%" alt="Sample 3"/></td>
  </tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_154935_6.3mm.jpg" width="100%" alt="Sample 4"/></td>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_155744_7.9mm.jpg" width="100%" alt="Sample 5"/></td>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_160432_6.3mm.jpg" width="100%" alt="Sample 6"/></td>
  </tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_163909_6.3mm.jpg" width="100%" alt="Sample 7"/></td>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_170852_7.9mm.jpg" width="100%" alt="Sample 8"/></td>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_171301_6.3mm.jpg" width="100%" alt="Sample 9"/></td>
  </tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260731_220015_6.3mm.jpg" width="100%" alt="Sample 10"/></td>
    <td colspan="2">&nbsp;</td>
  </tr>
</table>

## 🛠 Tech Stack

| Layer | Technology |
| --- | --- |
| Languages | Kotlin · C/C++ (NDK) |
| Camera | Camera2 API, full manual control (exposure / focus / WB / multi-lens) |
| Rendering | OpenGL ES real-time RAW rendering pipeline |
| Native | CMake + JNI, C++ for tone curves / LUT generation, etc. |
| Platform | minSdk 26 · targetSdk 36, arm64-v8a / x86_64 |

## 📂 Project Layout (excerpt)

```
app/src/main/java/com/classic/camera/
├── RawPipeline.kt        # Core RAW processing pipeline
├── CameraController.kt   # Camera2 control / focus / multi-lens
├── ManualController.kt   # Full manual parameter control
├── GpuAlignMerge.kt      # GPU alignment & multi-frame merging
├── FilmicHrEngine.kt     # Filmic tone-mapping engine
├── LearnFilterActivity.kt# LUT learning system
├── ToneCurve / CurveEditor  # Custom tone curves
└── assets/filters/*.cube    # 35+ film simulation LUTs
```

## 🚀 Build

```bash
# Requires Android SDK + NDK
./gradlew assembleDebug
```

## 📄 License

This project is for learning and technical exchange purposes only.

---

<p align="center">
  <b>English</b> &nbsp;|&nbsp; <a href="README.md">简体中文</a>
</p>
