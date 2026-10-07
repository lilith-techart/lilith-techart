# Lilith / Technical Art

**Technical Art / Real-time Graphics / Interactive Media**

广州美术学院湾区创新学院，**科技艺术方向本科生**。我用 UE / Unity、Shader 与实时渲染开展技术实践，把视觉效果、交互反馈和验证方法组织成可解释、可比较的系统。

## Featured Projects

### 1. [SoftMatter / STMS](https://github.com/lilith-techart/SoftMatter-STMS)

如何把厚度、透光、湿润高光、形变、损伤与多主体绑定组织成可复用的软材质研究系统？

**Implemented / verified**：jelly optical prototype、Profile / Preset、spring motion、local deformation、single-mesh visual soft tear / regeneration，以及 M2-A explicit subject binding；后者已通过 compile/import、M1-F preset 与 M1-G lifecycle regression。

**Current research**：jellyfish generalization 已进入实现阶段，但 bell / tentacle geometry、multi-renderer look 与 hero capture 尚未完成验证。scattering 是艺术化近似，tear 不改变拓扑，也不是 FEM soft-body simulation。

<img src="https://raw.githubusercontent.com/lilith-techart/SoftMatter-STMS/main/media/jelly-optics-cover.png" alt="STMS procedural jelly optical comparison, current validated hero while jellyfish visual validation remains in progress" width="680">

### 2. [FluidMatter Water](https://github.com/lilith-techart/FluidMatter-Water)

如何让波面、深度、光学与边界共享一致数据？

**Implemented**：Unity URP、Linear Eye Depth、screen-space refraction、Beer–Lambert transmittance、reflection preview、Gerstner、SurfaceData、boundary field、Profile / binding / cache。

**Research Prototype**：W3.0 Boundary Field 已有验收证据；**WIP**：W3.1 Shoreline & Foam consumer，尚未通过自身验收。

**Visual status**：真实 water-scene HERO 与 actual-run short demo 仍为 **NEEDS_CAPTURE**。在拿到真实水景前，不再用 Gerstner debug mesh 充当项目主视觉；现有技术图保留在项目仓库的 Debug & Validation 区。

### 3. [Tidemark](https://github.com/lilith-techart/Tidemark)

如何让环境视觉迭代保留可走路线与可替换资产结构？

**Implemented**：UE 场景 construction、visual / collision separation、相机输出与历史角色遍历验证。

**WIP**：First Art Pass awaiting human review；未作为最终环境成品。

<img src="https://raw.githubusercontent.com/lilith-techart/Tidemark/main/media/first-art-pass.png" alt="Tidemark First Art Pass scene capture, WIP" width="680">

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
