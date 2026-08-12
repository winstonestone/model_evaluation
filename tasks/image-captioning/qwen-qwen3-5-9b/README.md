# qwen/qwen3.5-9b — image-captioning (standard)

[← leaderboard](../README.md)  ·  [download breakdown (xlsx)](results.xlsx)

**Model:** [Qwen/Qwen3.5-9B](https://huggingface.co/Qwen/Qwen3.5-9B)

Over recent months, we have intensified our focus on developing foundation models that deliver exceptional utility and performance. Qwen3.5 represents a significant leap forward, integrating breakthroughs in multimodal learning, architectural efficiency, reinforcement learning scale, and global accessibility to empower developers and enterprises with unprecedented capability and efficiency.

## Results

| field | value |
| --- | --- |
| LLM judge pass rate | 0.95 |
| LLM judge mean (0–5) | 4.1 |
| Samples | 20 |
| Frozen sample | 4704ecefa02e |
| Assessment | The model demonstrates inconsistent accuracy in image captioning, occasionally introducing hallucinations such as incorrect structures or object details, but does not exhibit a clear recurring edge case across the samples. |
| Inference time | 14.014s p50 e2e @ c=1 (self_hosted_gpu_colab) |
| Hardware | NVIDIA A100-SXM4-40GB (34.25 GB) |

## Metrics

| metric | value |
| --- | --- |
| token_f1 | 0.2506 |
| rouge_l | 0.1508 |
| meteor | 0.3067 |
| cider | 1.189 |
| bertscore | 0.8125 |
| clipscore | 0.7134 |
