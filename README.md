### Rajath John

Building open-source tools for ML infrastructure, distributed systems, quantitative finance, and AI safety.

**Focus areas:** LLM serving & optimization · GPU compute · consensus protocols · market microstructure · AI safety & interpretability

---

#### LLM Infrastructure

| Project                                                                                     | Description                                                                  |
| ------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| [llm-inference-benchmark](https://github.com/jrajath94/llm-inference-benchmark)             | Benchmark vLLM vs TGI vs TensorRT-LLM with realistic bursty traffic patterns |
| [attention-kernel-cuda](https://github.com/jrajath94/attention-kernel-cuda)                 | Custom CUDA Flash Attention kernel for non-standard head dimensions          |
| [triton-inference-kernels](https://github.com/jrajath94/triton-inference-kernels)           | Fused Triton kernels for attention + FFN with autotuning for LLM serving     |
| [distributed-rlhf-trainer](https://github.com/jrajath94/distributed-rlhf-trainer)           | Minimal distributed RLHF training loop with Ray + DeepSpeed                  |
| [llm-eval-suite](https://github.com/jrajath94/llm-eval-suite)                               | Evaluation framework with LLM-as-judge and custom rubrics                    |
| [token-streaming-proxy](https://github.com/jrajath94/token-streaming-proxy)                 | High-perf SSE proxy for LLM APIs with backpressure handling                  |
| [model-quantization-lab](https://github.com/jrajath94/model-quantization-lab)               | GPTQ/AWQ/GGML quantization comparison with quality metrics                   |
| [prompt-cache-engine](https://github.com/jrajath94/prompt-cache-engine)                     | KV-cache sharing for prompt prefix deduplication                             |

#### Systems & Infrastructure

| Project                                                                         | Description                                                          |
| ------------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| [gpu-memory-profiler](https://github.com/jrajath94/gpu-memory-profiler)         | Visual GPU memory profiler with leak detection for PyTorch           |
| [distributed-kv-store](https://github.com/jrajath94/distributed-kv-store)       | Raft-consensus KV store optimized for ML metadata                    |
| [container-gpu-scheduler](https://github.com/jrajath94/container-gpu-scheduler) | K8s operator for GPU-aware batch scheduling with bin-packing         |
| [data-pipeline-monitor](https://github.com/jrajath94/data-pipeline-monitor)     | Real-time ML pipeline observability with statistical drift detection |
| [zero-copy-tensor-ipc](https://github.com/jrajath94/zero-copy-tensor-ipc)       | Zero-copy tensor sharing across processes via shared memory          |
| [fault-tolerant-training](https://github.com/jrajath94/fault-tolerant-training) | Elastic checkpoint/recovery for distributed training jobs            |
| [ml-feature-store](https://github.com/jrajath94/ml-feature-store)               | Point-in-time correct feature store with DuckDB + Arrow              |

#### Quantitative Finance

| Project                                                                                 | Description                                                            |
| --------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| [orderbook-simulator](https://github.com/jrajath94/orderbook-simulator)                 | High-fidelity limit order book with microstructure modeling            |
| [alpha-signal-framework](https://github.com/jrajath94/alpha-signal-framework)           | Walk-forward backtesting with lookahead bias prevention                |
| [real-time-risk-engine](https://github.com/jrajath94/real-time-risk-engine)             | Portfolio VaR engine with Monte Carlo simulation and Greeks            |
| [market-data-lakehouse](https://github.com/jrajath94/market-data-lakehouse)             | High-throughput market data ingestion into columnar storage            |
| [llm-financial-agent](https://github.com/jrajath94/llm-financial-agent)                 | Multi-agent financial analysis with hallucination detection            |
| [low-latency-matching-engine](https://github.com/jrajath94/low-latency-matching-engine) | Price-time priority matching engine — cache-line alignment & seqlock   |
| [polymarket-hft](https://github.com/jrajath94/polymarket-hft)                           | Prediction market HFT strategy with sub-second order execution         |

#### NLP & AI Safety

| Project                                                                               | Description                                                              |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| [adversarial-prompt-suite](https://github.com/jrajath94/adversarial-prompt-suite)     | Red-teaming harness for systematic jailbreak & prompt injection testing  |
| [bpe-tokenizer](https://github.com/jrajath94/bpe-tokenizer)                           | BPE tokenizer from scratch with vocabulary analysis and merge tracking   |
| [jax-transformer-impl](https://github.com/jrajath94/jax-transformer-impl)             | MHA, MQA, and GQA attention in pure functional JAX with JIT/vmap/pmap    |

---

#### Research Code

Experiment code and reproducibility artifacts for independent research on LLM systems.

| Project                                                                                             | Description                                                              |
| ---------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| [paper3_failure_planning](https://github.com/jrajath94/paper3_failure_planning)                     | Failure-aware planning for LLM agents: predicting mid-execution failure from traces |
| [stair-tts-scaling-laws](https://github.com/jrajath94/stair-tts-scaling-laws)                       | Per-problem discrete structure in test-time compute scaling              |
| [semcp-conformal-prediction](https://github.com/jrajath94/semcp-conformal-prediction)               | Conformal prediction over semantic meaning classes for LLM outputs       |
| [contamination-contagion](https://github.com/jrajath94/contamination-contagion)                     | How benchmark leakage propagates through fine-tuning and corrupts evals  |
| [crisp-grokking-paper](https://github.com/jrajath94/crisp-grokking-paper)                           | Unifying grokking and neural scaling laws via phase transitions          |
| [paper1_orchestrabench](https://github.com/jrajath94/paper1_orchestrabench)                         | Benchmarking multi-agent LLM topologies across task types                |

#### Currently Building

Active projects, in progress as of July 2026: [agentsla](https://github.com/jrajath94/agentsla) (SLO-aware reliability runtime for tool-calling agents), [draftforge](https://github.com/jrajath94/draftforge) (EAGLE-3 speculative-decoding draft head training), [goodputlab](https://github.com/jrajath94/goodputlab) (control plane for disaggregated LLM serving).

---

Contact: jrajath94@gmail.com
