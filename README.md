# Lilith / Technical Art

**Technical Art / Real-time Graphics / Interactive Media**

广州美术学院湾区创新学院，**科技艺术方向本科生**。我用 UE / Unity、Shader 与实时渲染开展技术实践，把视觉效果、交互反馈和验证方法组织成可解释、可比较的系统。

## Featured Projects

### 1. [SoftMatter / STMS](https://github.com/lilith-techart/SoftMatter-STMS)

如何把厚度、透光、湿润高光、形变、损伤与多主体绑定组织成可复用的软材质研究系统？

**Implemented / verified**：单一 shader core 的光学模型（解析厚度 proxy、Beer–Lambert 透光、screen-space 折射、湿润高光、艺术化 back-scatter）、spring 运动与局部接触形变、damage lifecycle 驱动的同网格视觉软撕裂与再生、Material / Motion Profile 与 Preset 系统，以及 M2-A 的显式 subject binding（renderer 成员 / 角色 / per-renderer body metrics）；后者已通过 compile/import、preset 与 fracture lifecycle 的独立进程回归。

**Current research**：第二主体泛化进行中。binding 目前证明的是**不改变既有主体行为**，多 renderer 的 preset look 应用与水母主体的正向验证仍未完成——bell 代码只是未编译草稿，**尚无任何 jellyfish capture**。scattering 是艺术化近似，tear 不改变拓扑，也不是 FEM soft-body simulation。

<img src="https://raw.githubusercontent.com/lilith-techart/SoftMatter-STMS/main/media/jelly-hero.png" alt="STMS validated hero render: translucent jelly with internal pulp, wet highlights and soft scattering" width="680">

### 2. [FluidMatter Water](https://github.com/lilith-techart/FluidMatter-Water)

如何让波面、深度、光学与边界共享一致数据，而不是每个效果各自解释“这里水有多深”？

**Implemented / verified**：Unity URP、Linear Eye Depth 与 validity、screen-space refraction、Beer–Lambert transmittance、reflection **preview**、Gerstner 位移、SurfaceData 契约、boundary field、Profile / binding / shared-material-cache / MPB。

**关键限定**：reflection 是 preview 路径，不是 SSR 或 planar reflection；boundary 目前是**数据契约**，accepted 配置中该特性关闭，没有 production 外观消费它，仓库里的两种 boundary 视觉都是诊断视图。

**Research Prototype**：W3.0 Boundary Field 已通过 15 gates × 2 passes，3,343 条 graded rows、0 FAIL、`isolation_unresolved = 0`；这是有界测试通过，不是全场景与全硬件认证。**WIP**：W3.1 Shoreline & Foam consumer 尚未通过自身验收，precheck 与在写代码都不构成 PASS 声明。

**Visual status**：项目仓库顶部使用一张真实 final-composite 引擎捕获，并明确标注为验证 rig 而非美术成品；带艺术方向的 water-scene HERO 与 actual-run short demo 仍为 **NEEDS_CAPTURE**。不使用生成图像冒充运行结果。

<img src="https://raw.githubusercontent.com/lilith-techart/FluidMatter-Water/main/media/current-build-composite.png" alt="FluidMatter accepted build final composite capture from the W3.0 validation rig, two Gerstner waves active, not an art pass" width="680">

### 3. [Tidemark](https://github.com/lilith-techart/Tidemark)

如何在持续环境重构中保留可走路线、碰撞边界、场景结构与可替换视觉层，并用明确的 retention / rejection 证据决定哪个版本才是真正的“当前状态”？

**Current retained candidate**：**G012** integrated visual blockout。visible architecture density、reference massing、settlement asymmetry、vertical layering、tower grounding、building-terrain integration、access logic 等主要 blockout gate 已达到 **STRONG_PARTIAL**；boardwalk composition、water negative space、protected regression 为 **PASS**。

**Evidence boundary**：真实 Character regression 只验证继承的 G004 collision surface；新 visual terrain / stairs 尚未认证为 production gameplay。**Human Art = PENDING**，未进行 canonical promotion。

<img src="https://raw.githubusercontent.com/lilith-techart/Tidemark/main/media/current-c027-g012.jpg" alt="Tidemark G012 retained visual blockout, current C027 capture" width="680">

## Current Research

- 软半透明材质的视觉线索与交互反馈：从技术机制发展对照方法。
- 水渲染的数据契约、波面与边界场；W3.1 consumer 仍在研发。
- **AFTERIMAGE**：Godot Pixel3D、空间叙事与交互状态，Experimental / WIP，暂未公开工程。
- **SceneValidationCore**：可重放的场景通行与结构化失败检查，Experimental tool，暂未公开源码。

## Study Direction

申请目标：**广州美术学院 140300 设计学学硕，08 数字媒体与影视动画设计理论研究（数媒）方向**。

希望继续深化技术美术、实时图形、引擎与互动媒体实践，同时补足设计研究、数媒理论、文献研究和研究方法，让技术项目形成更完整的研究问题、方法与作品体系。这是我的申请目标与长期方向，不代表录取或已完成研究。

## Technical Stack

Unreal Engine · Unity / Tuanjie · Godot · HLSL / ShaderLab · C# · C++ · GDScript · Python · Git

## Project Status / Links

**Implemented** 表示已有实现与相应证据；**Research Prototype** 表示有界实验；**WIP** 表示仍在研发；**Roadmap** 仅是未来工作。以上项目均未包装为成熟产品。

三个项目仓库是教师与作品集审阅入口。Source/project distribution is not currently provided；公开可见不等于开源许可。

[STMS](https://github.com/lilith-techart/SoftMatter-STMS) · [FluidMatter](https://github.com/lilith-techart/FluidMatter-Water) · [Tidemark](https://github.com/lilith-techart/Tidemark)
