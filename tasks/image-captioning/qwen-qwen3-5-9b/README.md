# qwen/qwen3.5-9b — image-captioning (standard)

[← leaderboard](../README.md)  ·  [download breakdown (xlsx)](results.xlsx)

**Model:** [Qwen/Qwen3.5-9B](https://huggingface.co/Qwen/Qwen3.5-9B)

Over recent months, we have intensified our focus on developing foundation models that deliver exceptional utility and performance. Qwen3.5 represents a significant leap forward, integrating breakthroughs in multimodal learning, architectural efficiency, reinforcement learning scale, and global accessibility to empower developers and enterprises with unprecedented capability and efficiency.

## Results

| field | value |
| --- | --- |
| LLM judge pass rate | 0.95 |
| LLM judge mean (0–5) | 4.08 |
| Samples | 20 |
| Frozen sample | 4704ecefa02e |
| Assessment | The model generally provides accurate descriptions of images but occasionally introduces minor inaccuracies or hallucinations, particularly in details like object orientations, specific text, and structural elements, without a clear recurring edge case. |
| Inference time | 14.014s p50 e2e @ c=1 (self_hosted_gpu_colab) |
| Hardware | NVIDIA A100-SXM4-40GB (39.49 GB) |

## Metrics

| metric | value |
| --- | --- |
| token_f1 | 0.2515 |
| rouge_l | 0.1511 |
| meteor | 0.3064 |
| cider | 1.1643 |
| bertscore | 0.8135 |
| clipscore | 0.7072 |
