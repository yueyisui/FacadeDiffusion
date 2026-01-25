# FaçadeDiffusion

> **FaçadeDiffusion**: Building Façade Generation via Diffusion Models with Soft Semantic Guidance.  

<p align="center">
  <img src="assets/figures/fig1_overview.png" width="100%"/>
</p>

## 🔥 Highlights
- **Semantic layout control**: generate façades aligned with target semantic maps.
- **Reference-style control**: use a reference façade image (and its semantic map) to transfer appearance while respecting structure.
- **Supports partial reference**: center-cropped reference image → complete façade generation.
- **LoD texture projection demo**: map generated façade textures onto LoD building models.
- **LSAA-v2 datasets**: provides 5,961 building façade images with corresponding semantic labels and text prompts.

<p align="center">
  <img src="assets/figures/fig2_pipeline.png" width="100%"/>
</p>

---

## 🏢 LSAA-v2 Dataset

**LSAA-v2** provides **5,961 building façade images** with paired **semantic labels and text prompts**.

- The **test split** of LSAA-v2 can be downloaded from [Google Drive](https://drive.google.com/drive/folders/1PLhzE8qJrwigYaXsqC40buLZRlF5H3B6?hl=zh-cn).
- The **train split** of LSAA-v2 is coming soon.

---

## 📌 News
- **2026-01-25**: Initial public repo template + paper figures.
- **2026-01-25**: Provide the test split of LSAA-v2 dataset .

---

## 🧩 Results at a glance

### Experiment setting 1: different reference façades + semantic layouts
<p align="center">
  <img src="assets/figures/exp1_multi_ref_semantic.png" width="100%"/>
</p>

### Experiment setting 2: center-cropped reference → full façade completion
<p align="center">
  <img src="assets/figures/exp2_center_crop_reference.png" width="100%"/>
</p>

---

## 📦 Data preparation

This repo is dataset-agnostic. You only need paired data:
- RGB façade image `I`
- semantic map `S` (integer labels or color-coded map)
- text prompt `T`

See [docs/DATASETS.md](https://github.com/yueyisui/FacadeDiffusion/blob/main/docs/DATASETS.md) for expected folder layout and label conventions.

---

## 🎬 LoD texture projection demo
<p align="center">
 <video src="assets/demos/lod_with_texture.mp4" controls width="80%"></video>
</p>
---

## 📊 Evaluation

- Semantic parsing metrics: mIoU / F1 / Precision / Recall / Accuracy
- Appearance consistency: LPIPS / CLIP-Score / FID / DINO / CLIP-IQA / CLIP-based multi-façade similarity (CLIP-MF), etc.

See: [docs/EVALUATION](https://github.com/yueyisui/FacadeDiffusion/blob/main/docs/EVALUATION.md).

---

## 🧾 License

- **Code**: Apache-2.0 (see [LICENSE](https://github.com/yueyisui/FacadeDiffusion/blob/main/LICENSE))  
- **Dataset (if you release LSAA-v2)**: CC BY-NC-SA 4.0 (derivative work based on LSAA).  
  See [docs/DATASETS.md](https://github.com/yueyisui/FacadeDiffusion/blob/main/docs/DATASETS.md).

---

## 🙏 Acknowledgements
- Built on top of the Diffusers / Accelerate ecosystem.
- Thanks to the authors of LSAA and related façade datasets.

