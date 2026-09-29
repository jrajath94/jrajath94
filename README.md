# Rajath John Bosco

Vice President, Lead Software Engineer at JPMorgan Chase (May 2023 - present), based in New York. I build production LLM, retrieval, and analytics systems in regulated environments.

I work on LLM inference and serving efficiency: benchmarking vLLM and SGLang, speculative decoding, and custom Triton/CUDA kernels, alongside guarded agent systems and hybrid retrieval serving 300+ engineers.

Earlier roles: Quantitative Developer, Global Markets at Goldman Sachs (Oct 2021 - Apr 2023); Software Engineer Intern, Product Security at NVIDIA (May 2020 - Aug 2020); and Associate Software Engineer, promoted to Software Engineer at Visa (Jul 2016 - Aug 2019).

My independent, AI-assisted open-source systems work covers agent reliability, LLM evaluation, efficient inference, and distributed serving. I publish measured results, test status, and explicit unmeasured boundaries; repository READMEs are the source of truth for each project's current status.

## Current systems work

| Project | Evidence available in the repository |
| --- | --- |
| [AgentSLA](https://github.com/jrajath94/agentsla) | Reliability runtime for tool-calling agents with policy gates, numeric verification, execution budgets, append-only traces, and deterministic replay for deterministic adapters. |
| [DraftForge](https://github.com/jrajath94/draftforge) | EAGLE-3 draft-head training and evaluation pipeline. Three A100 seeds measured 68.7% +/- 1.0% held-out greedy agreement; serving inter-token latency remains explicitly unmeasured pending a weight-schema adapter. |
| [GoodputLab](https://github.com/jrajath94/goodputlab) | SLO-aware control plane and benchmark rig for vLLM. A 54-cell dedicated-H100 sweep retained the negative result that disaggregation slightly improved mean inter-token latency but lost on time to first token and hardware cost for the measured 7B setup. |
| [dpo-lab](https://github.com/jrajath94/dpo-lab) | Honest DPO fine-tuning experiments at weekend scale. Run 6 on Qwen2.5-1.5B-Instruct with ultrafeedback_binarized measured a 54.2% held-out win rate over the base model (n=400, 95% Wilson CI [0.494, 0.591]), independently verified; the MMLU guard failure is documented as a known limit. |
| [rag-chunking-eval](https://github.com/jrajath94/rag-chunking-eval) | RAG chunking evaluation harness on SQuAD v2 (60-question dev slice). Recall@5: hierarchical 0.917 > semantic 0.867 > fixed-500-100 0.817 > fixed-500-0 0.800; near-zero faithfulness scores are documented as a metric artifact, not a finding. |
| [agent-checkpoint-replay](https://github.com/jrajath94/agent-checkpoint-replay) | Checkpoint, restore, and deterministic replay for long-running tool-calling agent runs. Real kill -9 crash demo with byte-identical resume (20/20 steps); 14/14 tests green; ~480 lines of standard-library Python. |

## Additional verified implementations

| Project | Scope |
| --- | --- |
| [bpe-tokenizer](https://github.com/jrajath94/bpe-tokenizer) | BPE and WordPiece implementations with 144 locally passing tests. |
| [adversarial-prompt-suite](https://github.com/jrajath94/adversarial-prompt-suite) | Prompt-injection and jailbreak evaluation across six attack categories with 93 locally passing tests. |
| [distributed-kv-store](https://github.com/jrajath94/distributed-kv-store) | Distributed key-value store focused on storage, replication, and recovery behavior, with 79 locally passing tests. |

Other public implementations cover Triton and CUDA attention kernels, functional JAX transformers, tokenization, checkpoint recovery, model evaluation, and quantitative systems. Their repositories should be treated as implementation evidence; hardware-dependent performance claims require the environment described in each project.

## Repository index

- [Adversarial Prompt Suite](https://github.com/jrajath94/adversarial-prompt-suite) · [BPE Tokenizer](https://github.com/jrajath94/bpe-tokenizer) · [Distributed KV Store](https://github.com/jrajath94/distributed-kv-store)
- [JAX Transformer](https://github.com/jrajath94/jax-transformer-impl) · [Triton Inference Kernels](https://github.com/jrajath94/triton-inference-kernels) · [Orderbook Simulator](https://github.com/jrajath94/orderbook-simulator)
- [Attention Kernel CUDA](https://github.com/jrajath94/attention-kernel-cuda) · [Fault-Tolerant Training](https://github.com/jrajath94/fault-tolerant-training) · [Model Quantization Lab](https://github.com/jrajath94/model-quantization-lab)

## Technical scope

- Employer-backed engineering: Python, SQL, Java, TypeScript, AWS, Kafka, distributed systems, developer platforms, retrieval systems, guarded text-to-SQL, and React at JPMorgan Chase and Goldman Sachs.
- Independent ML systems: AI agents and reliability, large language model evaluation, RAG, speculative decoding, inference benchmarking, PyTorch, JAX, CUDA, Triton, vLLM, and SGLang.
- Independent systems tooling: API development, Kubernetes, Docker, FastAPI, DuckDB, Prometheus, and Grafana.

## Writing

- [Reliability contracts for tool-calling agents](https://www.rajathjohn.com/writing/agentsla-reliability-contracts-for-tool-calling-agents)
- [Measuring EAGLE-3 before claiming a speedup](https://www.rajathjohn.com/writing/draftforge-measuring-eagle3-before-claiming-speedups)
- [When disaggregated LLM serving does not win](https://www.rajathjohn.com/writing/goodputlab-when-disaggregated-serving-does-not-win)

More at [rajathjohn.com/writing](https://www.rajathjohn.com/writing).

Contact: rajathjohnbosco@gmail.com | linkedin.com/in/rajathj
