# A Multi-Modal Prompt-tuning Method of Ultrasound Diagnosis for Thyroid Nodule

Introduction
------------
This project proposes a Multi-Modal Prompt-tuning method for assisting the diagnosis of thyroid nodules in ultrasound images.
Given that ultrasound diagnosis heavily relies on clinical expertise — especially challenging in underdeveloped regions — we present a lightweight solution using small-scale multi-modal learning, combining both ultrasound images and symptom descriptions.
Our method achieves state-of-the-art performance, even surpassing human radiologists on multiple datasets.

Method Overview
---------------
- Image Feature Extraction: A pre-trained BEiT (Bidirectional Encoder representation from Image Transformers) model is used to extract regional features from ultrasound images.
- Text Feature Extraction: A hard-prompt tuning model is designed to process clinical symptom descriptions.
- Multi-Modal Fusion: Image and text features are concatenated and input into an MLP (Multi-Layer Perceptron) for final diagnosis prediction.
- Few-shot Learning: Achieves strong performance with only a small number of image-text samples, without expensive full model fine-tuning.

Main Contributions
------------------
- Proposed a novel multi-modal prompt-tuning framework that enhances ultrasound diagnosis without full model fine-tuning.
- Demonstrated that hand-crafted hard prompts outperform soft prompts in medical text understanding.
- Achieved superior accuracy compared to human radiologists across datasets.
