# LLM Text Watermarking Reproduction

reproduction of the watermarking method from the paper  
"A watermark for Large Language Models" (Kirchenbauer et al., 2023).

The experiment evaluates whether AI-generated text contains a detectable watermark signal and how robust the watermark is against simple attacks such as paraphrasing.

Setup:
Python, PyTorch, HuggingFace Transformers  
Model: GPT-2  
Environment: Google Colab (GPU)

Procedure:
1. Generate text normally (no watermark).
2. Generate text using the watermark processor.
3. Run the statistical detector on the generated tokens.
4. Apply a paraphrasing attack and test the detector again.

The detector measures the green-token fraction and computes a z-score to determine whether the text is watermarked.

Example result:

Prediction: Watermarked  
z-score: 13.1
