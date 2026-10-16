<div align="center">

# 谢安豪 · anhaoXie

**计科 2026 级 · 广外南国商学院**

正在系统学习 Python、Web 与机器学习。目标很简单：**做出 3 个真能跑、真有人用的项目。**

<sub>Learning Python, web development and ML in public — the goal is three projects that actually run and actually get used.</sub>

</div>

---

## 现在在做什么

**90 天出海挑战** — 从 2026-10-01 起，每天一个 commit，每个项目都必须真的部署上线，
而不是只在我自己电脑上跑得起来。**今天是第 16 天，连续没断。**

规则和每天的进度都记在 **[hello-micro-tools](https://github.com/anhaoXie/hello-micro-tools)**。

## 精选项目

<table>
<tr>
<td width="50%" valign="top">

### 🏔️ [3dgs-cpu-port](https://github.com/anhaoXie/3dgs-cpu-port)

**在一台没有 NVIDIA 独显的笔记本上，用纯 PyTorch 把 SIGGRAPH 2023 的
3D Gaussian Splatting 完整复现出来。**

官方 `train.py` / `render.py` / `metrics.py` **一个字节都没改**——只把两个算法性的
CUDA 扩展换成 CPU 实现，再用一个启动期 shim 把 `device="cuda"` 重定向到 CPU。
"官方代码没被改过" 不是一句声明，而是脚本里的 SHA-256 校验。

15000 迭代、**87,475 个高斯**下 PSNR **17.63**、SSIM 0.594、LPIPS 0.414（CPU 8 线程，约 3.4 小时）。
论文在 RTX 3090 上是 23.14 / 0.841 / 0.183——差距约 5.5 dB，根因是没显卡导致的
迭代预算与模型容量压缩，而不是算法简化。**我把这个差距也写进了文档。**

`PyTorch` `CUDA-free` `3D Reconstruction` `COLMAP`

</td>
<td width="50%" valign="top">

### 🎬 [videonote](https://github.com/anhaoXie/videonote) ⭐

**本地视频学习工作台**：把视频丢进来，自动做
语音识别 → 画面分析 → 摘要笔记 → 字幕，还有**逐句跟读发音评分**。

完全本地可跑——**不配任何 API key 也能用**。插件化架构，加功能不用动已有代码；
桌面图标双击即开，像 App 一样用，没有浏览器地址栏。

`Python` `Whisper` `Offline` `Desktop`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🛂 [visa-photo-tool](https://github.com/anhaoXie/visa-photo-tool)

把自拍裁成**像素精确的签证 / 护照证件照**，内置美签、申根、中国三种官方规格，
带人脸对齐椭圆参考线和浏览器内 AI 去背景。

照片全程不出浏览器 —— 没有后端、没有账号、没有广告。

`Next.js` `TypeScript` `Canvas` `ONNX Runtime`

**[→ visa.anhaoxie.com](https://visa.anhaoxie.com)**

</td>
<td width="50%" valign="top">

### 📡 [ai-frontier](https://github.com/anhaoXie/ai-frontier)

**AI 前沿每日雷达**：从 20 个公开源采集、去重、打分，输出 Excel 清单和
**带判断的日报**——不只是罗列链接，而是写出"这条为什么值得看"。

**零 API Key**，全本地跑。

`Python` `Data Pipeline` `Excel` `Local-first`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🎯 [hr-radar](https://github.com/anhaoXie/hr-radar)

**行业 HR 需求雷达**：抓真实招聘岗位，量化出这个行业到底要什么技能、给多少钱、
卡什么学历，再对上你自己的能力，告诉你缺什么、先补什么、怎么证明。
面向在校大学生的实习 / 校招。

零第三方依赖。库内 509 条真实岗位。

`Python` `Zero-dependency` `Data Analysis`

</td>
<td width="50%" valign="top">

### 📓 [kaggle-journey](https://github.com/anhaoXie/kaggle-journey)

Kaggle 竞赛学习日志，**当天写、不做事后美化**。里面有一次完整的事故复盘：
教程里的模型三个都跑出 100% 准确率，查下去发现是 `Survived` 答案列被当成特征喂进了模型。

`Machine Learning` `Python` `Data Science`

**[→ 读 Day 03](https://github.com/anhaoXie/kaggle-journey/blob/main/logs/Day03.md)**

</td>
</tr>
</table>

## 技术栈

<div align="center">

![Python](https://img.shields.io/badge/Python-3776ab?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-ee4c2c?style=flat-square&logo=pytorch&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178c6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-f7df1e?style=flat-square&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-e34f26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572b6?style=flat-square&logo=css3&logoColor=white)

![React](https://img.shields.io/badge/React-61dafb?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38bdf8?style=flat-square&logo=tailwindcss&logoColor=white)

![Git](https://img.shields.io/badge/Git-f05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-0078d4?style=flat-square&logo=windows&logoColor=white)

</div>

## 我在坚持的几件事

- **每天一个 commit。** 进度可以慢，但不能断。今天是第 16 天。
- **每个项目都必须真的上线。** "在我电脑上能跑"不算完成，公开链接才算。
- **把卡住的地方写下来。** 报错、判断失误、走过的弯路，都留在日志里而不是删掉。
- **先砍范围，再动手。** 一个做完的小东西，胜过十个没做完的大东西。
- **不把复现说成创新。** 3DGS 是复现别人论文，我会把"我改了什么、没改什么、差在哪"分开写。

## 联系

- GitHub: [@anhaoXie](https://github.com/anhaoXie)
- Email: [wde23@foxmail.com](mailto:wde23@foxmail.com)

<div align="center">
<sub>如果你也在做 90 天挑战，或者对 <a href="https://visa.anhaoxie.com">visa-photo-tool</a> 有建议，欢迎开 issue 找我。</sub>
</div>
