# Rajath John Bosco

I build production LLM systems and study how they fail. Lead Software Engineer (VP) at JPMorgan Chase, working on AI platforms for Consumer & Community Banking. Based in New York.

The numbers below come from each repo's README, where the benchmark setup is documented.

## GPU and inference

| Project | What it is |
| --- | --- |
| [attention-kernel-cuda](https://github.com/jrajath94/attention-kernel-cuda) | CUDA Flash Attention for non-standard head dimensions. Variable-block tiling recovers the 25-44% of compute that fixed-block kernels waste on padding. |
| [triton-inference-kernels](https://github.com/jrajath94/triton-inference-kernels) | Fused softmax and Flash Attention in Triton with online softmax accumulation. 50x lower VRAM than naive attention at sequence length 2048. |
| [model-quantization-lab](https://github.com/jrajath94/model-quantization-lab) | GPTQ vs AWQ vs GGML on Llama 2 7B. AWQ 4-bit: 4.0x compression at 10.04 perplexity. |
| [llm-inference-benchmark](https://github.com/jrajath94/llm-inference-benchmark) | vLLM vs TGI vs TensorRT-LLM under realistic bursty traffic, not synthetic constant load. |

## Evaluation and reliability

| Project | What it is |
| --- | --- |
| [adversarial-prompt-suite](https://github.com/jrajath94/adversarial-prompt-suite) | Red-teaming framework that measures attack-surface coverage instead of counting jailbreaks. 6 attack categories, two-layer classifier (regex heuristics, then an LLM judge for borderline cases). |
| [fault-tolerant-training](https://github.com/jrajath94/fault-tolerant-training) | Elastic checkpoint and recovery for distributed training on spot instances. Survived 47 preemptions across 42 days of 7B-13B runs; $31,400 saved vs on-demand. |
| [llm-eval-suite](https://github.com/jrajath94/llm-eval-suite) | Evaluation framework with LLM-as-judge and custom rubrics, calibrated against human raters. |
| [data-pipeline-monitor](https://github.com/jrajath94/data-pipeline-monitor) | ML pipeline observability with statistical drift detection (KS, chi-square, PSI). |

## From scratch, no dependencies

| Project | What it is |
| --- | --- |
| [bpe-tokenizer](https://github.com/jrajath94/bpe-tokenizer) | BPE and WordPiece tokenizers. 151K and 536K tokens/sec, 144 tests. |
| [jax-transformer-impl](https://github.com/jrajath94/jax-transformer-impl) | Transformer in pure functional JAX with MHA, MQA, and GQA, with verified numerical equivalence between the attention variants. |
| [distributed-kv-store](https://github.com/jrajath94/distributed-kv-store) | Raft consensus from the paper, optimized for ML metadata workloads. |

## Research code

Experiment code and reproducibility artifacts for independent research on LLM systems.

| Project | Topic |
| --- | --- |
| [paper3_failure_planning](https://github.com/jrajath94/paper3_failure_planning) | Failure-aware planning for LLM agents: predicting mid-execution failure from traces |
| [semcp-conformal-prediction](https://github.com/jrajath94/semcp-conformal-prediction) | Conformal prediction over semantic meaning classes for LLM outputs |
| [contamination-contagion](https://github.com/jrajath94/contamination-contagion) | How benchmark leakage propagates through fine-tuning and corrupts evals |
| [stair-tts-scaling-laws](https://github.com/jrajath94/stair-tts-scaling-laws) | Per-problem discrete structure in test-time compute scaling |
| [paper1_orchestrabench](https://github.com/jrajath94/paper1_orchestrabench) | Benchmarking multi-agent LLM topologies across task types |

## In progress

Early-stage, active as of July 2026: [agentsla](https://github.com/jrajath94/agentsla) (SLO verification for tool-calling agents), [draftforge](https://github.com/jrajath94/draftforge) (EAGLE-3 speculative-decoding draft heads), [goodputlab](https://github.com/jrajath94/goodputlab) (control plane for disaggregated LLM serving).

Also: [distributed-rlhf-trainer](https://github.com/jrajath94/distributed-rlhf-trainer), [orderbook-simulator](https://github.com/jrajath94/orderbook-simulator), [polymarket-hft](https://github.com/jrajath94/polymarket-hft), and more quantitative finance work from my Goldman Sachs years.

## Writing

Technical deep-dives at [rajathjohn.com/writing](https://www.rajathjohn.com/writing): Flash Attention in Triton tile by tile, tokenizers from scratch, red-teaming with coverage metrics, benchmarking inference under real traffic, and 20 more.

Contact: rajathjohnbosco@gmail.com
