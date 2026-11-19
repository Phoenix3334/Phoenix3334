<h1 align="center">Feihong Guo</h1>

<p align="center">
  <b>AI Systems · LLM Inference Engineering</b><br/>
  Model Adaptation · Distributed Serving · GPU/NPU Performance
</p>

<p align="center">
  <a href="https://phoenix3334.github.io/">Personal Website</a> ·
  <a href="https://phoenix3334.github.io/blog/">Engineering Notes</a> ·
  <a href="https://github.com/sgl-project/sglang/pulls?q=is%3Apr+author%3APhoenix3334">SGLang PRs</a> ·
  <a href="https://github.com/stars/Phoenix3334/lists/ai-infra">AI Infra Reading List</a>
</p>

## About

I work on turning models into **reliable inference capacity under real latency and resource constraints**. From medical-AI prototyping and multimodal inference optimization on Ascend to distributed SGLang serving at Baidu AI Cloud, I follow the **model → runtime → hardware → capacity** path—using reproducible performance evidence to inform parallelism choices, accelerator selection, and downstream cost/TCO assessment.

我关注如何把模型能力转化为**满足业务时延与资源约束的可靠推理产能**。从医疗 AI 原型、昇腾多模态推理与算子优化，到百度智能云的 SGLang 分布式推理压测和运行时排障，我始终沿着**模型 → 运行时 → 硬件 → 服务容量**这条主线，以可复现的性能数据支撑并行配置、算力选型及后续成本与 TCO 评估。

## Selected Work

**[SGLang · Distributed LLM Serving](https://github.com/sgl-project/sglang)** — Benchmarked and debugged DeepSeek/Kimi inference on NVIDIA H200, B300 and GB300, covering Prefill/Decode, parallel configurations, runtime correctness and service capacity.

- **Runtime correctness:** [DP health routing #35721](https://github.com/sgl-project/sglang/pull/35721) · [Async PP stream lifetime #47614](https://github.com/sgl-project/sglang/pull/47614)
- **Kernel & configuration work:** [Inverse RoPE + FP8 fusion #43786](https://github.com/sgl-project/sglang/pull/43786) · [EPLB validation #48404](https://github.com/sgl-project/sglang/pull/48404)

**[MiniCPM-o 4.5 · Full-Duplex Inference](https://github.com/Phoenix3334/minicpmo45-ascend)** — Connected DSpark draft training on B300/DP8 with GGUF deployment and llama.cpp-omni / ggml-CANN optimization on Ascend 910C. Worked on TileLang kernels, ACL Graph and Flow/Vocoder execution; paired 120 s duplex **core RTF: 0.6754 → 0.4829 (−28.5%)**.

**[ThermoPulse · Medical AI Prototype](https://phoenix3334.github.io/#medical)** — A measurement-to-report system spanning long-wave infrared acquisition, YOLOv11 localization, **ResNet18 + Transformer spatial dual-stream vision**, CUDA/TensorRT deployment work, and **Qwen3-8B CPT → SFT** for structured medical reporting.

## Platforms & Tooling

- **Hardware:** NVIDIA H200 / B300 / GB300 · Ascend 910B / 910C · Kunpeng 920
- **Serving & training:** SGLang · vLLM / vLLM-Ascend · llama.cpp-omni · PyTorch · DeepSpeed
- **Kernels & systems:** CUDA / CANN · Triton · TileLang · NCCL · Nsight Systems / Compute

## Systems View

<p align="center">
  <img src="./assets/ai-systems-map.svg" width="100%" alt="AI systems map spanning data, training, inference runtime, accelerators, evaluation, and feedback." />
</p>

## Contact

[Email](mailto:1187883824@qq.com) · [Personal Website](https://phoenix3334.github.io/)
