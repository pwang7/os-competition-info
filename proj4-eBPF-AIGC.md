# 搭建性能分析与 eBPF 代码生成的 AIGC 辅助工具

### 项目名称

搭建性能分析与 eBPF 的 AIGC 辅助工具

### 项目描述

本项目旨在针对性能分析的痛点，，使用自然语言处理和语言模型技术，以及现有的性能分析工具和 eBPF 技术，搭建一个更加高效、智能和定制化的性能分析与可观测辅助工具。该工具将利用自然语言描述用户需要进行的性能分析任务，并根据用户需求选择并调用相应的性能分析工具或 eBPF 技术，以完成定制化的性能分析任务。

本项目借鉴了 Toolformer 的思想，即利用语言模型和自然语言处理技术，让大型语言模型微调和学习和使用现成的工具，不需要手动编写或配置性能分析工具，或编写 eBPF 代码。用户只需提供简要的性能分析需求，就可以得到更加高效、智能和精确的性能分析结果。

Toolformer: Language Models Can Teach Themselves to Use Tools
[https://arxiv.org/abs/2302.04761](https://arxiv.org/abs/2302.04761)

现有的性能分析工具非常丰富，但是有很多工具不知道该如何选择，也有很多定制化的场景需要针对内核进行性能分析和观测，可以使用 eBPF 的定制化工具来完成，但手工开发 eBPF 程序的成本很高。本项目旨在利用人工智能和大型语言模型等技术，自动化地生成性能分析流程，或者生成eBPF代码注入内核，以实现交互式的性能分析和可观测，类似于GPTtrace（[https://github.com/eunomia-bpf/GPTtrace](https://github.com/eunomia-bpf/GPTtrace)）。项目需要利用LLM生成各种不同的指令，操纵各种工具（例如perf）并分析它们的返回信息。通过这种方式，参赛者将能够为操作系统开发人员提供一个强大的工具，帮助他们更轻松地识别性能瓶颈和进行调优。

本项目的参赛者需要具备一定的性能分析知识，同时具备 eBPF 编程能力与 prompt 经验。

### 所属赛道

2023 全国大学生操作系统比赛的“OS功能设计”赛道

### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2023春季学期或之后本科毕业的大一~大四的学生）或研究生。
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖。
- 请遵循“2023 全国大学生操作系统比赛”的章程和技术方案要求。

### 项目导师

赖晓铮（华南理工计算机学院）

- Email： [laixz@scut.edu.cn](mailto:laixz@scut.edu.cn)

郑昱笙（浙江大学/DatenLord）

- Email： [yusheng.zheng@datenlord.com](mailto:yusheng.zheng@datenlord.com)

### 难度

- 基础特性的难度：中等
- 高级特性的难度：较高

### 基本要求

- 利用自然语言处理和语言模型技术实现性能分析需求的智能化描述和转换，支持中英文语言输入。
- 支持自动调用常用的性能分析工具，如 perf、top、strace 等，自动分析这些工具的返回信息，并自动选择最优工具以提高分析效率。
- 支持生成 eBPF 代码以进行交互式、定制化的的性能分析和可观测，例如生成 bpftrace 脚本。
- 支持输入输出格式的定制化配置，以适应不同的性能分析场景，或与其他大型平台集成。

### 预期目标

以下是本项目的预期目标，可根据实际情况进行选择其中一些完成。

- 利用大型语言模型技术，实现对性能分析需求的智能化描述和转换。
- 针对不同的性能分析场景，选择并调用最优的性能分析工具，以提高分析效率。例如，对于 CPU 相关的性能分析需求，自动选择 perf 工具；对于 I/O 相关的性能分析需求，自动选择 iotop 工具等。
- 针对用户提供的输入和输出规则，自动生成 eBPF 代码，并且能够进行交互式的性能分析和可观测，提高性能分析的精度和效率。
- 支持输入输出格式的定制化配置，以适应不同的性能分析场景。例如，支持配置输入输出的数据格式、采样间隔、采样时间等。
- 实现可视化的性能分析结果展示，支持图表、列表等形式的展示，并提供交互式的数据过滤和排序功能。
