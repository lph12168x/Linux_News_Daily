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
