# LLM Text Watermarking Reproduction
This project reproduces the watermarking method proposed in the paper  
"A Watermark for Large Language Models".
The goal is to test whether AI-generated text can contain a detectable watermark.
The experiment generates text with and without watermarking.
A statistical detector is used to identify whether the watermark is present.
The project also tests whether paraphrasing can weaken or remove the watermark signal.
Tools used: Python, PyTorch, HuggingFace Transformers, and GPT-2.
Experiments were run in Google Colab.
