<div align="center">

# IndEgo: A Dataset of Industrial Scenarios and Collaborative Work for Egocentric Assistants

**[Vivek Chavan](https://vivekchavan.com/)¹²\*, [Yasmina Imgrund](https://www.linkedin.com/in/yasmina-imgrund/)²†, [Tung Dao](https://www.linkedin.com/in/lam-dao-tung/)²†, [Sanwantri Bai](https://www.linkedin.com/in/sanwantri-bai-0a808a1b3/)³†, [Bosong Wang](https://www.linkedin.com/in/bosong0106/)⁴†, Ze Lu⁵†, [Oliver Heimann](https://www.linkedin.com/in/oliver-heimann/)¹, [Jörg Krüger](https://www.tu.berlin/iat/ueber-uns/leitung)¹²**

<p>
¹Fraunhofer IPK, Berlin &nbsp;&nbsp;&nbsp; ²Technical University of Berlin &nbsp;&nbsp;&nbsp; ³University of Tübingen<br>
⁴RWTH Aachen University &nbsp;&nbsp;&nbsp; ⁵Leibniz University Hannover
</p>

*<sup>\*Project Lead &nbsp;&nbsp;&nbsp; †Work done during student theses/projects at Fraunhofer IPK, Berlin.</sup>*

### **Published at NeurIPS 2025**

<p>
    <a href="https://IndEgo-Dataset.github.io/" target="_blank"><img src="https://img.shields.io/badge/Project-Website-blue?style=for-the-badge&logo=google-chrome" alt="Project Website"></a>
    <a href="https://openreview.net/forum?id=jKw3Qhc8m1" target="_blank"><img src="https://img.shields.io/badge/Paper-PDF-red?style=for-the-badge&logo=adobe-acrobat-reader" alt="Paper PDF"></a>
    <a href="https://huggingface.co/datasets/FraunhoferIPK/IndEgo" target="_blank"><img src="https://img.shields.io/badge/🤗-Dataset-yellow?style=for-the-badge" alt="Hugging Face Dataset"></a>
    <a href="https://neurips.cc/virtual/2025/poster/121501" target="_blank"><img src="https://img.shields.io/badge/NeurIPS-Page-orange?style=for-the-badge" alt="NeurIPS Page"></a>
</p>
<p>
    <a href="https://colab.research.google.com/drive/1qCZnFQNRjBuy3vBlkMy7sMTcYkTNOzgg?usp=sharing" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
</p>

</div>

---

Welcome to the official code repository for **IndEgo**, a **NeurIPS 2025 Datasets & Benchmarks Track** accepted dataset and open-source framework for **industrial egocentric vision**, designed to support **training, real-time guidance, process improvement, and collaboration**.

---

## 🔍 Key Features
- 3000+ egocentric videos, 1000+ exocentric videos
- Task steps, audio narration, SLAM, gaze, motion data
- Reasoning-based video QA benchmark
- Annotated collaborative sequences with tools and workspace layout

---

## 🛠️ Environment Setup

### Create and install from `requirements.txt`
```bash
# Create a new virtual environment
python3 -m venv $HOME/indego_env
source $HOME/indego_env/bin/activate

# Install dependencies
pip install -r requirements.txt
```
---

## 📦 Dataset Structure
Each Category includes:
- Egocentric + Exocentric videos
- Gaze, motion, hand-pose logs
- Narrations (where applicable)
- Keysteps and mistakes (if any)
- SLAM data (missing for some sequences)

> [!WARNING]
> # 🚧 MAINTENANCE IN PROGRESS 🚧
>
> ### ⚠️ The dataset structure is currently being reorganised. 
> **File paths and folder names are changing.** 
>
> If you download the data right now, your local file structure may become inconsistent with future updates. 
> We recommend waiting until the restructuring is complete (ETA: 12 Dec, 2025).
>
> **[👉 Click here to be notified when the dataset is ready](https://forms.gle/j8krD3At2hEWjJPg8)**
---

## 🤝 Related Works

This repository builds upon and integrates components from several open-source projects and pretrained models. We gratefully acknowledge the contributions of the following repositories and their authors:

- [facebookresearch/projectaria_tools](https://github.com/facebookresearch/projectaria_tools) – for egocentric device support and video/sensor tooling  
- [DAMO-NLP-SG/VideoLLaMA3](https://github.com/DAMO-NLP-SG/VideoLLaMA3) for baseline evaluations.
- [QwenLM/Qwen3](https://github.com/QwenLM/Qwen3) for baseline evaluations.
- [OpenGVLab/InternVL](https://github.com/OpenGVLab/InternVL) for baseline evaluations.

This project also leverages the open-source AI ecosystem, including [🤗 Hugging Face Transformers](https://github.com/huggingface/transformers), [FlashAttention](https://github.com/Dao-AILab/flash-attention), [Decord](https://github.com/dmlc/decord), and other publicly released models and frameworks.

We thank these communities for making research reproducible and accessible.

---

## 🧩 Citation

If you use the IndEgo dataset or code in your research, please cite our paper:

```bibtex
@inproceedings{Chavan2024IndEgo,
  author    = {Vivek Chavan and Yasmina Imgrund and Tung Dao and Sanwantri Bai and Bosong Wang and Ze Lu and Oliver Heimann and J{\"o}rg Kr{\"u}ger},
  title     = {IndEgo: A Dataset of Industrial Scenarios and Collaborative Work for Egocentric Assistants},
  booktitle = {Advances in Neural Information Processing Systems (NeurIPS) Datasets and Benchmarks Track},
  year      = {2024},
  url       = {https://neurips.cc/virtual/2025/poster/121501}
}
```

## 🏆 Acknowledgments & Funding

This work is funded by the German Federal Ministry of Research, Technology and Space (BMFTR) and the German Aerospace Center (DLR) under the KIKERP project (Grant No. 16IS23055C) in the KI4KMU program. We thank the Meta AI team and Reality Labs for the Project Aria initiative, including the research kit, the open-source tools and related services. The data collection for this study was carried out at the IWF research labs and the test field at TU Berlin. Lastly, we sincerely thank the student volunteers and workers who participated in the data collection process.

<div align="center" style="margin-top: 20px;">
    <a href="https://www.bmftr.bund.de/" target="_blank" rel="noopener noreferrer" style="margin: 20px;">
        <img src="https://IndEgo-Dataset.github.io/assets/BMFTR_-_Logo_en.svg" alt="BMBF Logo" height="100">
    </a>
    &nbsp;&nbsp;&nbsp;&nbsp;
    <a href="https://www.dlr.de/" target="_blank" rel="noopener noreferrer" style="margin: 20px;">
        <img src="https://IndEgo-Dataset.github.io/assets/PT_DLR_Logo_SW_D_2018_lang.png" alt="DLR Logo" height="60">
    </a>
    &nbsp;&nbsp;&nbsp;&nbsp;
    <a href="https://www.dlr.de/" target="_blank" rel="noopener noreferrer" style="margin: 20px;">
        <img src="https://IndEgo-Dataset.github.io/assets/logo-iwf-mit-namen-en.jpg" alt="IWF Logo" height="60">
    </a>
    &nbsp;&nbsp;&nbsp;&circ;
    <a href="https://www.projectaria.com/" target="_blank" rel="noopener noreferrer" style="margin: 20px;">
        <img src="https://IndEgo-Dataset.github.io/assets/Reality_Labs_logo.svg" alt="Meta Reality Labs Logo" height="60">
    </a>
</div>
