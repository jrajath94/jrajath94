### Rajath John

Building open-source tools for ML infrastructure, distributed systems, and quantitative finance.

**Focus areas:** LLM serving & optimization · GPU compute · consensus protocols · market microstructure

---

#### LLM Infrastructure

| Project                                                                           | Description                                                                  |
| --------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| [llm-inference-benchmark](https://github.com/jrajath94/llm-inference-benchmark)   | Benchmark vLLM vs TGI vs TensorRT-LLM with realistic bursty traffic patterns |
| [attention-kernel-cuda](https://github.com/jrajath94/attention-kernel-cuda)       | Custom CUDA Flash Attention kernel for non-standard head dimensions          |
| [distributed-rlhf-trainer](https://github.com/jrajath94/distributed-rlhf-trainer) | Minimal distributed RLHF training loop with Ray + DeepSpeed                  |
| [llm-eval-suite](https://github.com/jrajath94/llm-eval-suite)                     | Evaluation framework with LLM-as-judge and custom rubrics                    |
| [token-streaming-proxy](https://github.com/jrajath94/token-streaming-proxy)       | High-perf SSE proxy for LLM APIs with backpressure handling                  |
| [model-quantization-lab](https://github.com/jrajath94/model-quantization-lab)     | GPTQ/AWQ/GGML quantization comparison with quality metrics                   |
| [prompt-cache-engine](https://github.com/jrajath94/prompt-cache-engine)           | KV-cache sharing for prompt prefix deduplication                             |

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

| Project                                                                                 | Description                                                 |
| --------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| [orderbook-simulator](https://github.com/jrajath94/orderbook-simulator)                 | High-fidelity limit order book with microstructure modeling |
| [alpha-signal-framework](https://github.com/jrajath94/alpha-signal-framework)           | Walk-forward backtesting with lookahead bias prevention     |
| [real-time-risk-engine](https://github.com/jrajath94/real-time-risk-engine)             | GPU-accelerated portfolio VaR with Monte Carlo simulation   |
| [market-data-lakehouse](https://github.com/jrajath94/market-data-lakehouse)             | High-throughput market data ingestion into columnar storage |
| [llm-financial-agent](https://github.com/jrajath94/llm-financial-agent)                 | Multi-agent financial analysis with hallucination detection |
| [low-latency-matching-engine](https://github.com/jrajath94/low-latency-matching-engine) | Sub-microsecond matching engine with price-time priority    |

---

📫 jrajath94@gmail.com
