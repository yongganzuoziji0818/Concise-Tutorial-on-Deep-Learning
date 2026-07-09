# 数据集与模型权重说明

本仓库不跟踪大型数据集、训练好的模型权重和运行缓存。这样可以保持 GitHub 仓库轻量，避免克隆时下载大量与教程源码无关的二进制文件。

## 本地目录约定

Notebook 中使用的数据和权重建议放在对应章节目录下，例如：

```text
代码/02.PyTorch入门/data/
代码/03.神经网络与全连接模型/data/
代码/04.卷积模型/data/
代码/04.卷积模型/model/
代码/06.生成模型/model/
```

这些目录已经被 `.gitignore` 忽略，不会被提交到 GitHub。

## 常见数据来源

- MNIST：可通过 `torchvision.datasets.MNIST(..., download=True)` 自动下载
- CIFAR-10：可通过 `torchvision.datasets.CIFAR10(..., download=True)` 自动下载
- 图像分类示例数据：请根据 Notebook 中的路径要求放到本地 `data/` 目录
- 预训练模型权重：请根据 Notebook 中的模型名称从官方来源下载，或在本地训练生成

## 提交规则

请不要提交以下文件：

- `data/`
- `*.pt`
- `*.pth`
- `*.ckpt`
- `*.onnx`
- `__pycache__/`
- `.ipynb_checkpoints/`
- `runs/`
- `outputs/`
- `checkpoints/`

如果某个小型示例文件对教程讲解必不可少，可以单独放入 `image/` 或其他明确的轻量资源目录，并在 README 中说明用途。
