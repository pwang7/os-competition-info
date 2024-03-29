# 使用 eBPF 实现 GPU 虚拟化

### 项目名称

使用 eBPF 实现 GPU 虚拟化

### 项目描述

GPU 是现代计算机中重要的计算资源，往往被用于处理大规模的、计算密集型的任务。然而，由于 GPU 硬件资源的有限性，多个程序可能需要共享同一块 GPU 资源。而当前的 GPU 虚拟化技术存在性能问题，无法满足多租户环境下的 GPU 资源分配和隔离需求。本课题旨在通过 eBPF 技术实现高效、可扩展的 GPU 虚拟化，以提高 GPU 资源的利用率和性能。

本项目旨在利用 eBPF 技术实现一种轻量级的 GPU 虚拟化方案，解决上述问题。使用 eBPF 技术可以在不改变内核的情况下，动态修改系统的行为。eBPF 还提供了强大的安全隔离和性能优化功能，可以用于实现 GPU 虚拟化。

例如，参赛团队可以实现一种基于 eBPF 技术的 GPU 虚拟化方案，通过标签化挂载的 CUDA 指令触发 eBPF 进程进行对 GPU 资源量的执行审计，进而实现多租户环境下的 GPU 资源隔离和分配。

### 所属赛道

2023全国大学生操作系统比赛的“OS功能设计”赛道

### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2023春季学期或之后本科毕业的大一~大四的学生）或研究生
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2023全国大学生操作系统比赛”的章程和技术方案要求

### 项目导师

赖晓铮（华南理工计算机学院）

- Email： [laixz@scut.edu.cn](mailto:laixz@scut.edu.cn)

郑昱笙（浙江大学/DatenLord）

- Email： [yusheng.zheng@datenlord.com](mailto:yusheng.zheng@datenlord.com)

### 难度

- 基础特性的难度：高
- 高级特性的难度：较高

### 基本要求

- 使用 eBPF 技术实现 GPU 虚拟化
- 提供安全隔离和共享设备的功能
- 具备低性能损耗

### 预期目标

**安全隔离和共享设备。** GPU 虚拟化需要考虑到安全隔离和共享设备的问题。参赛团队需要利用 eBPF 技术提供一种轻量级的 GPU 虚拟化方案，使得多个应用程序可以安全地共享 GPU 设备，同时实现安全隔离。

**优化 GPU 虚拟化的性能。** GPU 虚拟化可能会对应用程序的性能产生负面影响。参赛团队需要使用 eBPF 技术对 GPU 虚拟化进行性能优化，使得应用程序可以充分发挥 GPU 的计算能力，同时不会受到虚拟化的性能损失的影响。

**实现更多的特性。** eBPF 技术可以提供更多的特性，如调试和追踪功能，可以帮助用户更好地了解 GPU 虚拟化的性能瓶颈和问题。参赛团队可以尝试实现更多的特性，以提高 GPU 虚拟化的可用性和可扩展性。
