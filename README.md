# UniStomaExtraction: High-Throughput Stomatal Phenotyping Tool

# UniStomaExtraction: 高通量气孔表型分析工具

[English](#english) | [中文说明](#chinese)

</div>

---

<a name="english"></a>

## English Documentation

**UniStomaExtraction** is an automated, deep-learning-based software designed for the high-throughput analysis of plant stomatal phenotypes. Built upon the **MMSegmentation** framework and **PyQt5**, it offers precision segmentation of stomata and pores, coupled with comprehensive morphological and spatial statistical analysis.

### ✨ Key Features

| Feature Categories | Description |
| --- | --- |
| **🧠 Deep Learning Core** | Integrated PyTorch & OpenMMLab algorithms for robust segmentation of stomata and pores. |
| **🚀 Batch Processing** | One-click batch analysis for hundreds of images, exporting results to Excel automatically. |
| **📏 Comprehensive Phenotyping** | • **Morphological**: Area, Perimeter, Length, Width, Circularity, Eccentricity, Aspect Ratio.<br>

<br>• **Functional**: Stomatal Opening Degree, Pore Area, Guard Cell Metrics.<br>

<br>• **Population**: Stomatal Density, SPI (Stomatal Pore Index), Orientation Consistency. |
| **🌐 Spatial Analysis** | • **Voronoi Diagrams**: Visualization of stomatal distribution homogeneity.<br>

<br>• **Topology Network**: Nearest neighbor connections.<br>

<br>• **Radar/Rose Charts**: Multi-dimensional metric visualization and orientation distribution. |
| **🖥️ Interactive GUI** | Visual validation, mask color customization, and instant chart preview. |

---

### 📥 Download & Installation

We provide a packaged executable for Windows users. No complex Python environment setup is required.

> **Note:** The package includes trained model weights and configuration. Just download, extract, and run.

<div align="center">
<a href="[https://drive.google.com/file/d/1i7dFmPhitrp0wPbuXJToYyi1-qAx3-G2/view?usp=drive_link](https://www.google.com/search?q=https://drive.google.com/file/d/1i7dFmPhitrp0wPbuXJToYyi1-qAx3-G2/view%3Fusp%3Ddrive_link)" target="_blank">
<img src="[https://img.shields.io/badge/Download_UniStoma_V17.7-(Google_Drive)-4285F4?style=for-the-badge&logo=google-drive&logoColor=white](https://www.google.com/search?q=https://img.shields.io/badge/Download_UniStoma_V17.7-(Google_Drive)-4285F4%3Fstyle%3Dfor-the-badge%26logo%3Dgoogle-drive%26logoColor%3Dwhite)" alt="Download Button" height="50">
</a>
</div>

---

### 🛠 Usage Guide

1. **📂 Open Image Directory**: Click `1. Open Image Dir` to select the folder containing your microscopic images (`.jpg`, `.png`, `.tif`).
2. **⚙️ Configuration (Optional)**:
* **Appearance**: Customize mask colors for stomata/pores.
* **Pre-processing**: Toggle "Filter Border" (ignore incomplete stomata at edges) or "Filter Small" (remove noise).


3. **▶️ Batch Analysis**: Click `4. Batch Analysis`, select an output folder, and wait for the process to finish.
4. **📊 Result Inspection**:
* **Visuals**: Check the `masks`, `overlays`, and `charts` folders in your output directory.
* **Data**: Open `batch_individual.xlsx` (per-stoma data) and `batch_summary.xlsx` (per-image statistics).


5. **👁️‍🗨️ Preview**: Use the GUI to view overlays or select charts (Radar, Rose, Voronoi) from the dropdown menu for the current image.

---

---

<a name="chinese"></a>

## 中文说明

**UniStomaExtraction** 是一款基于深度学习的植物气孔表型高通量分析工具。它集成了 **MMSegmentation** 算法框架与 **PyQt5** 图形界面，旨在为研究人员提供精确的气孔与气孔开口（Pore）分割，以及全自动的形态学与空间分布分析。

### ✨ 核心功能

| 功能类别 | 描述 |
| --- | --- |
| **🧠 深度学习内核** | 内置 PyTorch & OpenMMLab 核心组件，实现气孔与气孔开口的高精度分割。 |
| **🚀 批量处理** | 支持一键处理文件夹内所有图片，自动生成标注图（Overlay）并导出 Excel 数据表。 |
| **📏 全维度表型指标** | • **形态指标**: 面积、周长、长/宽、圆度、偏心率、等效直径等。<br>

<br>• **功能指标**: 气孔开口度 (Opening Degree)、保卫细胞面积、气孔开口指数 (SPI)。<br>

<br>• **群体指标**: 气孔密度 (Density)、排列一致性、最近邻距离。 |
| **🌐 空间拓扑分析** | • **Voronoi 图**: 用于分析气孔分布的均匀性。<br>

<br>• **拓扑网络**: 可视化最近邻气孔连接。<br>

<br>• **雷达图与玫瑰图**: 多维数据展示与气孔角度分布分析。 |
| **🖥️ 交互式 GUI** | 支持缩略图导航、遮罩颜色自定义及实时图表预览。 |

---

### 📥 下载与安装

我们为 Windows 用户提供了打包好的可执行程序，无需配置复杂的 Python 环境即可直接使用。

> **注意:** 下载包中已包含训练好的模型权重和配置文件，解压即用。

<div align="center">
<a href="[https://drive.google.com/file/d/1i7dFmPhitrp0wPbuXJToYyi1-qAx3-G2/view?usp=drive_link](https://www.google.com/search?q=https://drive.google.com/file/d/1i7dFmPhitrp0wPbuXJToYyi1-qAx3-G2/view%3Fusp%3Ddrive_link)" target="_blank">
<img src="[https://img.shields.io/badge/下载_UniStoma_V17.7-(Google_Drive)-4285F4?style=for-the-badge&logo=google-drive&logoColor=white](https://www.google.com/search?q=https://img.shields.io/badge/%E4%B8%8B%E8%BD%BD_UniStoma_V17.7-(Google_Drive)-4285F4%3Fstyle%3Dfor-the-badge%26logo%3Dgoogle-drive%26logoColor%3Dwhite)" alt="Download Button" height="50">
</a>
</div>

---

### 🛠 使用指南

1. **📂 导入图片**: 点击界面左上角的 `1. Open Image Dir` 选择包含显微照片的文件夹。
2. **⚙️ 参数设置 (可选)**:
* **外观**: 自定义气孔和气孔开口的遮罩颜色。
* **预处理**: 建议勾选 "Filter Border" (过滤边缘不完整气孔) 和 "Filter Small" (过滤噪点)。


3. **▶️ 批量分析**: 点击 `4. Batch Analysis`，选择结果保存路径，程序将自动运行。
4. **📊 查看结果**:
* **可视化**: 在输出目录中查看 `masks` (掩膜), `overlays` (叠加图), `charts` (统计图表)。
* **数据**: 打开 `batch_individual.xlsx` (单气孔数据) 和 `batch_summary.xlsx` (单图统计汇总)。


5. **👁️‍🗨️ 实时预览**: 在主界面选择图片后，通过下拉菜单 (`5. Visualization`) 即可实时查看该图片的雷达图、玫瑰图或 Voronoi 图。

</div>
