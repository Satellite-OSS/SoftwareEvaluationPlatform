<div align="center">

  A community-curated list of open-source platforms for testing/evaluating satellite software, maintained by the **[OPENSAT](https://github.com/Satellite-OSS)** open-source satellite community.

[![Total views](https://raw.githubusercontent.com/Satellite-OSS/.github/main/traffic/SoftwareEvaluationPlatform/views.svg)](https://github.com/Satellite-OSS/.github/tree/main/traffic/SoftwareEvaluationPlatform "Cumulative recorded repository views; updated hourly")
[![Discussions](https://img.shields.io/badge/Discussions-Join%20the%20Community-2ea44f?style=flat-square&logo=github)](https://github.com/orgs/Satellite-OSS-BUPT/discussions)
[![README](https://img.shields.io/badge/README-中文-blue?style=flat-square)](README.zh-CN.md)

**English** | [中文](README.zh-CN.md)

</div>

---

## 📋 About This List

Satellite software research needs somewhere to run experiments. This repository collects ten open-source projects that can serve as **evaluation platforms** — they let you drive workloads, run benchmarks, reproduce experiments and compare policies for satellite computing, networking and scheduling. 

Everything here comes from one of two places:

- **Community originals(TBD)** — evaluation tools built by OPENSAT itself, collected under [`original tools/`](<original tools/README.md>). They cover containerized and Wasm (WebAssembly) software evaluation and are closely tied to the work OPENSAT members do.
- **Third-party links** — open-source projects maintained elsewhere, listed as ready-made evaluation platforms.

---

## 🎯 Selection Criteria

1. Directly relevant to satellite software evaluation scenarios
2. Real, runnable source code 
3. Supports at least one evaluation workflow: benchmarking, reproducibility, policy comparison or performance analysis

---

## Third-Party Platforms

The projects below are ordered roughly by how close they sit to the satellite itself: from satellite edge computing and constellation networking, through in-orbit benchmarks and astrodynamics, out to ground-segment tooling.

### 1️⃣ SatEdgeSim

[SatEdgeSim](https://github.com/wjy491156866/SatEdgeSim) simulates satellite edge computing, and is mostly used to compare scheduling strategies against latency, throughput and resource metrics.

### 2️⃣ StarPerf-Satellite-Simulator

[StarPerf-Satellite-Simulator](https://github.com/zhanghefan123/Starperf-Satellite-Simulator) focuses on large-scale constellation network performance, which makes it a good fit for routing, congestion and link-dynamics experiments.

### 3️⃣ STAR-Bench

[STAR-Bench](https://github.com/necst/STAR-Bench) is a benchmark and testbed for in-orbit vision tasks, built around comparing accuracy and robustness against compute cost.

### 4️⃣ LuPNT

[LuPNT](https://github.com/Stanford-NavLab/LuPNT) offers a simulation and experimentation platform for space navigation, aimed at evaluating PNT algorithms and reproducing scenarios.

### 5️⃣ EOS-Bench

[EOS-Bench](https://github.com/Ethan19YQ/EOS-Bench) gathers Earth-observation satellite scheduling instances into a single benchmark, so different scheduling algorithms can be compared on the same instances and metrics.

### 6️⃣ Basilisk

[Basilisk](https://github.com/AVSLab/basilisk) is a high-fidelity spacecraft dynamics framework, typically used for GNC validation, closed-loop experiments and performance analysis.

### 7️⃣ poliastro

[poliastro](https://github.com/poliastro/poliastro) is a Python astrodynamics library, useful for orbit-algorithm experiments, batch parameter studies and rapid prototyping.

### 8️⃣ Orekit

[Orekit](https://github.com/CS-SI/Orekit) is a high-precision astrodynamics and orbit-computation library in Java, and serves as a baseline for orbit propagation, determination and estimation evaluation.

### 9️⃣ CubeSatSim

[CubeSatSim](https://github.com/alanbjohnston/CubeSatSim) simulates a CubeSat end to end, and is used for communication-link evaluation, mission-flow validation and teaching or research experiments.

### 🔟 AIT-Core

[AIT-Core](https://github.com/NASA-AMMOS/AIT-Core) is the core of a ground mission-operations and testing framework, where it supports command and telemetry validation, integration testing and experiment automation.

---

## 🤔 How to Choose

- For **satellite edge computing research**: SatEdgeSim, StarPerf
- For **benchmark-oriented workflows**: STAR-Bench, EOS-Bench
- For **astrodynamics simulation and evaluation**: Basilisk, Orekit, poliastro
- For **ground-system and mission-pipeline experiments**: AIT-Core, CubeSatSim

---

## 🤝 Contributing

Researchers, developers, students and satellite enthusiasts are all welcome. If you know of a project that belongs on this list, open a pull request or start a thread in the Discussions.
👉 **[Join the Discussions](https://github.com/orgs/Satellite-OSS-BUPT/discussions)**

---

## 📄 License

This document is a curated navigation summary. Licenses and copyrights for each project remain with their original repositories.