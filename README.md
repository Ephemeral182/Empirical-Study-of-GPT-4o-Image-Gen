# 🚀 Unveiling GPT-4o's Image Generation Prowess: A Comprehensive Empirical Deep Dive 🖼️

**[Paper on arXiv](https://arxiv.org/abs/2504.05979)** | **[High-Res PDF on Google Drive](https://drive.google.com/file/d/14PNtDBv1LC2QG5E6zdMV-gpIv9TTl_VQ/view?usp=drive_link)** | **(Link to Project Page/Demo if applicable)**

**Authors:** Sixiang Chen, Jinbin Bai, Zhuoran Zhao, Tian Ye, Qingyu Shi, Donghao Zhou, Wenhao Chai, Xin Lin, Jianzong Wu, Chao Tang, Shilin Xu, Tao Zhang, Haobo Yuan, Yikang Zhou, Wei Chow, Linfeng Li, Xiangtai Li, Lei Zhu, Lu Qi

*(Affiliations: The Hong Kong University of Science and Technology (GZ), National University of Singapore, Peking University, The Chinese University of Hong Kong, University of Washington, Wuhan University)*

## Overview

The world marvels at the image generation capabilities of models like GPT-4o, but their closed-source nature leaves many questions unanswered. How truly capable is GPT-4o compared to its peers? Has the dream of a *unified* model for text and image generation been realized internally?

This repository accompanies our paper, **"An Empirical Study of GPT-40 Image Generation Capabilities"**, which presents the **first comprehensive empirical benchmark** of GPT-4o's image generation performance. We rigorously evaluated GPT-4o against leading open-source and commercial systems (including Gemini 2.0 Flash Experimental, Midjourney, FLUX, and various SOTA models) across a massive range of tasks, providing critical insights into its strengths, weaknesses, and its place in the evolution of generative AI.

## Key Contributions & Scope

We conducted a detailed qualitative analysis covering **more than 20 distinct tasks** across four major categories:

1.  **Text-to-Image Generation:**
    * Complex Prompt Following (Attribute Binding, Numeracy, Object Relationships)
    * **Exceptional Text Rendering (Short & Long Text, Document Generation)**
    * Panorama Generation
2.  **Image-to-Image Generation:**
    * Style Transfer (Diverse Artistic Styles)
    * **Advanced Image Editing (Fine-grained, Large-scale, Subject Preservation)**
    * Subject Customization (Single & Multi-Concept Personalization)
    * Story Image Generation (Coherent Multi-Panel Narratives)
    * Low-Level Vision (Denoising, Deraining, Dehazing, Super-Res, In/Outpainting, Colorization, Relighting, etc.)
    * Spatial Control (Canny, Depth, Sketch, Pose, Mask)
    * Camera Control (Bokeh, Focal Length, Shutter Speed, Temperature)
    * In-Context Visual Prompting (Few-shot task adaptation)
3.  **Image-to-3D Generation:**
    * Image-to-3D Modeling (Interface Rendering, .obj Export)
    * UV Map-to-3D Rendering
    * Novel View Synthesis
4.  **Image-to-X (Dense Understanding & Generation):**
    * Image Segmentation (Referring, Semantic, Panoptic)
    * Edge Detection & Image Matting
    * Salient/Mirror/Shadow/Camouflage Object Detection
    * Depth & Normal Estimation
    * Layout & Text Detection
    * Object Tracking (Multi-Object)

## ✨ GPT-4o: Key Strengths Identified

Our study highlights several areas where GPT-4o demonstrates remarkable, often state-of-the-art, performance:

* 🥇 **Unmatched Text Rendering:** Truly exceptional ability to render coherent and accurate text (short and long) within images, crucial for documents, charts, and creative uses.
* 🧠 **Superior Prompt Comprehension & Composition:** Excels at understanding and executing complex prompts involving multiple objects, attributes, and spatial relationships.
* 🎨 **Powerful Image Manipulation:** Strong generalization across a wide array of image editing, style transfer, and customization tasks, often preserving subject identity better than competitors.
* 📐 **Impressive Spatial & 3D Reasoning:** Shows inherent understanding of geometry and consistency in tasks like 3D view synthesis, depth-conditioned generation, and UV map rendering.
* 🔧 **Versatile Image Transformation:** Capably handles diverse image restoration and understanding tasks (like segmentation, denoising, depth estimation) under a unified framework without task-specific tuning.

## ⚠️ Limitations and Challenges

Despite its strengths, GPT-4o is not without limitations:

* ❓ **Inconsistent Generation:** Can sometimes deviate from precise prompt details (counts, colors, layout) or input image content, especially in editing and low-level tasks.
* 👻 **Hallucination:** Susceptible to generating non-existent or factually incorrect content, particularly with complex or underspecified prompts.
* 🌐 **Data Bias:** Struggles with generating underrepresented cultural elements and rendering non-Latin scripts accurately.
* 📉 **Task-Specific Gaps:** Underperforms specialized models in certain areas like panorama generation, precise spatial control, layout/text detection, and object tracking consistency.

## Conclusion

This work provides a crucial, in-depth empirical baseline for understanding GPT-4o's image generation capabilities. It showcases the immense power achieved by large multimodal models while highlighting the remaining challenges in consistency, fidelity, bias, and reasoning that pave the way for future research towards truly unified and reliable generative systems.

**Dive into the full paper for detailed examples and analysis!**

## Acknowledgements

We sincerely thank all authors for their dedication and hard work in conducting this comprehensive empirical study.

## Citation

If you find this work useful in your research, please consider citing our paper:

```bibtex
@misc{chen2025empirical,
      title={An Empirical Study of GPT-40 Image Generation Capabilities}, 
      author={Sixiang Chen and Jinbin Bai and Zhuoran Zhao and Tian Ye and Qingyu Shi and Donghao Zhou and Wenhao Chai and Xin Lin and Jianzong Wu and Chao Tang and Shilin Xu and Tao Zhang and Haobo Yuan and Yikang Zhou and Wei Chow and Linfeng Li and Xiangtai Li and Lei Zhu and Lu Qi},
      year={2025},
      eprint={2504.05979},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
