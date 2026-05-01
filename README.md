# Lung-CL(INTERSPEECH 2026)

![architecture](/figures/architecture.png)

Lung-CL: Spectrum-aware Distillation and Generative Replay for Continual Learning based buffer-free Respiratory Sound Classification

Qinben Lai, Shuai Liu, Jiaxin Zhao, Wenjuan Wang, Lukui Shi*

*corresponding author

Our work, **Lung-CL**, introduces a privacy-first approach to respiratory sound analysis through three core innovations:   

- **Unified Buffer-Free Framework**: We provide a robust, privacy-preserving solution for domain-incremental learning (DIL) in clinical settings. 
- **Class-Specific Latent Replay (CSLR)**: To mitigate catastrophic forgetting without storing sensitive patient audio, we developed CSLR. It utilizes lightweight **Class-Specific Gaussian Mixture Models (CS-GMMs)** to synthesize high-fidelity pseudo-features within the latent semantic space.   
- **Multi-Level Spectrum-Aware Distillation (MLSAD)**: We designed MLSAD to handle the unique time-frequency characteristics of respiratory sounds. Its core component, **Energy-Gated Distillation (EGD)**, acts as a filter to suppress device-specific noise and artifacts, guiding the model to focus explicitly on domain-invariant pathological patterns.   

## Requirements

Install the necessary packages with:

```
$ pip install torch torchvision torchaudio
$ pip install -r requirements.txt
```

The code is coming soon