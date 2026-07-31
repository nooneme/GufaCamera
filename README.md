<p align="center">
  <b>简体中文</b> &nbsp;|&nbsp; <a href="README_EN.md">English</a>
</p>

<h1 align="center">📷 Classic Camera</h1>

<p align="center">
  <em>全 RAW 管线 · 所见即所得 · LUT 学习系统</em>
</p>

---

**Classic Camera** 是一款功能极简、面向创作的全手动相机应用。它不依赖厂商的图像处理算法，而是直接驱动相机传感器的 **RAW 数据**，把最纯净的光学质感交还给你。所有参数调节都实时作用在 RAW 数据上，你在预览框看到的就是最终成片。

## 📱 界面预览

<p align="center">
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053222.jpg" width="19%" alt="界面预览 1"/>
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053243.jpg" width="19%" alt="界面预览 2"/>
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053247.jpg" width="19%" alt="界面预览 3"/>
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053359.jpg" width="19%" alt="界面预览 4"/>
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053407.jpg" width="19%" alt="界面预览 5"/>
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053417.jpg" width="19%" alt="界面预览 6"/>
  <img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/screenshots/Screenshot_20260801_053635.jpg" width="19%" alt="界面预览 7"/>
</p>

## ✨ 核心功能

### 1. 全 RAW 管线 · 纯净光学质感

完全绕过厂商的 ISP（图像信号处理）算法。从 Bayer 原始数据开始，经过降噪、白平衡、CFA 重排与色调映射，全程由应用自己掌控。**没有暴力锐化、没有过度涂抹，只有传感器最初捕捉到的光。**

### 2. 预览实时 RAW 渲染 · 所见即所得

取景器不是厂商 ISP 出来的带全套算法和不一致曝光的预览流，而是对 RAW 数据的**实时完整渲染**。你在屏幕上看到的光影、色彩与细节，就是按下快门后得到的成片——不需要靠经验脑补最终效果。

### 3. 参数调节作用在 RAW 数据上 · 免去后期麻烦

曝光、白平衡、色温、色调曲线、胶片模拟……每一项调节都**直接作用在 RAW 像素上**，并在预览框中实时呈现。拍摄现场即可完成创作调整，摆脱「拍完再进后期」的繁琐流程。

### 4. 自带 LUT 学习系统 · 最低 2 张照片学懂任何滤镜

应用内置 LUT 学习引擎：

- **最低仅需 2 张照片**，即可学习出任意滤镜（一张原图 + 一张带目标滤镜效果的图）
- 自带 **35+** 款高质量胶片模拟滤镜（富士、理光、徕卡、宾得、Lumix 等经典胶片风格）
- 学习引擎提供覆盖率 / 训练与验证误差可视化，帮助评估学到的滤镜质量

### 5. 功能极简

没有广告、没有推送、没有账号系统、没有花哨的社区功能。只保留拍摄最核心的能力：**干净、专注、可离线使用。**

> **兼容性说明：** 目前仅在 **Samsung Galaxy S23 Ultra** 上测试过，其它设备上的表现可能有所差异。

## 🖼 样片展示

全部随手拍，直出，本人摄影水平有限，仅作效果展示。

<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260722_175518_6.3mm.jpg" width="100%" alt="样片 1"/></td>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260725_191039_6.3mm.jpg" width="100%" alt="样片 2"/></td>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_151337_6.3mm.jpg" width="100%" alt="样片 3"/></td>
  </tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_154935_6.3mm.jpg" width="100%" alt="样片 4"/></td>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_155744_7.9mm.jpg" width="100%" alt="样片 5"/></td>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_160432_6.3mm.jpg" width="100%" alt="样片 6"/></td>
  </tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_163909_6.3mm.jpg" width="100%" alt="样片 7"/></td>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_170852_7.9mm.jpg" width="100%" alt="样片 8"/></td>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260727_171301_6.3mm.jpg" width="100%" alt="样片 9"/></td>
  </tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/nooneme/GufaCamera/main/images/samples/IMG_20260731_220015_6.3mm.jpg" width="100%" alt="样片 10"/></td>
    <td colspan="2">&nbsp;</td>
  </tr>
</table>

## 🛠 技术栈

| 层面 | 技术 |
| --- | --- |
| 语言 | Kotlin · C/C++ (NDK) |
| 相机 | Camera2 API，全手动控制（曝光/对焦/白平衡/多镜头） |
| 渲染 | OpenGL ES 实时 RAW 渲染管线 |
| 原生 | CMake + JNI，C++ 实现色调曲线 / LUT 生成等 |
| 平台 | minSdk 26 · targetSdk 36，支持 arm64-v8a / x86_64 |

## 📂 项目结构（部分）

```
app/src/main/java/com/classic/camera/
├── RawPipeline.kt        # 核心 RAW 处理管线
├── CameraController.kt   # Camera2 控制 / 对焦 / 多镜头
├── ManualController.kt   # 全手动参数控制
├── GpuAlignMerge.kt      # GPU 对齐与多帧合成
├── FilmicHrEngine.kt     # 胶片感影调引擎
├── LearnFilterActivity.kt# LUT 学习系统
├── ToneCurve / CurveEditor  # 自定义色调曲线
└── assets/filters/*.cube    # 35+ 款胶片模拟 LUT
```

## 🚀 构建

```bash
# 需要 Android SDK + NDK 环境
./gradlew assembleDebug
```

## 📄 许可

该项目仅供学习与技术交流使用。

---

<p align="center">
  <a href="README_EN.md">English</a> &nbsp;|&nbsp; <b>简体中文</b>
</p>
