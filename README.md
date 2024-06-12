<h2 align="center"> <a href="https://arxiv.org/abs/xxx">Holmes-VAD: Towards Unbiased and Explainable
Video Anomaly Detection via Multi-modal LLM</a></h2>
<h5 align="center"> If you like our project, please give us a star ⭐ on GitHub for latest update.  </h2>

## 📰 News
* **[2024.06.12]** 👀 Our **HolmesVAD** and **VAD-INstruct50k** will be available soon, welcome to **star** ⭐ this repository for the latest updates.


## 😮 Highlights
Towards open-ended Video Anomaly Detection (VAD), existing methods often exhibit biased detection when faced with challenging or unseen events and lack interpretability. To address these drawbacks, we propose Holmes-VAD, a novel framework that leverages precise temporal supervision and rich multimodal instructions to enable accurate anomaly localization and comprehensive explanations.


## 🛠️ Requirements and Installation
* Python >= 3.10
* Pytorch == 2.0.1
* CUDA Version >= 11.7
* transformers >= 4.37.2
* Install required packages:
```bash
git clone https://github.com/pipixin321/HolmesVAD.git
cd HolmesVAD
conda create -n holmesvad python=3.10 -y
conda activate holmesvad
pip install --upgrade pip  # enable PEP 660 support
pip install -e .
pip install -e ".[train]"
pip install flash-attn --no-build-isolation
```

## 🤗 Demo

### CLI Inference

```bash
CUDA_VISIBLE_DEVICES=0 python demo/cli.py --model-path your/path/to/videollava-7b-vad-lora --model-base your/path/to/Video-LLaVA-7B --file your/path/to/video.mp4
```

### Gradio Web UI

```bash
CUDA_VISIBLE_DEVICES=0 python demo/gradio_demo.py
```
