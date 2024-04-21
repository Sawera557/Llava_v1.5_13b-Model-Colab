# Llava_v1.5_13b-Model-Colab

# LLaVA-1.5-13B

LLaVA-1.5-13B is a state-of-the-art multimodal model achieving remarkable performance across 11 benchmarks. It builds upon the original LLaVA framework, utilizing publicly available data to train on a single 8-A100 node in approximately one day. This version surpasses previous methods by leveraging billion-scale data and demonstrating exceptional capabilities in visual and language understanding.

## Abstract

While large language models (LLMs) have shown enhanced zero-shot capabilities in the language domain through instruction tuning using machine-generated data, their application in the multimodal field remains relatively unexplored. In this context, we introduce LLaVA (Large Language-and-Vision Assistant), an end-to-end trained large multimodal model that integrates a vision encoder and language model for comprehensive visual and language comprehension.

## Multimodal Instruction Data

A key aspect of LLaVA is its utilization of language-only GPT-4 for generating multimodal language-image instruction-following data. This marks the inaugural attempt to employ such data in the multimodal domain, facilitating improved understanding of both textual and visual information.

## Performance

Early experiments with LLaVA have demonstrated impressive multimodal chat capabilities, occasionally mirroring behaviors of multimodal GPT-4 on unseen images/instructions. It achieves an 85.1% relative score compared to GPT-4 on a synthetic multimodal instruction-following dataset. Furthermore, upon fine-tuning for Science QA, LLaVA and GPT-4 together achieve a new state-of-the-art accuracy.

## Usage

To use LLaVA for image captioning and instruction-following tasks, follow the steps below:

1. Clone the LLaVA repository:

```bash
%cd /content
!git clone -b v1.0 https://github.com/camenduru/LLaVA
%cd /content/LLaVA
```


2. Install the required dependencies:
```bash
!pip install -q transformers==4.36.2
!pip install -q gradio .
```

3. Import libraries and dependencies
4. Load the model
5. Define the function caption image that takes two inputs:
   image_path -> url
   Prompt -> text
   
