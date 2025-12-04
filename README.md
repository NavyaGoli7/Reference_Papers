# Reference_Papers
Related to efficient training/fine-tuning design for LLMs

1. Zhang, Y., Liu, Y., Yuan, H., Qin, Z., Yuan, Y., Gu, Q., & Yao, A. C. C. (2025). Tensor product attention is all you need. arXiv preprint [arXiv:2501.06425](https://arxiv.org/pdf/2501.06425)
- The main goal of TPA is to address the severe memory overhead caused by Key-Value (KV) caches during autoregressive inference. This is crucial for enabling LLMs to process longer context sequences.
2. Yang, X., Leng, J., Guo, G., Zhao, J., Nakada, R., Zhang, L., ... & Chen, B. (2024). S $^{2} $ FT: Efficient, scalable and generalizable LLM fine-tuning by structured sparsity. Advances in Neural Information Processing Systems, 37, 59912-59947.[paper link](https://proceedings.neurips.cc/paper_files/paper/2024/file/6e3b9fb0c0c56cf6e1ee61e6a068fca4-Paper-Conference.pdf)
  - The fundamental contribution of S2FT is its ability to concurrently achieve state-of-the-art (SOTA) fine-tuning performance, training efficiency, and inference scalability
3. Li, K., Han, S., Su, Q., Li, W., Cai, Z., & Ji, S. (2025). Uni-LoRA: One Vector is All You Need. arXiv preprint [arXiv:2506.00799](https://arxiv.org/pdf/2506.00799)
- Uni-LoRA's specific "one-vector-only" solution uses an efficient, fixed, and isometric projection matrix that enables global parameter sharing and requires training only this single vector θ\_d to reconstruct parameters for the entire LLM, achieving state-of-the-art parameter efficiency with O(D) time complexity
4. Jeon, H., Lee, S., Kang, B., Kim, Y., & Kim, J. J. (2025). QWHA: Quantization-Aware Walsh-Hadamard Adaptation for Parameter-Efficient Fine-Tuning on Large Language Models. [arXiv preprint arXiv:2509.17428](https://arxiv.org/pdf/2509.17428)
  - QWHA contributes to efficient LLM design by offering a PEFT method that is both computationally efficient during training (due to the WHA design) and effective at preserving accuracy in highly compressed, efficient LLMs for inference (due to its QA initialization scheme)
5. Deng, Y., Zhang, A., Gurses, S., Wang, N., Yang, Z., & Yin, P. (2025). Cloq: Enhancing fine-tuning of quantized llms via calibrated lora initialization. arXiv preprint [arXiv:2501.18475](https://arxiv.org/pdf/2501.18475)
- CLoQ is an efficient design because it focuses on minimizing the computational cost of the initialization step while maximizing the final performance of the memory-efficient combination of LoRA and quantization, a critical area for efficient LLM design
6. 
