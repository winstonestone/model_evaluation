# Leaderboard — summarization (standard)

[← all models](../../README.md)

| model | model_description | assessment | inference p50 e2e (s) @ c=1, self_hosted_gpu_colab | hardware | task | family | mode | model_supported_languages | eval_languages | n_samples | sample_id | token_f1 | rouge_l | llm_judge_pass_rate | llm_judge_coherence_mean_0_to_5 | llm_judge_consistency_mean_0_to_5 | llm_judge_fluency_mean_0_to_5 | llm_judge_relevance_mean_0_to_5 | llm_judge_faithfulness_mean_gate_score | llm_judge_safety_pass_rate | llm_judge_faithfulness_pass_rate | llm_judge_dimension_mean_0_to_5 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [qwen/qwen3.5-9b](qwen-qwen3-5-9b/) | Over recent months, we have intensified our focus on developing foundation models that deliver exceptional utility and performance. Qwen3.5 represents a significant leap forward, integrating breakthroughs in multimodal learning, architectural efficiency, reinforcement learning scale, and global accessibility to empower developers and enterprises with unprecedented capability and efficiency. | We need to write exactly one concise prose sentence assessing the model's overall behavior and mention any recurring edge case or hallucination pattern only if evidence supports it. If no clear recurring edge case, say so plainly. We have evidence: In all samples, model outputs a "Thinking Process" meta outline... | 19.031 | NVIDIA A100-SXM4-40GB (34.17 GB) | summarization | generative-reference | standard | 201 languages | en | 200 | 4649c02d1615 | 0.3378 | 0.1489 | 0.335 | 3.5751 | 3.9626 | 4.2516 | 3.0009 | 1.489 | 0.78 | 0.415 | 3.7 |

## Definitions

| term | meaning |
| --- | --- |
| llm_judge_dimension_mean_0_to_5 | For each sample, each valid LLM judge scores every graded rubric dimension from 0 to 5. The scorer averages judges per dimension, averages those graded dimensions into a sample score, then averages sample scores across the run. Binary gates such as Safety and Faithfulness are not included in this mean. |
| llm_judge_pass_rate | The fraction of samples whose LLM-judge consensus passed: dimension mean is at least 3.0, no graded dimension is 0 or 1, and all binary/ranged gates pass. |
| sample_id | A short hash of the frozen sample definition and selected dataset rows. Matching sample IDs mean runs are using the same frozen sample. |
| model_supported_languages | Languages claimed by the model card or model metadata. If the model card describes broad support without enumerating every language, the workbook keeps the concise claim, such as 'over 140 languages'. |
| eval_languages | Languages covered by this evaluation task or dataset. This is provenance for the run, not the full language capability of the model. |
| hardware | The hardware the performance timing was measured on. For self-hosted Colab runs this is the exact GPU (name and peak VRAM), pinned across models for comparability. For remote third-party APIs it records that the measurement was client-observed, since the serving hardware is not exposed. |
| token_f1 | Token-level F1 between the model output and the reference: treats each as a bag of lowercased word tokens and computes the harmonic mean of precision (fraction of output tokens found in the reference) and recall (fraction of reference tokens found in the output). Ranges 0 to 1; order-insensitive, so it rewards content overlap rather than exact phrasing. |
| rouge_l | ROUGE-L F1 based on the longest common subsequence (LCS) between output and reference token sequences. Unlike token_f1 it respects word order (the LCS must appear in sequence), so it credits fluent, correctly-ordered overlap. Ranges 0 to 1. |
