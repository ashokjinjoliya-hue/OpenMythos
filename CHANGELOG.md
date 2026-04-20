# Changelog

All notable changes to OpenMythos are documented here.

## [0.3.0] — 2026-04-20

### Added
- MLA (Multi-Latent Attention) support alongside GQA — switchable via `attn_type`
- LTI-stable injection via ZOH discretization (spectral radius < 1 guaranteed)
- ACT (Adaptive Computation Time) halting mechanism
- Depth-wise LoRA adapter for per-loop adaptation
- Loop-index RoPE embedding to differentiate recurrent block across iterations
- Pre-configured model variants: `mythos_1b` through `mythos_1t`
- Training script for 3B model on FineWeb-Edu with multi-GPU support (DDP)
- Full API documentation in `docs/open_mythos.md`
- Dataset guidance in `docs/datasets.md`

### Changed
- MoEFFN now uses fine-grained expert segmentation (DeepSeekMoE-style)
- Router bias is a buffer (not a gradient parameter) for load balancing

## [0.2.0] — 2026-04-10

### Added
- Initial MoE FFN with shared and routed experts
- GQA attention with KV cache
- RoPE positional embeddings
- Prelude → Recurrent Block → Coda architecture

## [0.1.0] — 2026-04-01

### Added
- Initial release: basic looped transformer skeleton
