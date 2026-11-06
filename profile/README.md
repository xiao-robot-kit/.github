<!-- SPDX-License-Identifier: MIT -->
# XIAO Robot Kit 🤖

> 一块 XIAO ESP32-S3、一套 IMU/电机硬件板、六个公开仓——从手写 C 到 AI 代写
> 到无实物仿真到可视化调试，一条链全给你。

## 六仓地图

| 仓库 | 是什么 | 什么时候用 |
| --- | --- | --- |
| [xiao_robot_kit_idf](https://github.com/xiao-robot-kit/xiao_robot_kit_idf) | 手工档 **ESP-IDF 库**：LSM6DS3 IMU 驱动 + 姿态 + 电机 + 参数持久化（纯 C 核心，已验证示例） | 手写 IDF 工程 |
| [xiao_robot_kit_arduino](https://github.com/xiao-robot-kit/xiao_robot_kit_arduino) | 手工档 **Arduino 库**：同一颗 C 核心 + `library.properties` + 三 sketch | Arduino IDE 用户 |
| [xiao_robot_kit_vibe](https://github.com/xiao-robot-kit/xiao_robot_kit_vibe) | **vibecoding 工作区**：五份 AI 多代理工作流配方，大小库自由切换 | 让 AI 替你写代码 |
| [xiao_robot_kit_docs](https://github.com/xiao-robot-kit/xiao_robot_kit_docs) | **文档**：硬件介绍 + 三库教学 + 示例用法（教怎么用，不是罗列） | 拿到套件先看这里 |
| [xiao_robot_kit_qemu](https://github.com/xiao-robot-kit/xiao_robot_kit_qemu) | **调试**：ESP32-S3 QEMU 虚拟板，无实物烧录仿真 | 没有真板照样调 |
| [xiao_robot_kit_host](https://github.com/xiao-robot-kit/xiao_robot_kit_host) | **上位机**：可视化交互调试（波形/姿态/电机/存储），sim/real 双档 | 想先看到数据在动 |

## 30 秒选路

```
拿到套件 → xiao_robot_kit_docs（硬件认识 + 第一个示例）
写代码   → IDF 用 idf 仓 / Arduino 用 arduino 仓（同一 C 核心，API 一致）
不想写   → vibe 仓派 AI
没真板   → qemu 仓 QEMU 仿真
想看着跑 → host 仓上位机（无设备也有 sim 档）
```

## 设计哲学（一句话）

**零硬编码参数**：每个可调项来自命名预设表；**同一颗 C 核心**：
IDF/Arduino 两形态 API 一致、自由切换；**禁隐式回落**：模式显式，不自动仿真。

## 仓库惯例

- 全部 MIT，SPDX 头标注
- 每库自带可复跑测试（idf 1311 断言 / arduino 语法检查 / host 27 组 / qemu FAQ）
- 提交即证据：可复现命令 + 实际输出

## 收藏 = 免广告

机器人套件 + AI 工作流 + 开源库，三合一。⭐️ 记得 Star。