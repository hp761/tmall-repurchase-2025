# -
基于Python的问题解析-期末大作业
# 天猫用户复购预测

> 基于用户行为日志与画像数据，预测用户是否会对特定商家产生复购行为。  
> 本项目实现了完整的机器学习流程：特征工程 → 多模型训练（LR/RF/DNN）→ 交叉验证调参 → 提交生成。

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-1.2%2B-green)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.12%2B-orange)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📌 项目简介

本项目基于阿里天池公开数据集，目标是预测用户在给定时间窗口后是否会**再次购买**某商家的商品（二分类任务）。

核心实现包括：
- ✅ **特征工程**：融合用户画像（年龄、性别）、行为日志（点击、加购、购买）及用户-商家交互统计特征  
- ✅ **多模型训练**：逻辑回归（LR）、随机森林（RF）、深度神经网络（DNN）  
- ✅ **严谨评估**：5 折分层交叉验证 + AUC 作为主评估指标  

当前最佳模型（随机森林）在本地验证集上达到 **AUC ≈ 0.64**，具备基础判别能力，仍有较大优化空间。

---

## 🧪 运行环境与依赖

### 系统要求
- Python ≥ 3.8
- 64 位操作系统（推荐 Linux / macOS）

### 安装依赖

```bash
pip install -r requirements.txt
