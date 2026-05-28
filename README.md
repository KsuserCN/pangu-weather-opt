<!--
Copyright (c) 2026 Qintsg, KsuserKQY, and Raying-9
SPDX-License-Identifier: AFL-3.0

第三方使用声明摘要：
  依赖库：onescience(0.3.0), torch(2.5.1), onnx(1.21.0), onnxsim(0.6.3),
          onnxconverter-common(1.16.0), tensorly(0.9.0), torch-pruning(1.6.1)
  模型/算法：Pangu-Weather (BY-NC-SA 4.0)
  数据来源：ERA5 (Copernicus License)
-->
# Pangu-Weather 推理部署优化

先导杯 2026 参赛项目 — 基于国产科学智算生态（OneScience）的 Pangu-Weather 气象大模型轻量化与推理性能优化。

## 第三方使用声明

### 第三方 Python 包

| 包名 | 版本 | 许可证 | 用途 |
|---|---|---|---|
| onescience | 0.3.0 | Apache-2.0 | 科学计算工具包 |
| torch | 2.5.1 | BSD-3 | 深度学习框架 |
| onnx | 1.21.0 | Apache-2.0 | 模型格式 |
| onnxsim | 0.6.3 | MIT | ONNX 模型简化 |
| onnxconverter-common | 1.16.0 | MIT | ONNX 转换通用工具 |
| tensorly | 0.9.0 | BSD-3 | 张量分解 |
| torch-pruning | 1.6.1 | MIT | PyTorch 模型剪枝 |

### 开源代码/算法引用

| 名称 | 来源 | 许可证 | 说明 |
|---|---|---|---|
| Pangu-Weather | <https://github.com/198808xc/Pangu-Weather> | BY-NC-SA 4.0 | 模型架构与预训练权重 |

### 数据来源

| 数据 | 来源 | 许可 |
|---|---|---|
| ERA5 | ECMWF | Copernicus License |

## 环境准备

1. 安装 Python 3.11 及 [uv](https://docs.astral.sh/uv/)
2. 创建虚拟环境并安装依赖：

```bash
uv sync
```

## 项目结构

```
pangu-weather-opt/
├── src/pangu_weather_opt/   # 训练、推理优化源码
├── docs/report.md           # 优化说明文档
├── pyproject.toml           # 项目依赖与配置
├── uv.lock                  # 依赖锁文件
├── LICENSE                  # AFL-3.0
├── NOTICE                   # 双许可证声明
└── README.md
```

## 许可证

- 源代码：AFL-3.0
- 项目文档：CC-BY-SA-4.0

详见 [`NOTICE`](NOTICE)

## 贡献者

- @Qintsg
- @Ksuserkqy
- @Raying-9
