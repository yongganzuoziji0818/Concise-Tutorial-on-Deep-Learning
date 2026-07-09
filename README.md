# 简明深度学习教程

本仓库整理了一套面向教学和自学的深度学习简明教程，包含课程课件、Jupyter Notebook 示例和少量配套 Python 代码。内容从 PyTorch 基础逐步过渡到卷积模型、序列模型、生成模型和大模型相关方法。

## 仓库内容

- `代码/`：各章节 Notebook、示例代码和必要的轻量图片素材
- `课件/`：各章节 PowerPoint 课件
- `requirements.txt`：完整冻结环境，适合复现实验机器上的环境
- `requirements-minimal.txt`：推荐的最小运行环境，适合新用户快速开始
- `DATASETS.md`：数据集和模型权重的本地准备说明

## 章节目录

| 章节 | 主题 | Notebook |
| --- | --- | --- |
| 01 | 引言 | `代码/01.引言/` |
| 02 | PyTorch 入门 | `代码/02.PyTorch入门/` |
| 03 | 神经网络与全连接模型 | `代码/03.神经网络与全连接模型/` |
| 04 | 卷积模型 | `代码/04.卷积模型/` |
| 05 | 序列模型 | `代码/05.序列模型/` |
| 06 | 生成模型 | `代码/06.生成模型/` |
| 07 | 大模型 | `代码/07.大模型/` |

## 快速开始

建议使用 Python 3.9 或更新版本，并在虚拟环境中安装依赖：

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements-minimal.txt
```

如果需要完全复现实验环境，可以改用：

```bash
pip install -r requirements.txt
```

然后使用 Jupyter Notebook、JupyterLab 或 VS Code 打开 `代码/` 目录下的 Notebook。

## 数据与模型权重

为了让公开仓库保持轻量，以下内容不会提交到 GitHub：

- 数据集目录，例如 `data/`
- 训练好的模型权重，例如 `*.pt`、`*.pth`、`*.onnx`
- Notebook 缓存和 Python 缓存
- 训练输出目录，例如 `runs/`、`outputs/`、`checkpoints/`

部分 Notebook 需要本地数据集或预训练权重才能完整运行。请参考 [DATASETS.md](DATASETS.md) 准备相关文件。

## 适用对象

本教程适合：

- 刚开始学习深度学习和 PyTorch 的学生
- 需要课程演示材料的教师或助教
- 希望通过 Notebook 快速复现实验流程的学习者

## 说明

本仓库以教学清晰度为优先，代码侧重展示模型结构、训练流程和关键概念。若用于正式项目，请根据实际任务补充数据划分、实验记录、模型评估和工程化配置。
