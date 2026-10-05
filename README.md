# 🧭 Experience-Sharing · 经验分享

> 一个用于**学习与分享**的个人开源仓库 📚，记录我在 **机械臂机器人 🤖**、**VoCat 硬件复刻 🔧** 等方向上的学习笔记、资料整理与踩坑经验。
>
> 仓库按「**软件 / 硬件 / 文档**」三块组织：**软件资料 → [`code/`](code/) · 硬件资料 → [`hardware/`](hardware/) · 学习 / 复刻文档 → [`doc/`](doc/)**

[![GitHub 仓库](https://img.shields.io/badge/GitHub-Experience--Sharing-181717?logo=github&style=flat-square)](https://github.com/OoOZzZzzzz/Experience-Sharing)
[![License](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)
[![主题](https://img.shields.io/badge/主题-机械臂·嵌入式·硬件-FF6F00?style=flat-square)](#)
[![状态](https://img.shields.io/badge/状态-持续更新-2ea44f?style=flat-square)](#)

---

## 📑 目录

<a id="toc"></a>

- [📦 仓库结构](#structure)
- [📖 文档导航](#docs)
  - [🤖 机械臂开源项目研究笔记](#robot-arm)
  - [🔧 VoCat 复刻文档](#vovat)
- [🧭 建议学习路线](#roadmap)
- [📁 子目录入口](#subdirs)
- [📜 开源许可](#license)
- [📝 更新日志](#changelog)

---

## 📦 仓库结构

<a id="structure"></a>

```text
Experience-Sharing/
├── README.md            # 📖 仓库总览（本文件）
├── LICENSE              # 📜 MIT 开源许可
├── code/                # 💻 软件资料（上位机 / 固件 / 示例代码）
├── hardware/            # 🔌 硬件资料（原理图 / PCB / 官网硬件）
└── doc/                 # 📚 学习文档与复刻文档
    ├── 机械臂.md        # 🤖 机械臂开源项目研究笔记（核心文档）
    ├── Vocat复刻文档.md  # 🔧 VoCat 硬件复刻全流程记录
    ├── image/           # 🖼️ 文档插图
    └── back/            # 🗄️ 本地备份（已被 .gitignore 忽略，不随仓库推送）
```

| 目录 | 存放内容 | 入口 |
| --- | --- | --- |
| 💻 [`code/`](code/) | 软件资料：上位机 / 固件 / 示例代码 | [`code/readme.md`](code/readme.md) |
| 🔌 [`hardware/`](hardware/) | 硬件资料：原理图 / PCB / 官网硬件 | [`hardware/readme.md`](hardware/readme.md) |
| 📚 [`doc/`](doc/) | 学习文档与复刻文档 | 见下方 [📖 文档导航](#docs) |

---

## 📖 文档导航

<a id="docs"></a>

### 🤖 机械臂开源项目研究笔记

> 📄 入口：[`doc/机械臂.md`](doc/机械臂.md) ｜ 🖼️ 插图：`doc/image/`

面向**新手 → 进阶**的机械臂开源项目研究笔记，帮你从「看个热闹」🚶 到「动手复刻」🔧。

- 🧠 **机械臂核心知识速览**：自由度（DoF）、驱动方式选型（舵机 / 步进 / 无刷伺服）、减速器（行星 / 谐波 / RV）、零基础学习路线
- 🚀 **开源项目大观**：从千元级 LeRobot / SO-ARM100 到终极目标稚晖君 Dummy-Robot，共 9 个项目的选型对比、视频、项目地址与完整 BOM
- 🎯 **选型速查表**：一屏对比各项目的成本 / 精度 / 难度 / 推荐度

![六自由度机器人](doc/image/六自由度机器人.png)

### 🔧 VoCat 复刻文档

> 📄 入口：[`doc/Vocat复刻文档.md`](doc/Vocat复刻文档.md) ｜ 💻 软件：[`code/readme.md`](code/readme.md) ｜ 🔌 硬件：[`hardware/readme.md`](hardware/readme.md)

VoCat 硬件复刻的全流程记录：从官方开源硬件（echoear）出发，覆盖 **PCB 焊接（0402 封装）**、**热风枪 / 烙铁焊接工艺**、**电源板 / 主板焊接要点**、**固件烧录** 等完整环节，以及大量避坑经验。

![VoCat](doc/image/VoCat.gif)

> ⚠️ 复刻有风险，焊接需谨慎。手残党建议先从大封装练手 😄

---

## 🧭 建议学习路线

<a id="roadmap"></a>

**想玩机械臂 🤖：**

1. 📖 读 [`doc/机械臂.md`](doc/机械臂.md) 的「机械臂核心知识速览」建立认知框架
2. 🚀 对照「开源项目总览」按预算 / 目标选型
3. 🔧 从低成本舵机臂练手 → LeRobot 玩遥操作 → 挑战步进电机高精度臂
4. 🏆 终极目标：复刻稚晖君 Dummy-Robot

**想玩嵌入式 / 硬件焊接 🔧：**

1. 🔌 看 [`hardware/readme.md`](hardware/readme.md) 了解开源硬件来源
2. 📖 跟 [`doc/Vocat复刻文档.md`](doc/Vocat复刻文档.md) 走一遍焊接流程
3. 💻 到 [`code/readme.md`](code/readme.md) 取软件资料，烧录 + 调通

---

## 📁 子目录入口

<a id="subdirs"></a>

| 目录 | 说明 | 当前内容 |
| --- | --- | --- |
| [`code/`](code/) | 💻 软件资料 | 上位机 / 固件等，详见 [外部软件仓库](https://github.com/OoOZzZzzzz/VoCat_Replication/tree/master/software) |
| [`hardware/`](hardware/) | 🔌 硬件资料 | 原理图 / PCB 等，详见 [官网开源硬件](https://oshwhub.com/esp-college/echoear) |

---

## 📜 开源许可

<a id="license"></a>

本仓库采用 [MIT License](LICENSE) 开源。

> 仓库中引用的外部项目、视频、网盘资料版权归原作者所有，仅供学习交流使用 🔖。

---

## 📝 更新日志

<a id="changelog"></a>

| 日期 | 更新内容 |
| --- | --- |
| 2026-10-05 | 新增仓库总览 README；机械臂文档重构为 GitHub 友好版 |
| 2026-10-04 | 机械臂文档大改：补充核心知识速览、选型对比、学习路线 |

---

> 🧡 如果这个仓库对你有帮助，欢迎 **Star ⭐** 或 **Fork 🍴**，也欢迎提 [Issue](https://github.com/OoOZzZzzzz/Experience-Sharing/issues) 一起交流。