# What You Read Isn’t What You Hear: Linguistic Sensitivity in Deepfake Speech Detection

This repository contains the code and interactive webpage for the paper:

**What You Read Isn’t What You Hear: Linguistic Sensitivity in Deepfake Speech Detection**  
Binh Nguyen, Shuju Shi, Ryan Ofman, Thai Le  
arXiv:2505.17513v1

---

## Overview

Recent text-to-speech (TTS) advances have enabled highly realistic voice generation, increasing the risk of audio-based deepfake attacks. While most anti-spoofing systems focus on acoustic features, this work demonstrates that _linguistic_ variations in the transcript—such as subtle word choices—can dramatically impact the effectiveness of both open-source and commercial deepfake speech detectors.

This project introduces and systematically studies **transcript-level adversarial attacks**: small, semantically-preserving changes to the transcript that, when synthesized to audio, can cause state-of-the-art detectors to misclassify deepfakes as genuine speech. Results show attack success rates exceeding 60% on several detector–voice pairs, and in some cases, commercial system accuracy drops from 100% to just 32% under attack[1].

---

## Features

- **Interactive Demo:** Explore how changing transcript wording can fool deepfake detectors.
- **Attack Pipeline:** Implements adversarial transcript generation using synonym substitution, masked language models, and semantic similarity constraints.
- **Model-Agnostic:** Works with both open-source and commercial anti-spoofing APIs in black-box settings.
- **Comprehensive Analysis:** Includes feature attribution and case studies (e.g., Brad Pitt scam) to illustrate real-world risks[1].

## Key Findings

- Minor linguistic perturbations (e.g., synonym swaps) can significantly degrade deepfake detection accuracy.
- Some voice and detector combinations are more vulnerable than others; female voices and high-fidelity TTS models are often easier to attack.
- Feature analysis reveals that both linguistic complexity and model-level audio embedding similarity contribute to detector vulnerability.
- Case studies show that transcript-level attacks can enable deepfake scams to bypass commercial defenses in practice[1].

---

## Citation

If you use this demo, please cite:

@article{nguyen2025linguistic,
title={What You Read Isn’t What You Hear: Linguistic Sensitivity in Deepfake Speech Detection},
author={Nguyen, Binh and Shi, Shuju and Ofman, Ryan and Le, Thai},
journal={arXiv preprint arXiv:2505.17513},
year={2025}
}

## Learn More

- [Read the full paper (arXiv:2505.17513v1)](https://arxiv.org/abs/2505.17513)
- For questions or contributions, open an issue or contact the authors.
