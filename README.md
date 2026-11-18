<h1 align="center">Feihong Guo</h1>

<p align="center">
  <b>AI Infra Engineer · SGLang Contributor · GPU Computing</b><br/>
  I work on making LLM inference faster, more reliable, and easier to debug.
</p>

<p align="center">
  <a href="https://github.com/sgl-project/sglang/pulls?q=is%3Apr+author%3APhoenix3334">SGLang Pull Requests</a> ·
  <a href="https://github.com/sgl-project/sglang">SGLang</a> ·
  <a href="https://github.com/Phoenix3334">GitHub / Contact</a>
</p>

## About Me

I'm an AI infrastructure engineer focused on **distributed LLM inference and GPU systems**. I enjoy tracing performance and correctness issues across the serving stack — from request scheduling and parallel execution to CUDA streams, communication, and kernels.

My work includes inference runtime debugging, profiling, kernel optimization, and reproducible benchmarking on **NVIDIA GPUs and Ascend NPUs**.

## What I Work On

| Area | Focus |
| :--- | :--- |
| **LLM serving & parallelism** | SGLang, P/D disaggregation, TP / PP / DP / EP / DCP |
| **Runtime correctness** | Request routing, asynchronous execution, CUDA stream and memory lifetimes |
| **GPU performance** | CUDA / Triton kernels, NCCL communication, profiling and optimization |
| **Inference benchmarking** | Throughput, latency, resource utilization, and controlled A/B experiments |
| **Capacity planning & TCO** | SLO-aware GPU sizing, P:D capacity ratios, cross-hardware efficiency, and inputs to deployment-cost estimates |

## Selected SGLang Contributions

| Contribution | What I worked on | PR |
| :--- | :--- | :--- |
| **DP health-check routing** | Isolated health-check traffic from user dispatch state to prevent load imbalance and throughput regressions | [#35721](https://github.com/sgl-project/sglang/pull/35721) · Merged |
| **Async pipeline-parallel correctness** | Fixed received tensor lifetime tracking across CUDA streams to prevent silent output corruption | [#47614](https://github.com/sgl-project/sglang/pull/47614) · Merged |
| **DCP all-to-all packing** | Reduced per-layer packing kernel time from 15.0 to 6.9 µs on B300 while preserving bit-identical results | [#49455](https://github.com/sgl-project/sglang/pull/49455) · Open |

<details>
<summary><b>More things I've explored</b></summary>

- **MoE and distributed execution:** expert parallelism, load balancing, and communication/computation overlap.
- **GPU/NPU optimization:** Triton, TileLang, quantization, and graph capture/replay.
- **Systems performance:** Nsight profiling, capacity planning, and end-to-end inference experiments.

</details>

## Contact

Interested in inference systems, GPU kernels, or tricky runtime bugs? Feel free to connect via [GitHub](https://github.com/Phoenix3334).

<!-- Add a public contact email or LinkedIn URL here when you're ready. -->
