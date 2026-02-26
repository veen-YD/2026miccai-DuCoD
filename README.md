# DuCoD: Dual-Scale Concept Distillation for Unpaired NBI-WLI Endoscopic Classification

This repository contains the process diagram and abstract part of our paper titled **"DuCoD: Dual-Scale Concept Distillation for Unpaired NBI-WLI Endoscopic Classification"**, submitted to MICCAI 2026. The complete code will be made publicly available after the paper is accepted for publication.

## Abstract

Accurate classification of gastrointestinal lesions from endoscopic images is critical for early cancer detection and clinical decision making. In routine practice, white-light imaging (WLI) is widely available, while narrow-band imaging (NBI) provides enhanced mucosal and vascular contrast with stronger diagnostic cues. However, paired NBI-WLI data are scarce, which limits the development of effective cross-modal learning approaches. This paper proposes a dual-scale concept-guided distillation framework for unpaired cross-modal endoscopic classification. The method leverages NBI during training to transfer diagnostic knowledge to WLI for reliable WLI-only inference. Our framework uses dual-scale semantic concepts and distillation strategies at both sample and class levels to preserve local decision behavior and global class structure. Experimental results on an esophageal endoscopy dataset show significant improvement over baseline methods.

## Process Diagram

![Process Diagram](/framework.png)

The diagram above illustrates the overall framework of DuCoD, where the NBI teacher provides distillation signals to the WLI student using sample-level distillation and class-level optimal transport (OT) alignment, optimized alongside cross-entropy. The concept generation block introduces dual-scale concept candidates for both coarse- and fine-grained lesion descriptions, which are filtered by mutual information (MI) and diversity score (div) for more discriminative supervision.

## Future Plans

The full code for the methods described in the paper will be made publicly available once the paper is accepted. Stay tuned!
