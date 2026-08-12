# qwen/qwen3.5-9b — summarization (standard)

[← leaderboard](../README.md)  ·  [download breakdown (xlsx)](results.xlsx)

**Model:** [Qwen/Qwen3.5-9B](https://huggingface.co/Qwen/Qwen3.5-9B)

Over recent months, we have intensified our focus on developing foundation models that deliver exceptional utility and performance. Qwen3.5 represents a significant leap forward, integrating breakthroughs in multimodal learning, architectural efficiency, reinforcement learning scale, and global accessibility to empower developers and enterprises with unprecedented capability and efficiency.

## Results

| field | value |
| --- | --- |
| LLM judge pass rate | 0.335 |
| LLM judge mean (0–5) | 3.7 |
| Samples | 200 |
| Frozen sample | 4649c02d1615 |
| Assessment | We need to write exactly one concise prose sentence assessing the model's overall behavior and mention any recurring edge case or hallucination pattern only if evidence supports it. If no clear recurring edge case, say so plainly. We have evidence: In all samples, model outputs a "Thinking Process" meta outline... |
| Inference time | 19.031s p50 e2e @ c=1 (self_hosted_gpu_colab) |
| Hardware | NVIDIA A100-SXM4-40GB (34.17 GB) |

## Metrics

| metric | value |
| --- | --- |
| token_f1 | 0.3378 |
| rouge_l | 0.1489 |
