# 分布式算力网络 | Decentralized Computing Network

我们正在推进一个分布式算力网络，旨在将闲置计算资源转化为可共享、可调用的网络算力。

We are actively building a decentralized computing network to transform idle computing resources into shared, accessible computing power.

## 核心机制 | How It Works

贡献闲置 CPU/GPU 算力，获得积分；需要额外算力时，使用积分调用网络资源。贡献与使用通过统一的积分机制连接。

Contribute spare CPU/GPU capacity to earn credits. Spend credits to access computing resources when needed. A shared credit system connects contributors with users.

例如，AI 企业可以在业务低峰期贡献闲置 GPU，在需求高峰期调用网络算力，减少对自有硬件的依赖。

For example, AI companies could contribute idle GPUs during off-peak periods and access additional capacity during demand spikes, reducing reliance on owned hardware.

## 当前方向 | Current Focus

我们正围绕本地原型、多设备协作、计算任务验证及内部积分机制推进项目，逐步验证核心架构与资源交换模式。

We are working toward a local prototype, multi-device collaboration, task verification, and an internal credit system to validate the core architecture and resource-sharing model.

这是一项正在推进的建设工作。我们希望从可验证的技术原型出发，逐步构建开放的算力协作网络。

This project is actively in development. Our approach is to start with a testable technical prototype and progressively build an open computing network.

让闲置算力成为资源，让贡献成为使用算力的通行证。

Turn idle computing power into a shared resource. Make contribution the key to access.

欢迎关注项目进展，也欢迎对分布式计算、AI 基础设施及开源协作感兴趣的开发者加入讨论。

Follow our progress and join the conversation if you're interested in distributed computing, AI infrastructure, and open-source collaboration.

---

## 技术原型说明（Phase D）

本地、单机、可测试的闲置算力网络原型。聚焦任务协议、状态机、结果验证与互惠积分账本。无任意代码执行、无代币、无真实资金。

### 已实现
- 互惠配额模型（贡献获得积分，提交任务消耗积分）
- 白名单确定性任务：`numeric_batch_v1`、`vector_stats_v1`、`prefix_sum_v1`
- CLI、演示脚本、启动脚本与配置模板
- 基础速率限制
- 抗审查模式设计（优先 Halo2 优化电路）

### 快速演示
```bash
python scripts/demo_quota.py
bash scripts/demo.sh
```

完整设计见 `docs/phase2/PHASE-D-DESIGN.md` 与 `docs/phase2/PHASE-D-README.md`。