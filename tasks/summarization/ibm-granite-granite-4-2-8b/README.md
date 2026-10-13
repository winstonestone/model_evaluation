# ibm-granite/granite-4.2-8b — summarization (standard)

[← leaderboard](../README.md)  ·  [download breakdown (xlsx)](results.xlsx)

**Model:** [ibm-granite/granite-4.2-8b](https://huggingface.co/ibm-granite/granite-4.2-8b)

[](https://huggingface.co/collections/ibm-granite/granite-42-language-models) [](https://huggingface.co/blog/ibm-granite/granite-4-2) [](https://github.com/ibm-granite/granite-4.2-language-models) [](https://www.apache.org/licenses/LICENSE-2.0)

## Results

| field | value |
| --- | --- |
| LLM judge pass rate | 1.0 |
| LLM judge mean (0–5) | 5.0 |
| Result status | Quality + performance complete |
| Samples | 2 |
| Frozen sample | c907fe7a8442 |
| Assessment | Judges found broadly acceptable outputs with no recurring edge case clearly isolated. |
| Inference time | 15.081s p50 e2e @ c=1 (self_hosted_gpu_colab) |
| Hardware | NVIDIA A100-SXM4-40GB (34.46 GB) |
| vLLM | 0.31.0 |
| Performance comparability | comparable |
| Comparability reason | Workload, request counts, runtime, and measurement scope are complete. |
| Comparability key | 1d9f7dc05dfe31d00c3f061630858ba512bfc8003ecd72a085097cb0599fee55 |
| Workload SHA-256 | bbedeabcb998219882636db76b900b9aa5c73345c51a6f731e8336af2e248361 |
| Performance workload | 2 frozen rows; 100 requests/sweep at [1, 4, 8, 16]; 400/400 measured requests succeeded; 0/0 warmups succeeded |
| TTFT | N/A — Offline vLLM does not expose reliable first-token timing. |
| GPU memory | available |

## Metrics

| metric | value |
| --- | --- |
| token_f1 | 0.5524 |
| rouge_l | 0.2897 |
