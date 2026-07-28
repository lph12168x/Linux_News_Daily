# Linux 图形·显示·计算 每日动态

> 自动化追踪 Linux 生态中 GPU 驱动、图形栈、显示协议与高性能计算领域的最新进展。

## 项目简介

每日通过 AI 自动筛选 Linux 领域 **3–5 条高价值动态**，侧重以下方向：

- **GPU** — AMDGPU、Intel Xe、NVIDIA Nova/Mesa、Vulkan 驱动
- **显示** — Wayland、Weston、HDR、分数缩放
- **计算** — NPU 加速器、RDMA、内核调度、AI 推理
- **内核** — Linux 合并窗口、DRM 子系统、Rust-for-Linux

每期以美观的深色主题 HTML 仪表盘呈现，包含事件摘要与**关注理由**。

> 在线浏览：[lph12168x.github.io/Linux_News_Daily](https://lph12168x.github.io/Linux_News_Daily/)

## 浏览日报

| 日期 | 主题亮点 |
|------|----------|
| [2026-07-29](linux-news-2026-07-29.html) | AMD P-State 按核 EPP boost 补丁：游戏 1% Low 帧率提升 31.8%（Meta 工程师 David Vernet 提交 amd_pstate.epp_boost：每 10ms 采样核心 C0 占用率、繁忙即临时置 EPP=performance、300ms 静默恢复，Steam Deck《文明 6》1% Low +31.8%、p99 帧时间 +4.1%，避免全局 EPP=performance 烧掉掌机 CPU/GPU 共享功耗预算）· Starling：Swift 编写的全新 Linux 桌面（自研 C 语言 Wayland 合成器 + 内置 X11 服务器免 XWayland，主要由 Claude AI 辅助编写）· Ryzen AI 9 HX 470 "Gorgon Point" 四系统横评（BOSGAME VTA-439：近 100 项基准几何平均 CachyOS 领先 Windows 11 约 11%、仅快 Ubuntu 26.04 约 1%，Llama.cpp Vulkan 后端 Linux 更快） |
| [2026-07-28](linux-news-2026-07-28.html) | 神秘厂商披露 16-Tile 与 32-Tile AMX 实现（x86 专家 Christian Ludloff「受托」在 LKML 公开文档：Intel 迄今仅 8-tile，「16/32 tile 实现已大规模运行一段时间」，委托方系 Intel/AMD 之外的企业实体、身份成谜，正值 AMX 演进 ACE 关口）· AMD「低功耗」第三种 CPU 核心类型补丁进入 Linux 7.3（TOPO_CPU_TYPE_LOW_POWER 合入 tip x86/cpu，为 Zen 6 客户端低功耗核正确调度铺路）· Wayfire 0.11 发布（v1.0 前最后一版：显式同步、security-context-v1/ext-copy-capture 等协议、XWayland 与触控改进）· Framework Laptop 13 Pro 评测（Panther Lake + Arc B390、CNC 铝机身、LPCAMM2、74Wh，Ubuntu 26.04 开箱即用）· NVIDIA 等二十余家公司成立 Open Secure AI Alliance（构建于 LF Akrites/OpenSSF，保障开源 AI 模型安全） |
| [2026-07-27](linux-news-2026-07-27.html) | Linux 7.2-rc5 发布（Linus：「再次迎来相当庞大的 -rc5」，网络补丁超三分之一、罕见 USB 变更多于 GPU 驱动、修复 2009 年以来 Firewire IPv4 老 bug，稳定版预计 8 月 16 日）· 「KVM 电锯」重构预计进 Linux 7.3（Paolo Bonzini 将 kvm-chainsaw 合入 next：把承担三种职责的 kvm_mmu「上帝数据结构」拆为 kvm_pagewalk/kvm_mmu/kvm_page_format，为 XS!=XU SPTE 铺路）· GNU Binutils 2.47 发布（新增 zvqwdota/zvfwdota 等大批 RISC-V 向量点积扩展与 SpacemiT xsmtvdot、BFD 链接器 -O 0 快速模式、弃用 32 位 s390）· Ubuntu Touch 24.04-2.0（Lomiri 支持刘海屏与圆角显示、Morph 浏览器 Chromium 87→134、FSCRYPT v2 加密转正） |
| [2026-07-26](linux-news-2026-07-26.html) | glibc 2.44 发布（引入 /etc/tunables.conf 系统级可调参数持久配置、x86_64 FMA cosh 提速约 35%、导入 CORE-MATH 正确舍入数学函数、LoongArch 优化 + LoongArch32 首次支持、AArch64/RISC-V 优化，将进入 Ubuntu 26.10/Fedora 45）· KDE Plasma 6.8 引入 kscreenctl 屏幕控制工具（取代 kscreen-doctor 管理显示输出配置；同周修复新款 NVIDIA GPU + 色彩管理组合 KWin 登录崩溃、RDP 断开自动锁屏）· Wine 11.14 发布（WoW64 模式初步登陆 FreeBSD、开始菜单支持图标、DirectSound 7.1 声道转换、BCrypt AES-GMAC，修复《风暴英雄》《帝国时代 I/II》等 21 个 bug） |
| [2026-07-25](linux-news-2026-07-25.html) | Imagination PowerVR 驱动将 BXM-4-64 MC1 GPU 从「实验性」提升为「已支持」、随 Linux 7.3 落地（配合 Mesa Vulkan 跑通 Vulkan CTS + 固件上游，为 T-Head TH1520 等 RISC-V 板卡带来完全上游开源 GPU 栈）· AMD ROCm 转向固定六周发布周期（紧随首个 TheRock 生产版 7.14，下个 8 月版本携 ROCm.AI）· Snapdragon X Elite 在 Ubuntu 26.04 LTS 图形进一步回退（qcom-firmware-extract 需手动升级、Adreno GPU 跌回 LLVMpipe 软件渲染、Linux 7.0 下 MSM DRM 初始化报错）· AMD Advancing AI 2026「开源/开放」为主线（Kria 公开硬件原理图、Robotics Suite 与 FPGA RTL 开源、Helios 网络基于 SONiC、OpenSIL 在 Zen 6 达生产、OpenBMC 续用） |
| [2026-07-24](linux-news-2026-07-24.html) | AMD Advancing AI 2026 大爆发：发布 Instinct MI455X + Helios 机架（2nm、432GB HBM4、峰值 MXFP8/MXFP4 达 MI355X 4 倍，机架 4600 CPU 核 + 18000 GPU CU）· 宣布面向开发者的 ROCm.AI 平台 · 正式发布 EPYC 9006 "Venice"（Zen 6C 最高 256 核/512 线程、DDR5-8000 + MRDIMM-12800、PCIe Gen6、AVX-512 BMM）· 确认 EPYC Zen 7 "Florence" 带 ACE AI 计算扩展、Zen 8 "Ravenna" 研发中 · Ryzen AI Software 1.8（低内存跑更大模型）· LLVM 23.1-rc1（AMD Zen 6/AVX-512 BMM、AMDGPU GFX1310、HIP 卸载驱动） |
| [2026-07-23](linux-news-2026-07-23.html) | SDL 落地 HDR10 渲染支持（SDL3 的 D3D11/D3D12/Vulkan 渲染器现支持 HDR10 显示，延续 SDL3 colorspace 与 Wayland 色彩管理铺垫）· System76 发布 COSMIC Epoch 1.4（Rust 桌面大量修复、合成器修正输入/窗口与分数缩放指针精度、COSMIC Monitor 新增强制退出与 GPU 频率采集）· libx11-compat 在 SDL2/SDL3 之上进程内重建 Xlib（无需 X Server 即可运行 XMosaic/Qt2/XCircuit/XMMS 等经典 X11 程序，覆盖纯 Wayland/macOS/Android）· Raspberry Pi Touch Display 2 推出 10 英寸型号（1200×1920、十点触控、$80） |
| [2026-07-22](linux-news-2026-07-22.html) | Intel 显卡「冷复位恢复」机制成型（DRM 新增冷复位楔形恢复、Xe 驱动先行，处理 PUNIT 等需整机掉电才能清除的 GPU 错误）· KDE Plasma 6.7 vs GNOME Shell 50.3 vs Xfce 4.20 桌面横评（CachyOS + NVIDIA RTX 5090，Xfce Wayland 仍黑屏只能走 X11）· Intel Compute Runtime 26.27.39122.11 持续推进实验性 LEO（OpenCL 重构于 Level Zero 之上、新增 AVX2/AVX-512 内存拷贝优化）· AMD 为 Zen 6 准备更多 EILVT 寄存器（EILVT 表 4→8 项、增强 Linux perf/IBS 性能剖析） |
| [2026-07-21](linux-news-2026-07-21.html) | KNOD：网络卸载直接进 AMD GPU（无需 ROCm、完全内核态下沉 XDP/IPsec 包处理）· Linux 7.2 提升 Panther Lake Xe3 Arc B390 图形性能（对比 7.1 实测）· AMD 谈 ROCm 中 SPIR-V IR 机遇（统一二进制跨 GPU 可移植）· Firefox 153 支持 Vulkan 视频解码 + 实验性 JPEG-XL（同时是 ESR）· Hyprland 0.56 发布（滚动/master 布局 + Lua API）· AMD 提交 AVX10_V2_AUX GCC 补丁（FP4/FP6/FP8 转换加速 AI/ML） |
| [2026-07-20](linux-news-2026-07-20.html) | Linux 7.2-rc4 发布（修复节奏进入「新常态」、AMDGPU 仍是 diff 噪声大户、AI 辅助修复常态化）· FFmpeg 落地 AVX-512 VPERMB 优化（RGB24→RGBA 1920×1080 转换快 1.372×，惠及 Zen 4+/Xeon）· 联想 Legion Y700 Gen4（骁龙 8 Elite）现身 Linux 支持补丁（frame-buffer 显示可用、下游可驱动 Adreno GPU 与触摸屏） |
| [2026-07-19](linux-news-2026-07-19.html) | NVK（Mesa 26.2）持续逼近 NVIDIA 闭源 Vulkan 驱动（Serious Sam 2017 已极接近）· AMDGPU DC 70 补丁修复 Apple Studio Display 5K 屏（隐藏第二条 tiled link）· oneDNN 3.13 为 Intel Nova Lake（AVX10.2）+ AMX Xeon + Xe3P-LPG/Arc B 优化 · D7VK 2.0 老 D3D 性能翻倍（Half-Life 19→59 FPS）· DXVK 3.0.2 游戏修复 + DXVK_DEBUG=hang 调试钩子 |
| [2026-07-18](linux-news-2026-07-18.html) | AMD 为 Linux 7.3 准备更多图形/计算驱动（DCN4.2·GFX12.1·OLED 省电·8K@240 修复）· FastFlowLM 团队加入 AMD 助推开源 NPU 软件 · OpenBLAS 0.3.34 多线程优化 + Fil-C 内存安全编译 · Arm Core Local Accelerator 驱动 RFC（加速器通用接口）· Mozilla Llamafile 0.10.4 新增 Transcribefile 语音转写 · Frame：纯 x86_64 汇编写的 X11 服务器 |
| [2026-07-17](linux-news-2026-07-17.html) | Wayland 1.26 正式发布（新增 wl_pointer.warp 修复指针位置错判）· Ubuntu 内核团队警告下一版 7.0.0-28.28 含 AMD GPU 计算回退最高慢 42×、上游 7.0.13 已修 · KDE KWin 引入服务端阴影将于 Plasma 6.8 落地 · AMD GAIA 0.22 本地 AI 邮件代理（仿写风格、cron 调度，含 Linux）· Imagination PowerVR BXM-4-64 固件上游化解锁 T-Head TH1520 RISC-V 板卡 GPU · AMD Ryzen 7 7700X3D Linux 性能评测（最便宜 3D V-Cache） |
| [2026-07-16](linux-news-2026-07-16.html) | Mesa 26.2-rc1 发布（本季度图形栈特性冻结、开放 26.3 开发，ANV/RADV/NVK/Rusticl 多线增强、OpenCL 3.1 落地、KRAID 编译器合入 Panfrost）· AMD Lemonade 11.0 本地 AI 服务新增文本转语音（声音克隆）+ 3D 生成、Linux 上 FastFlowLM NPU 后端自动安装 · Ubuntu 26.04 vs Windows 11 vs CachyOS 顶配游戏本横评（Razer Blade 18 / RTX 5090）· Linus Torvalds 重申 Linux 非「反 AI」项目、AI 仅是工具 · 首个 OpenCL 3.1 一致性实现：Apple M1/M2 经 Asahi Linux + Rusticl 通过 |
| [2026-07-15](linux-news-2026-07-15.html) | Weston 16.0 合成器发布，HDR 改进与 Vulkan 渲染器修复（Wayland 参考实现）· Intel ANV Vulkan 驱动新增 H.265 10-bit 视频编码（Igalia，Vulkan Video）· 开源软 GPU GlandaGPU 提交 Linux DRM 内核驱动 RFC（FPGA VHDL 全链路开源）· Intel 图形编译器 IGC 2.38.2 编译优化 · System76 Adder Pro 笔记本（NVIDIA 独显 + 2K OLED + 最高 96GB）· Blender 5.2 LTS 发布 |
| [2026-07-14](linux-news-2026-07-14.html) | AWS Graviton5 性能评测超 Intel Xeon Granite Rapids、仍不及 AMD EPYC Turin（Arm Neoverse-V3 vs x86 服务器 CPU，Ubuntu 26.04）· System76 COSMIC 桌面推出 Frosted Glass 磨砂玻璃视觉效果（cosmic-comp Wayland 合成器，系统级模糊）· Linux 7.3 将迎来 Thomas Gleixner 系统调用入口处理重构（统一架构栈随机化、小幅性能提升） |
| [2026-07-13](linux-news-2026-07-13.html) | Linux 7.2-rc3 发布，逼近 8 月稳定版（一半改动为驱动、含 AI 辅助补丁，将为 Ubuntu 26.10 内核基础）· Linux 7.2 默认内核构建启用 UltraRISC RISC-V 支持（UR-DP1000 八核 C100 进 defconfig）· 知名 LLVM/Clang 内核开发者 Nick Desaulniers 回归 Google 重启内核贡献 |
| [2026-07-12](linux-news-2026-07-12.html) | Linux 7.2-rc3 改进多 GPU 系统显示检测逻辑（AMD+NVIDIA 双显卡主显示判定修复）· LLVM 合并 x86 LFI 轻量级故障隔离目标（进程内沙箱，Spec2017 仅 2~7% 开销）· KDE Plasma 6.8 落地 Spectacle 音频录制 / vRAM 百分比监控等 · Mesa 26.2 Rusticl 默认启用 Arm Mali Panfrost 驱动支持 |
| [2026-07-11](linux-news-2026-07-11.html) | Linux 7.3 为 GFX11 AMD APU 启用第二图形管道（pipe1，RDNA3/3.5）· Intel ANV Vulkan 合并 HiZ Plane 优化（Mesa 26.2，游戏帧率 +1~3%）· LLVM/Clang 合并 NVIDIA Rigel 核心（下一代 Rosa CPU）初始支持（-mcpu=rigel）· Intel-Scaler-vLLM 0.21.0-b1 发布（XPU graph + Gemma 4 模型）· KDE Plasma 6.7 X11 vs Wayland NVIDIA 游戏性能对比（CachyOS）· Linux DT 补丁为 Apple M3 Pro/Max/Ultra 提供基础启动支持 |
| [2026-07-10](linux-news-2026-07-10.html) | AMDGPU DC 启用 CACP 为 OLED 屏省电（含 DCN42b PSR/Panel Replay/IPS 与 8K 时序修复）· Wayland 1.26 RC1 新增 wl_pointer.warp 修正指针坐标 · AMD Ryzen AI Halo（Strix Halo）RGB 灯带驱动 v8 接近主线 · Apple M4 初始 DT 补丁发布（仅能启动、GPU 加速未就绪） |
| [2026-07-09](linux-news-2026-07-09.html) | AMD ZenDNN 6.0 CPU 推理加速（MoE/FP16/权重缓存）· Linux Mint Cinnamon Wayland 不再实验性 · XWayland 24.1.13 修复 GLAMOR/GLX 安全漏洞（CVE-2026-55999/56000）· Intel 归档 Quantum Intrinsics/OAP-MLLIB 等开源 AI 项目 · Arrow Lake 单/双通道内存基准 |
| [2026-07-08](linux-news-2026-07-08.html) | Valve Proton 11.0-1 稳定版（基于 Wine 11.0）· AMD 30 补丁清除 AMDGPU BUG() · NVIDIA Rigel 核心进 GCC · NVIDIA Rosa CPU Rigel 核心细节 · NVIDIA 610.43.03 Linux 驱动 · Razer Blade 18 首款 Linux 认证笔记本 |
| [2026-07-07](linux-news-2026-07-07.html) | Microsoft Mesa 26.2 落地 DX12+HMFT AV1 编码 · Intel ANV Alchemist Vulkan Video H.264/H.265 编码 · Marek RADV VRS 重构部分场景性能翻倍 · Linux 7.3 "Flatten The Pick" 调度改进游戏帧率 · Intel i915 接近支持 RT 实时内核 · D7VK 1.12 老 D3D 性能提升 |
| [2026-07-06](linux-news-2026-07-06.html) | AMD Linux 7.3 图形/计算驱动提交（RDNA3/4 计算管道重置、DCN 4.2）· DXVK 3.0.1 游戏渲染修复 · Linux 6.19 修复 4K@60FPS USB 采集卡带宽降级 · GNOME Mutter 合并 ext-background-effect-v1 背景模糊 · KDE Plasma 6.8 KWin 仅保留 OpenGL ES |
| [2026-07-05](linux-news-2026-07-05.html) | Linux 7.3 Nova Lake S PCI ID 新增 · DRM调度器kthread_work优化大幅降低提交延迟 · Vulkan 1.4.356 OCP Microscaling MX格式扩展 · NVIDIA VR-NVL BMC OpenBMC上游化 · Rusticl OpenCL硬件利用率提升 |
| [2026-07-04](linux-news-2026-07-04.html) | Mutter GPU重置恢复（GSoC 2026）· Vulkan 1.4.356 OCP Microscaling MX格式扩展 · Intel Nova Lake CMTG/DC3CO显示支持 · NVIDIA VR-NVL BMC OpenBMC上游化 |
| [2026-07-03](linux-news-2026-07-03.html) | Intel ACE x86 AI计算扩展GCC补丁 · Rusticl OpenCL硬件利用率提升 · YSERVER 1.3 Rust X11服务器Xinerama支持 · RADV/RadeonSI修复AMD GCN 1.0/1.1 L2缓存VM故障 · RISC-V RVV 1.0向量性能基准测试 |
| [2026-07-02](linux-news-2026-07-02.html) | Nova TLV固件格式 · COSMIC Epoch 1.2 Intel显卡闪烁修复 · AMD GCN 1.0/1.1 驱动VM故障修复 · Linux 7.3 DRM色彩格式属性 · Intel取消AMX-TF32 · Gen5 NVMe小I/O性能提升 |
| [2026-07-01](linux-news-2026-07-01.html) | Q2总结特刊：Intel Arc Pro B70 32GB显存 · Linux 7.2-rc1 AMDGPU HDMI 2.1 FRL · Mesa 26.2 Vulkan Present Timing/NVK DLSS · Wine Wayland 指针偏移/分数缩放 · AMD Linux AI生态 |
| [2026-06-30](linux-news-2026-06-30.html) | Wine 11.12 Wayland 分数缩放 · RADV 默认启用描述符堆 · ZLUDA v6 PhysX 支持 · Linux 7.2-rc1 发布 · Nourish Vulkan 合成器 |
| [2026-06-29](linux-news-2026-06-29.html) | Linux 7.2-rc1 发布 · CVE-2026-53293 AMDGPU 死锁修复 · Intel HDR over DP MST · DXVK 3.0 发布 · Nourish Vulkan 合成器 |
| [2026-06-26](linux-news-2026-06-26.html) | Mesa 26.2 Present Timing · Valve RTI 光追检查器 · NVK DLSS 支持 · Linux 7.2 Blackwell-Next · AMD Gamma 2.4/2.6 |
| [2026-06-25](linux-news-2026-06-25.html) | Linux 7.2 合并窗口 · NVK DLSS 支持 · Xfce Wayland Alpha · AMD Gamma 曲线 |
| [2026-06-24](linux-news-2026-06-24.html) | sched_ext 源码重构 · EPYC Sorano 意外性能 · ROCDXG WSL · Xfce Wayland Alpha |
| [2026-06-23](linux-news-2026-06-23.html) | Valve RTI 光追调试 · Steam Machine $1049 上市 · Mesa 26.2 Present Timing · Blackwell-Next |
| [2026-06-22](linux-news-2026-06-22.html) | NVK DLSS 支持 · CAS 缓存感知调度 · RMR/BRMR RDMA 单跳复制 |
| [2026-06-18](linux-news-2026-06-18.html) | HDMI 2.1 FRL 合入 7.2 · Vino Rust 驱动 · Panther Lake Xe3 性能 |
| [2026-06-17](linux-news-2026-06-17.html) | Linux 7.1 正式发布 · Nova Lake NPU 早期支持 · Weston 16 Alpha HDR |

## 本地阅读

```bash
git clone https://github.com/lph12168x/Linux_News_Daily.git
cd Linux_News_Daily
# 用浏览器打开任意 .html 文件即可
```

## 自动化说明

本项目由 WorkBuddy 自动化引擎每日定时生成并推送，无需人工干预。

---

*专注 Linux 图形与计算，记录开源驱动的每一次进步。*
