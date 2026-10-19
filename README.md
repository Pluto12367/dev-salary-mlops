# dev-salary-mlops — 开发者薪资预测 MLOps 项目

基于机器学习的开发者薪资预测项目，采用工业界规范的目录结构，覆盖数据处理、模型训练与调优、实验追踪、模型解释与 Web 应用的完整 MLOps 流程。

## 代码仓库

- GitHub：https://github.com/Pluto12367/dev-salary-mlops
- Gitee：https://gitee.com/Pluto12367/dev-salary-mlops

## 目录结构

```
dev-salary-mlops/
├── data/
│   ├── raw/            # 原始数据
│   └── processed/      # 处理后的数据
├── src/                # 源代码（数据处理、特征工程、模型训练等）
├── models/             # 训练保存的模型文件
├── reports/
│   └── figures/        # 图表与分析报告
├── notebooks/          # Jupyter 探索性分析笔记本
├── requirements.txt    # Python 依赖
└── .gitignore
```

## 技术栈

| 类别 | 依赖 |
|---|---|
| 数据处理 | numpy、pandas |
| 可视化 | matplotlib、seaborn |
| 建模 | scikit-learn、lightgbm |
| 超参调优 | optuna |
| 实验追踪 | mlflow |
| 模型解释 | shap |
| Web 应用 | streamlit |
| 工具 | joblib |

## 环境安装

要求 Python 3.12+。

```bash
# 1. 创建并激活虚拟环境
python -m venv .venv
# Windows:
.venv\Scripts\activate
# Mac/Linux:
source .venv/bin/activate

# 2. 安装依赖
pip install -r requirements.txt
```

使用 [uv](https://github.com/astral-sh/uv) 安装（更快）：

```bash
uv pip install -r requirements.txt --python .venv
```

## Git 提交规范

采用 Conventional Commits 风格：

- `chore:` 杂务（环境、配置）
- `feat:` 新功能
- `fix:` 修复
- `docs:` 文档
- `refactor:` 重构

推送到双远程保持同步：

```bash
git push origin main
git push gitee main
```
