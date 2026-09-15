<div align="center">

 由 **[OPENSAT](https://github.com/Satellite-OSS)** 开源卫星社区维护的一份面向卫星软件测试/评估的开源平台清单。

[![Total views](https://raw.githubusercontent.com/Satellite-OSS/.github/main/traffic/SoftwareEvaluationPlatform/views.svg)](https://github.com/Satellite-OSS/.github/tree/main/traffic/SoftwareEvaluationPlatform "Cumulative recorded repository views; updated hourly")
[![Discussions](https://img.shields.io/badge/Discussions-Join%20the%20Community-2ea44f?style=flat-square&logo=github)](https://github.com/orgs/Satellite-OSS-BUPT/discussions)
[![README](https://img.shields.io/badge/README-English-blue?style=flat-square)](README.md)

[English](README.md) | **中文**

</div>

---

## 📋 关于这份清单

卫星软件研究需要一个能做实验的地方。本仓库收录了十个可作为**评估平台**的开源项目——它们可以用来跑工作负载、做基准测试、复现实验，以及比较卫星计算、组网与调度方面的方案。

本清单中的平台分为两类：

- **社区原创（TBD）** —— 由 OPENSAT 成员自行开发的评估工具，统一放在 [`original tools/`](<original tools/README.md>) 目录下，目前覆盖容器化软件评估与 Wasm（WebAssembly）软件评估等。
- **第三方链接** —— 由其他团队维护的开源项目，在此作为现成的评估平台推荐。

---

## 🎯 入选标准

1. 与卫星软件评估场景直接相关
2. 有真实可运行的源代码
3. 至少支持一条评估流程：基准测试、实验复现、策略对比或系统性能分析

---

## 第三方评估平台

下面大致按项目与卫星本体的距离排序：从卫星边缘计算与星座组网，到在轨基准测试与航天动力学，再到地面段工具。

### 1️⃣ SatEdgeSim

[SatEdgeSim](https://github.com/wjy491156866/SatEdgeSim) 用于对卫星边缘计算建模，最常见的用法是比较不同调度策略在时延、吞吐和资源占用上的表现。

### 2️⃣ StarPerf-Satellite-Simulator

[StarPerf-Satellite-Simulator](https://github.com/zhanghefan123/Starperf-Satellite-Simulator) 关注大规模星座的组网性能，适合做路由、拥塞和链路动态相关的实验。

### 3️⃣ STAR-Bench

[STAR-Bench](https://github.com/necst/STAR-Bench) 是一个面向在轨视觉任务的基准测试与试验床，核心是在精度、鲁棒性与算力开销之间做权衡比较。

### 4️⃣ LuPNT

[LuPNT](https://github.com/Stanford-NavLab/LuPNT) 提供空间导航方向的仿真与实验平台，主要用于评估 PNT 算法并复现场景。

### 5️⃣ EOS-Bench

[EOS-Bench](https://github.com/Ethan19YQ/EOS-Bench) 把对地观测卫星的调度实例汇集到同一套基准里，让不同调度算法可以在相同实例和指标下比较。

### 6️⃣ Basilisk

[Basilisk](https://github.com/AVSLab/basilisk) 是一个高保真的航天器动力学框架，常用于 GNC 验证、闭环实验和性能分析。

### 7️⃣ poliastro

[poliastro](https://github.com/poliastro/poliastro) 是一个 Python 航天动力学库，适合做轨道算法实验、批量参数研究和快速原型验证。

### 8️⃣ Orekit

[Orekit](https://github.com/CS-SI/Orekit) 是一个用 Java 编写的高精度航天动力学与轨道计算库，可作为轨道递推、确定和估计评估的基线。

### 9️⃣ CubeSatSim

[CubeSatSim](https://github.com/alanbjohnston/CubeSatSim) 对 CubeSat 做端到端仿真，可用于通信链路评估、任务流程验证以及教学和科研实验。

### 🔟 AIT-Core

[AIT-Core](https://github.com/NASA-AMMOS/AIT-Core) 是地面任务操作与测试框架的核心，用于支持指令与遥测校验、集成测试和实验自动化。

---

## 🤔 如何选择

- 做**卫星边缘计算研究**：SatEdgeSim、StarPerf
- 做**基准测试类工作**：STAR-Bench、EOS-Bench
- 做**航天动力学仿真评估**：Basilisk、Orekit、poliastro
- 做**地面系统与任务流水线实验**：AIT-Core、CubeSatSim

---

## 🤝 参与贡献

研究人员、开发者、学生和卫星爱好者都欢迎加入。如果你知道有项目应该出现在这份清单里，欢迎提交 pull request，或在 Discussions 里发起讨论。
👉 **[Join the Discussions](https://github.com/orgs/Satellite-OSS-BUPT/discussions)**

---

## 📄 许可

本文档是一份导航式的资源汇总。各项目的许可证与版权仍归其原始仓库所有。
