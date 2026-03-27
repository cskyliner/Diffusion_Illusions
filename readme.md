# Diffusion Illusions - CV Course Final Project

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Course](https://img.shields.io/badge/Course-Computer_Vision-orange.svg)]()

</div>

## 📖 简介 (Introduction)

本项目为 **2025年秋季（25fall）计算机视觉（Computer Vision）** 课程的期末项目。
本项目的核心目标是探索并尝试改进已有的扩散模型视错觉生成框架：[**Diffusion-Illusions**](https://github.com/RyannDaGreat/Diffusion-Illusions)。

通过结合文本到图像的扩散模型（Text-to-Image Diffusion Models），我们研究了如何生成在不同观察条件（如旋转、翻转、远近距离等）下呈现不同语义内容的视错觉图像，并针对其原有的模型细节和流程进行了多项改进尝试。

---

## 🌟 主要探索内容 (Features & Experiments)

本项目包含多个针对不同类型视错觉的独立实验模块，均以 Jupyter Notebook 的形式提供，方便在 Google Colab 或本地环境中直接运行：

- **`flippy_illusions_for_colab.ipynb`**: 翻转错觉 (Flippy Illusions) - 图像在正向和上下翻转时呈现出完全不同的有意义画面。
- **`hidden_characters_for_colab.ipynb`**: 隐藏字符 (Hidden Characters) - 在复杂的背景纹理中隐藏特定的字符或图案，远看或缩小观看时才能清晰辨认。
- **`parker_puzzle_colab.ipynb`**: 帕克拼图错觉 (Parker Puzzle) - 探索基于空间重排或拼图机制的视觉生成效果。
- **`rotation_overlays_for_colab.ipynb`**: 旋转叠加错觉 (Rotation Overlays) - 随着图像旋转不同角度，呈现多重且各异的视觉内容。
- **`twisting_squares_colab.ipynb`**: 扭曲方块错觉 (Twisting Squares) - 利用几何纹理和光影生成的几何视错觉效果。

---

## 🛠️ 安装与环境配置 (Installation)

建议使用 `conda` 或 `venv` 创建独立的虚拟环境来运行本项目。

1. **克隆仓库**：
   ```bash
   git clone https://github.com/cskyliner/Diffusion_Illusions.git
   cd Diffusion_Illusions
   ```

2. **安装依赖**：
   本项目依赖于 `diffusers`, `transformers` 以及其他常用的科学计算库。
   ```bash
   pip install -r requirements.txt
   ```

*(注：如果使用 GPU 进行推理或生成，请确保您已正确配置对应版本的 CUDA 和 PyTorch 环境。)*

---

## 🚀 使用方法 (Usage)

本项目的大部分实验都可以直接通过对应的 Jupyter Notebook 运行。代码主要为了在 **Google Colab** 环境下快速运行而设计。

如果您使用的是 **Google Colab**：
1. 将本仓库克隆至 Google Drive，或直接在 Colab 中打开对应 Notebook 的 GitHub 链接。
2. 将 Runtime 类型更改为 GPU。
3. 按照 Notebook 中的单元格顺序依次运行，安装必要环境后即可开始生成视错觉图像。

如果您使用的是 **本地环境**：
1. 确保您的机器上安装有支持 CUDA 的显卡。
2. 启动 Jupyter：
   ```bash
   jupyter notebook
   ```
3. 打开需要实验的 `.ipynb` 文件。

---

## 📄 参考文献与致谢 (Acknowledgements)

- 感谢原框架作者 **RyannDaGreat** 提供的灵感与强大的基础代码库：[**Diffusion-Illusions**](https://github.com/RyannDaGreat/Diffusion-Illusions)。
- 本项目是在计算机视觉课程的指导下完成的，旨在加深对图像生成模型、潜空间优化（Latent Optimization）和视错觉构成的理解。
