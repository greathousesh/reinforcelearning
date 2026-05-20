# 强化学习教程：CartPole 上的 DQN

本仓库提供了一份完整的强化学习（Reinforcement Learning）入门教程，使用 PyTorch 和 Gymnasium 从零实现一个 **深度 Q 网络（DQN）** 来解决经典的 **CartPole（倒立摆）** 控制问题。

## 一键在 Kaggle 运行

点击下方按钮即可在 Kaggle 上打开并运行 notebook：

[![Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://kaggle.com/kernels/welcome?src=https://github.com/greathousesh/reinforcelearning/blob/main/rl_tutorial.ipynb)

## 内容大纲

- **强化学习速览**：智能体、环境、状态、动作、奖励等核心概念
- **环境设置**：使用 Gymnasium 创建 CartPole 环境
- **经验回放（Replay Buffer）**：打破样本相关性，提升训练稳定性
- **Q 网络（DQN）**：三层 MLP 近似 Q 函数
- **DQN 智能体**：ε-greedy 动作选择、目标网络软更新（Polyak averaging）、Huber Loss、梯度裁剪
- **训练循环**：完整的训练流程并实时打印学习进度
- **可视化**：每回合奖励 + 滑动平均 + 训练损失曲线
- **评估**：关闭探索后测试智能体的真实表现
- **进一步优化方向**：Double DQN、Dueling DQN、Prioritized Replay、Rainbow 等

## 本地运行

确保已安装 Python 3.10+，然后安装依赖：

```bash
pip install "gymnasium[classic_control]" torch matplotlib numpy jupyter
```

启动 notebook：

```bash
jupyter notebook rl_tutorial.ipynb
```

## 许可证

本项目基于 MIT License 开源。
