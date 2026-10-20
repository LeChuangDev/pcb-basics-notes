# LeChuang PCB Basics Notes
> 樂創 PCB 与无源器件系统学习笔记

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)]()
[![main branch](https://img.shields.io/badge/branch-main-blue?style=flat-square)]()

## 📌 仓库概述
本仓库为硬件学习知识库，全部使用 Markdown 文档编写。
内容聚焦**无源器件基础**、**PCB基础理论**与**工程实操知识**，用于系统沉淀硬件底层知识，记录器件选型逻辑、公式推导、电路与PCB调试踩坑复盘，为模拟电路、电源PCB、高速信号链路设计打下基础。

> ⚠️ 仓库存放内容：Markdown笔记、原理示意图、工程计算表格。
> EDA完整工程、超大器件手册PDF不放在此仓库，工程文件单独存放在其他仓库。

## 📚 知识目录结构
```
pcb-basics-notes/
├── 01_Passive_Components/        # 无源器件【核心】
│   ├── Resistor/                 # 电阻：类型、功率、温漂、噪声、高频特性、选型
│   ├── Capacitor/                # 电容：介质分类 (MLCC / 电解 / 薄膜)、ESR/ESL、温度特性、去耦原理
│   ├── Inductor/                 # 电感：DCR、饱和电流、磁芯选型
│   └── Magnetic_Bead/            # 磁珠原理，与电感区分，高频噪声抑制
├── 02_PCB_Fundamentals/          # PCB 基础
│   ├── PCB_Material/             # 板材：FR4，介电常数，Tg，铜箔厚度
│   ├── Stackup_Design/           # 叠层设计，阻抗控制基础
│   ├── Trace_Routing/            # 走线宽度、载流、阻抗、走线工艺
│   └── Via_Design/               # 过孔：通孔 / 盲埋孔，孔径焊盘，寄生参数
├── 03_Layout_EMC/                # 布局、EMI & EMC 基础
│   ├── Layout_Rules/             # 布局基础原则，电源地分割
│   ├── Ground_Design/            # 地平面、单点接地、多点接地
│   └── EMI_Suppression/          # 干扰来源与抑制手段
├── 04_Engineering_Calc/          # 工程计算模板
├── 05_Debug_Record/              # 硬件调试踩坑记录
├── Attachments/                  # 图片、示意图、波形截图
├── README.md
└── .gitignore
```
## 📖 文档规范
1. 文档使用 Markdown，VS Code / Typora 均可打开编辑
2. 目录采用英文命名，笔记文件使用中文标题，方便检索阅读
3. 图片统一放置在 `Attachments` 文件夹内，笔记使用相对路径引用图片

### Git 提交规范（Conventional Commits）
feat: 新增章节 / 笔记
docs: 补充内容、文字修改
fix: 修正公式、概念错误
refactor: 调整目录结构

示例：
- `feat: 新增碳膜电阻与金属膜电阻对比笔记`
- `docs: 补充MLCC电容电压降额说明`
- `fix: 修正走线载流计算公式笔误`

## 📜 License
MIT License

笔记为个人硬件学习总结，可供自由参考学习。
工程设计时，请以器件官方datasheet与行业规范为准。

## 📫 About Author
LeChuang (樂創)
Hardware Engineering Student | Embedded & PCB Design Learner
