# YOLO Platform V2.0 - 一体化人工智能视觉平台

## 文档信息

| 项目 | 内容 |
|------|------|
| 文档名称 | YOLO Platform V2.0 项目说明 |
| 版本号 | v2.0.0 |
| 编写日期 | 2026-04-22 |
| 编写人 | FongSeungyen |
| 项目主页 | [https://github.com/FongSeungyen/YOLO_Platform](https://github.com/FongSeungyen/YOLO_Platform) |

---

## 系统简介

YOLO Platform V2.0 是一款面向工业级应用的全功能计算机视觉开发平台，基于 YOLO（You Only Look Once）系列算法构建。平台全面支持五种核心视觉任务：**图像分类（Classify）、目标检测（Detect）、实例分割（Segment）、姿态估计（Pose）、定向边界框检测（OBB）**，提供从数据采集、智能标注、模型训练、性能评估到模型部署的一站式解决方案。

### 核心特性

| 特性 | 说明 |
|------|------|
| 降低技术门槛 | 提供直观的图形化操作界面，使非专业用户也能快速上手 |
| 提升开发效率 | 集成AI辅助标注、自动化训练流程和一键式模型优化 |
| 支持全栈部署 | 覆盖云端服务器、边缘计算设备、移动端应用等多场景部署 |
| 保障模型性能 | 提供完整的模型评估体系和多维度优化工具 |
| 确保数据安全 | 支持本地私有化部署，数据无需上传云端 |

---

## 版本更新

| 版本 | 发布日期 | 主要更新内容 |
|------|----------|--------------|
| **v2.0.0** | 2026-04-22 | 重大版本更新：新增分类、分割、姿态估计、OBB四种任务支持；AI辅助标注全任务覆盖；系统诊断工具；现代化UI升级；完整的7篇技术文档 |
| v1.0.0 | 2026-03-31 | 初始版本发布：支持目标检测任务；数据集管理；模型训练评估部署 |

---

## 功能特性

### 1. 五大核心任务支持

| 任务类型 | 英文名称 | 核心功能 | 适用场景 |
|----------|----------|----------|----------|
| **图像分类** | Classify | • 图像级分类<br>• 多标签分类<br>• 置信度评分 | 内容识别、图像分类 |
| **目标检测** | Detect | • 边界框检测<br>• 多目标跟踪<br>• 实时检测 | 物体定位、计数 |
| **实例分割** | Segment | • 像素级分割<br>• 实例级掩码<br>• 轮廓提取 | 精确轮廓、像素分析 |
| **姿态估计** | Pose | • 关键点检测<br>• 骨架连接<br>• 姿态分析 | 人体/动物姿态分析 |
| **定向边界框** | OBB | • 旋转矩形检测<br>• 方向感知检测<br>• 任意角度目标 | 遥感、文本检测 |

### 2. 数据集管理与预处理

| 功能 | 说明 |
|------|------|
| 多格式支持 | COCO、Pascal VOC、YOLO、LabelMe、VIA、CVAT、LabelImg、Roboflow、CreateML、TFRecord等10种主流格式的导入与导出 |
| 数据增强 | Mosaic、MixUp、随机翻转、旋转、缩放、颜色抖动、高斯噪声等20+种增强策略 |
| 数据验证 | 自动检测损坏图像、标注越界、类别不平衡等问题 |
| 版本控制 | 支持数据集快照、历史回溯和增量更新 |

### 3. 交互式数据标注

| 功能 | 说明 |
|------|------|
| 多种标注方式 | 支持矩形框、多边形、关键点、旋转框等多种标注方式 |
| AI辅助标注 | 集成AI预标注功能，全五种任务类型支持，大幅提升标注效率 |
| 标注审核 | 支持对AI标注进行快速审核和精细调整 |

### 4. 模型训练

| 功能 | 说明 |
|------|------|
| 模型架构 | YOLOv8、YOLO11、YOLO26 全系列支持（n/s/m/l/x） |
| 可视化配置 | 可视化超参数配置界面，实时训练监控 |
| 高级特性 | 混合精度训练、梯度累积、学习率预热、早停机制、断点续训 |
| 多GPU支持 | 支持多GPU数据并行（DDP）训练 |

### 5. 模型评估

| 功能 | 说明 |
|------|------|
| 基础指标 | mAP@0.5、mAP@0.5:0.95、Precision、Recall、F1-Score |
| 高级分析 | 混淆矩阵、PR曲线、ROC曲线、错误样本分析 |
| 性能测试 | 推理速度（FPS）、模型大小、计算量（FLOPs） |
| 模型对比 | 支持不同模型版本的性能对比分析 |

### 6. 模型导出与部署

| 功能 | 说明 |
|------|------|
| 多格式导出 | 支持ONNX、TensorRT、CoreML、TFLite、OpenVINO、Paddle等主流部署格式 |
| 模型优化 | 提供INT8/FP16量化、模型剪枝、层融合等优化选项 |
| 本地推理 | 支持图像、视频、摄像头实时推理 |
| API服务 | 提供RESTful API接口，FastAPI构建 |
| 边缘部署 | 支持TensorRT、CoreML、OpenVINO等多平台边缘加速 |

### 7. 现代化GUI设计

| 功能 | 说明 |
|------|------|
| 界面设计 | 符合Material Design规范的现代化界面设计 |
| 响应式布局 | 适配不同分辨率的响应式布局 |
| 主题系统 | 支持6种预设主题（深色、浅色、海洋蓝、自然绿、活力橙、优雅紫） |
| 无边框窗口 | MacBook风格的无边框窗口设计 |

### 8. 系统工具

| 功能 | 说明 |
|------|------|
| 系统诊断 | 环境检查、硬件检测、性能测试、配置验证 |
| 缓存清理 | 清理Python缓存、临时文件、日志文件、图像缩略图缓存 |
| 日志查看器 | 日志级别筛选、关键词搜索、时间范围过滤、日志导出 |

---

## 系统要求

### 硬件要求

| 配置等级 | CPU | 内存 | 显卡 | 存储 | 适用场景 |
|----------|------|------|------|------|----------|
| **最低配置** | 4核 (i5/R5) | 8GB DDR4 | GTX 1060 6GB | 50GB SSD | 学习试用、小数据集 |
| **推荐配置** | 8核 (i7/R7) | 16GB DDR4 | RTX 3060 12GB | 100GB NVMe SSD | 常规开发、中等数据集 |
| **高性能配置** | 16核+ (i9/R9) | 32GB+ DDR4 | RTX 4090 / A100 24GB+ | 500GB+ NVMe SSD | 生产环境、大数据集 |

### 软件要求

| 软件 | 版本要求 | 说明 |
|------|----------|------|
| **操作系统** | Windows 10/11 (64位), Ubuntu 20.04/22.04, macOS 12+ | 64位系统 |
| **Python** | 3.10 - 3.12 (推荐 3.10) | 需64位版本 |
| **PyTorch** | 2.0+ | 深度学习框架 |
| **CUDA** | 11.8 / 12.1 / 12.4 | GPU训练必需 |
| **cuDNN** | 8.6+ | 深度学习加速库 |

---

## 安装

### 方式一：源码安装（推荐）

#### 1. 克隆仓库

```bash
git clone https://github.com/FongSeungyen/YOLO_Platform.git
cd YOLO_Platform
```

#### 2. 创建虚拟环境（推荐Python 3.10）

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Linux/macOS
python3.10 -m venv venv
source venv/bin/activate
```

#### 3. 安装依赖

**CPU版本：**
```bash
pip install -r requirements.txt
```

**GPU版本（CUDA 12.4）：**
```bash
pip install -r requirements-gpu.txt
```

**最小化版本（仅基础功能）：**
```bash
pip install -r requirements-minimal.txt
```

#### 4. 运行应用程序

```bash
python main.py
```

### 方式二：Conda环境安装

```bash
# 创建环境
conda create -n yolo-platform python=3.10
conda activate yolo-platform

# 安装PyTorch（GPU版本）
conda install pytorch torchvision torchaudio pytorch-cuda=12.4 -c pytorch -c nvidia

# 安装其他依赖
pip install -r requirements.txt

# 启动应用
python main.py
```

---

## PyTorch与CUDA版本对应关系

### 推荐配置（PyTorch 2.6+）

| PyTorch版本 | CUDA版本 | 安装命令 |
|-------------|----------|----------|
| 2.6.0 | 12.4 | `pip install torch==2.6.0 torchvision==0.21.0 torchaudio==2.6.0 --index-url https://download.pytorch.org/whl/cu124` |
| 2.6.0 | 11.8 | `pip install torch==2.6.0 torchvision==0.21.0 torchaudio==2.6.0 --index-url https://download.pytorch.org/whl/cu118` |
| 2.6.0 | CPU | `pip install torch==2.6.0 torchvision==0.21.0 torchaudio==2.6.0 --index-url https://download.pytorch.org/whl/cpu` |

更多版本请参考 [PyTorch官方安装页面](https://pytorch.org/get-started/previous-versions/)

---

## 快速开始

### 1. 启动应用程序

```bash
python main.py
```

### 2. 创建数据集

1. 点击侧边栏"📁 数据集"
2. 选择任务类型（Classify/Detect/Segment/Pose/OBB）
3. 点击"新建数据集"
4. 填写数据集信息和类别配置
5. 添加图像文件

### 3. AI辅助标注

1. 打开数据集，选择图像
2. 点击"🤖 AI标注"按钮
3. 选择预训练模型
4. 配置推理参数，开始AI标注
5. 审核并修正AI生成的标注

### 4. 模型训练

1. 点击侧边栏"🚀 训练"
2. 选择数据集和模型配置
3. 配置训练参数（epochs、batch size、learning rate等）
4. 点击"开始训练"，实时监控训练过程

### 5. 模型导出与部署

1. 点击侧边栏"🌐 部署"
2. 选择训练好的模型
3. 选择导出格式（ONNX/TensorRT/TFLite等）
4. 或启动API服务进行在线推理

---

## 项目结构

```
yolo-platform/
├── main.py                      # 主程序入口
├── requirements.txt             # CPU依赖
├── requirements-gpu.txt         # GPU依赖
├── requirements-minimal.txt     # 最小依赖
├── LICENSE.txt                  # 许可证文件
├── README.md                    # 项目说明文档
├── Logo.PNG                     # 应用程序Logo
├── Logo.ico                     # 应用程序图标
│
├── core/                        # 核心模块
│   ├── config.py               # 配置管理
│   ├── logger.py               # 日志系统
│   ├── theme_manager.py        # 主题管理
│   ├── version.py              # 版本管理
│   └── ...
│
├── auth/                        # 认证模块
│   ├── manager.py              # 认证管理器
│   ├── models.py               # 用户数据模型
│   └── ...
│
├── data/                        # 数据管理模块
│   ├── dataset_manager.py      # 数据集管理
│   ├── formats.py              # 格式转换器
│   └── ...
│
├── gui/                         # GUI界面模块
│   ├── main_window_modern.py   # 现代化主窗口
│   ├── widgets/                # 工作流组件
│   │   ├── dataset_classify_workflow_widget.py
│   │   ├── dataset_detect_workflow_widget.py
│   │   ├── dataset_segment_workflow_widget.py
│   │   ├── dataset_pose_workflow_widget.py
│   │   ├── dataset_obb_workflow_widget.py
│   │   ├── training_widget.py
│   │   ├── evaluation_widget.py
│   │   ├── inference_widget.py
│   │   └── ...
│   └── dialogs/                # 对话框
│       ├── login_dialog.py
│       ├── settings_dialog.py
│       ├── diagnostic_dialog.py
│       ├── cache_cleanup_dialog.py
│       └── log_viewer_dialog.py
│
├── tests/                       # 测试模块
├── logs/                        # 日志目录
├── config/                      # 配置目录
├── workspace/                   # 工作空间（自动创建）
│   ├── datasets/               # 数据集
│   ├── models/                 # 模型文件
│   ├── outputs/                # 输出结果
│   └── cache/                  # 缓存文件
├── docs/                        # 文档目录
│   └── zh/                     # 中文文档
│       ├── 01-系统概述.md
│       ├── 02-功能模块详细说明.md
│       ├── 03-技术架构设计.md
│       ├── 04-安装部署流程.md
│       ├── 05-用户操作指南.md
│       ├── 06-常见问题解答.md
│       └── 07-故障排除方法.md
└── Theme/                       # 主题资源
```

---

## 快捷键

| 快捷键 | 功能 |
|--------|------|
| `Ctrl+N` | 新建数据集 |
| `Ctrl+O` | 打开数据集 |
| `Ctrl+S` | 保存 |
| `Ctrl+Z` | 撤销 |
| `Ctrl+Y` | 重做 |
| `Ctrl+Q` | 退出应用 |
| `Tab` | 下一张图像（标注界面） |
| `R` | 矩形工具（检测标注） |
| `P` | 多边形工具（分割标注） |
| `K` | 关键点工具（姿态标注） |
| `O` | 旋转框工具（OBB标注） |

---

## 开发计划

- [x] 基础架构搭建
- [x] 配置管理系统
- [x] 数据集管理模块
- [x] 数据标注工具（5种任务类型）
- [x] AI辅助标注系统
- [x] 模型训练模块
- [x] 模型评估系统
- [x] 模型导出功能（多格式）
- [x] 推理部署模块（本地/API/边缘）
- [x] 现代化GUI界面（6种主题）
- [x] 系统诊断工具
- [x] 缓存清理工具
- [x] 日志查看器
- [x] 完整技术文档（7篇）
- [ ] 多人协作标注
- [ ] 高级数据增强算法
- [ ] 单元测试和集成测试

---

## 文档中心

| 文档 | 说明 | 路径 |
|------|------|------|
| 系统概述 | 系统整体介绍和功能概览 | [docs/zh/01-系统概述.md](./docs/zh/01-系统概述.md) |
| 功能模块详细说明 | 各功能模块的详细设计说明 | [docs/zh/02-功能模块详细说明.md](./docs/zh/02-功能模块详细说明.md) |
| 技术架构设计 | 系统技术架构和设计规范 | [docs/zh/03-技术架构设计.md](./docs/zh/03-技术架构设计.md) |
| 安装部署流程 | 详细的安装和部署指南 | [docs/zh/04-安装部署流程.md](./docs/zh/04-安装部署流程.md) |
| 用户操作指南 | 详细的使用操作说明 | [docs/zh/05-用户操作指南.md](./docs/zh/05-用户操作指南.md) |
| 常见问题解答 | 常见问题及解决方案 | [docs/zh/06-常见问题解答.md](./docs/zh/06-常见问题解答.md) |
| 故障排除方法 | 系统故障排查和解决方法 | [docs/zh/07-故障排除方法.md](./docs/zh/07-故障排除方法.md) |

---

## 常见问题

### Q1: Python版本不兼容

**问题：** 使用Python 3.14等开发版导致安装失败

**解决：** 请确保使用 Python 3.10 - 3.12 版本，推荐 Python 3.10

```bash
python3.10 -m venv venv
```

### Q2: PyTorch安装失败

访问 [PyTorch官网](https://pytorch.org/get-started/locally/) 获取适合您系统的安装命令。

### Q3: 安装速度慢

使用国内镜像源：
```bash
pip install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple
```

更多问题请参考 [06-常见问题解答.md](./docs/zh/06-常见问题解答.md) 和 [07-故障排除方法.md](./docs/zh/07-故障排除方法.md)

---

## 贡献指南

欢迎提交Issue和Pull Request！

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开 Pull Request

---

## 许可证

本项目采用 **MIT License** 开源协议，可自由使用、修改和分发。详见 [LICENSE.txt](LICENSE.txt) 文件。

---

## 联系方式

| 方式 | 信息 |
|------|------|
| 项目主页 | [https://github.com/FongSeungyen/YOLO_Platform](https://github.com/FongSeungyen/YOLO_Platform) |
| 问题反馈 | [https://github.com/FongSeungyen/YOLO_Platform/issues](https://github.com/FongSeungyen/YOLO_Platform/issues) |
| 技术支持邮箱 | fongseungyen@gmail.com |

---

## 致谢

- [Ultralytics YOLO](https://github.com/ultralytics/ultralytics)
- [PySide6 (Qt for Python)](https://doc.qt.io/qtforpython/)
- [PyTorch](https://pytorch.org/)
- [FastAPI](https://fastapi.tiangolo.com/)

---

**文档结束**

*本文档由 YOLO Platform 技术开发者FongSeungyen编写，遵循 MIT 开源协议。*

*最后更新：2026-04-22*

---

© 2026 FongSeungyen. All Rights Reserved.
