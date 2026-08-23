# s1-mini GGUF Q6_K

GGUF Q6_K conversion of [superwhisper/s1-mini](https://huggingface.co/superwhisper/s1-mini)
(Qwen3-0.6B fine-tune for dictation cleanup), for llama.cpp CPU inference.

Converted 2026-08-23 from snapshot 65f84bc via `convert_hf_to_gguf.py` (F16) +
`llama-quantize Q6_K`. Character-identical to the MLX 6-bit build on the full
`s1_mini_bench` reference set (13/13, greedy decoding).

Built for Typefree's dictation cleanup: iOS denies Metal to backgrounded apps,
so the CPU build is the one that can run while a keyboard extension is in
front. License: per upstream model (see the superwhisper/s1-mini model card).

Weights are attached to the [v1 release](../../releases/tag/v1).
