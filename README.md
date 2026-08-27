# Marcos Villagra

I'm a computer scientist and research engineer at [Bagel Labs](https://bagel.com), working on decentralized generative models, world and action modeling for robotics, and verifiable machine learning.

My background is in theoretical computer science, including computational complexity, cryptography, and quantum computation. My work connects that foundation with hands-on research engineering: diffusion models, expert routing, model training and evaluation, and Rust implementations of cryptographic primitives.

[Google Scholar](https://scholar.google.com/citations?user=poLYdvYAAAAJ&sortby=pubdate) · [Personal website](https://sites.google.com/view/marcosvillagra/) · [Hugging Face releases at Bagel Labs](https://huggingface.co/bageldotcom)

## Recent research

Selected collaborative work with my coauthors at Bagel Labs:

- [**WorldDiT: A Unified Diffusion Architecture for World and Action Modeling**](https://arxiv.org/abs/2607.23909) — 2026. A diffusion transformer that learns continuous robot actions alongside future visual prediction, without a large pretrained vision-language model as its action backbone. The public release includes checkpoints and an inference/evaluation runtime for all four LIBERO simulation suites.
- [**Paris 2.0: A Decentralized Diffusion Model for Video Generation**](https://arxiv.org/abs/2605.26064) — 2026. Extends independent expert training and learned routing from image generation to temporally coherent video generation.
- [**Heterogeneous Decentralized Diffusion Models**](https://openaccess.thecvf.com/content/CVPR2026/html/Jiang_Heterogeneous_Decentralized_Diffusion_Models_CVPR_2026_paper.html) — **CVPR 2026**. Combines independently trained DDPM and flow-matching experts at inference, with checkpoint conversion and efficient architectures that lower training requirements. [arXiv](https://arxiv.org/abs/2603.06741)
- [**Expert-Data Alignment Governs Generation Quality in Decentralized Diffusion Models**](https://arxiv.org/abs/2602.02685) — **ICLR 2026 DeLTa and Sci4DL workshops; first author**. Studies why routing to experts whose training distributions match the current denoising state matters more for generation quality than numerical stability alone.

## Open-source code and model releases

These are collaborative research releases; the links distinguish source code, documentation, and model weights.

| Project | What to explore | Links |
| --- | --- | --- |
| **WorldDiT** | Robot policy checkpoints, inference code, and LIBERO evaluator. | [Hugging Face](https://huggingface.co/bageldotcom/worlddit) |
| **Paris 2.0** | Video-generation expert checkpoints and learned router. | [Hugging Face — gated access](https://huggingface.co/bageldotcom/paris2) |
| **Paris** (2025) | Decentralized text-to-image generation with independently trained experts. The public GitHub repository contains the paper and release documentation. | [Paper](https://arxiv.org/abs/2510.03434) · [GitHub](https://github.com/bageldotcom/paris) · [Hugging Face — gated access](https://huggingface.co/bageldotcom/paris) |
| **ZKLoRA** (2025) | Zero-knowledge verification of private LoRA adapters. The current Python/Rust implementation uses native Halo2 proofs for transcript-bound, quantized LoRA delta correctness. | [Paper](https://arxiv.org/abs/2501.13965) · [Source code](https://github.com/bageldotcom/zkLoRA) |
| **Tiny Tool Use** (2025) | Config-driven LLM tool-use fine-tuning with SFT, DPO, synthetic data, and evaluation workflows. | [Source code](https://github.com/bageldotcom/bagel-RL/tree/main/Tiny%20Tool%20Use) · [Qwen3-0.6B ToolBench checkpoint](https://huggingface.co/bageldotcom/TinyToolUse-Qwen3-0.6B-toolbench) · [Write-up](https://blog.bagel.com/p/tiny-tool-use) |

Model access and usage terms are documented on each release page.

## Rust, cryptography, and systems experiments

| Repository | Focus |
| --- | --- |
| [poseidon-benchmarks](https://github.com/mdvillagra/poseidon-benchmarks) | Criterion benchmarks of Dusk, CryptoExperts, Risc0, and Neptune implementations. Supported by Ethereum Foundation grant FY23-1156. [Benchmark reports](https://mdvillagra.github.io/poseidon-benchmarks/) |
| [poseidon-rust](https://github.com/mdvillagra/poseidon-rust) | Compact Poseidon permutation and sponge implementation over arkworks fields, with parameter loading and regression tests. |
| [halo2-practice](https://github.com/mdvillagra/halo2-practice) | A readable custom PLONK-style gate, witness assignment, and public-input constraints checked with `MockProver`. |
| [radixsort](https://github.com/mdvillagra/radixsort) | Rust experiments sorting large field elements, benchmarked against the standard library. |

The compact cryptography implementations are research and learning projects, not audited production libraries.

## Teaching and mentoring

I design and maintain course material at Facultad Politécnica, Universidad Nacional de Asunción (FP-UNA):

- [Blockchain 2025](https://github.com/mdvillagra/blockchain-2025): Solidity, Hardhat, ERC-721, and React/MetaMask examples, assignment scaffolding, and project workflows.
- [Matemática Aplicada 2024](https://github.com/mdvillagra/matematica-aplicada-2024): applied mathematics final projects and submission workflows.

My role in these repositories is course design, scaffolding, and mentoring. Student submissions remain the work of their credited authors.
