# Leaderboard — summarization (standard)

[← all models](../../README.md)

| model | result_status | model_description | assessment | inference p50 e2e (s) | hardware | performance_comparability | performance_comparability_reason | performance_comparability_key | performance_workload_sha256 | performance_measurement | ttft_availability | gpu_memory_availability | task | task_version | task_config_sha256 | launch_plan_id | launch_plan_sha256 | planned_estimated_cost_usd | planned_cost_cap_usd | actual_cost_usd | family | mode | model_supported_languages | eval_languages | n_samples | sample_id | token_f1 | rouge_l | llm_judge_pass_rate | llm_judge_coherence_mean_0_to_5 | llm_judge_consistency_mean_0_to_5 | llm_judge_fluency_mean_0_to_5 | llm_judge_relevance_mean_0_to_5 | llm_judge_faithfulness_mean_gate_score | llm_judge_faithfulness_pass_rate | llm_judge_dimension_mean_0_to_5 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [ibm-granite/granite-4.2-8b](ibm-granite-granite-4-2-8b/) | Quality complete - performance pending | [](https://huggingface.co/collections/ibm-granite/granite-42-language-models) [](https://huggingface.co/blog/ibm-granite/granite-4-2) [](https://github.com/ibm-granite/granite-4.2-language-models) [](https://www.apache.org/licenses/LICENSE-2.0) | Judges found broadly acceptable outputs with no recurring edge case clearly isolated. | - | - | - | - | - | - | - | - | - | summarization | 5 | 66930ad8887ab5a537ddf873d9a84b53a8f595fa48491b00e8decdd4354163c3 | evalplan-8bc5c6c7e586fd90f9f0 | 8bc5c6c7e586fd90f9f0c69cd1f668399e261d99b622086f02faa74249003a60 | 0.363441 | 9.003441 | - | generative-reference | standard | en, de, es, fr, ja, pt, ar, cs, it, ko, nl, zh | en | 2 | c907fe7a8442 | 0.5218 | 0.2825 | 1.0 | 5.0 | 5.0 | 5.0 | 5.0 | 2.0 | 1.0 | 5.0 |

## Definitions

| term | meaning |
| --- | --- |
| result_status | Whether this immutable revision contains quality only, quality with performance still pending, or the completed quality-and-performance result. |
| llm_judge_dimension_mean_0_to_5 | For each sample, each valid LLM judge scores every graded rubric dimension from 0 to 5. The scorer averages judges per dimension, averages those graded dimensions into a sample score, then averages sample scores across the run. Gate scores are not included in this mean. |
| llm_judge_pass_rate | The fraction of samples whose LLM-judge consensus passed: dimension mean is at least 3.0, no graded dimension is 0 or 1, and all binary/ranged gates pass. |
| sample_id | A short hash of the frozen sample definition and selected dataset rows. Matching sample IDs mean runs are using the same frozen sample. |
| model_supported_languages | Languages claimed by the model card or model metadata. If the model card describes broad support without enumerating every language, the workbook keeps the concise claim, such as 'over 140 languages'. |
| eval_languages | Languages covered by this evaluation task or dataset. This is provenance for the run, not the full language capability of the model. |
| hardware | The hardware the performance timing was measured on. For self-hosted Colab runs this is the exact GPU (name and peak VRAM), pinned across models for comparability. For remote third-party APIs it records that the measurement was client-observed, since the serving hardware is not exposed. |
| performance_comparability | Whether the performance artifact passed its frozen-workload, request-count, hardware, and runtime contract. Only rows with the same comparability key are directly comparable. |
| performance_comparability_key | A SHA-256 grouping key over shared benchmark conditions. Different models may be compared only when this key matches. |
| performance_workload_sha256 | SHA-256 of the frozen prompt-row identities, prompt content hashes, system prompt, and generation limits used for the benchmark. |
| performance_measurement | The actual frozen dataset-row count, measured requests at each concurrency level, successful request count, and completed warmups. |
| token_f1 | Token-level F1 between the model output and the reference: treats each as a bag of lowercased word tokens and computes the harmonic mean of precision (fraction of output tokens found in the reference) and recall (fraction of reference tokens found in the output). Ranges 0 to 1; order-insensitive, so it rewards content overlap rather than exact phrasing. |
| rouge_l | ROUGE-L F1 based on the longest common subsequence (LCS) between output and reference token sequences. Unlike token_f1 it respects word order (the LCS must appear in sequence), so it credits fluent, correctly-ordered overlap. Ranges 0 to 1. |
