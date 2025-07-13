# 数维杯2024数学建模说明

## 目录结构

```
├── main.ipynb                  # 主建模与综合分析代码（多指标对比、雷达图等）
├── PCA.ipynb                   # 主成分分析（PCA）相关代码
├── data process.ipynb          # 数据预处理与特征工程代码
├── data/                       # 数据文件夹，存放原始数据Excel
│   ├── Appendix 1.xlsx         # 附件1，原始数据表
│   └── Appendix 2.xlsx         # 附件2，原始数据表
├── Competition_problem/        # 赛题文件夹，存放官方赛题PDF
│   └── 2024_“ShuWei Cup”D_Problem.pdf # 赛题PDF原文
├── README.md                   # 项目说明文件

```

## 文件说明

- `main.ipynb`：主建模分析脚本，包含数据读取、标准化、各类指标对比、可视化（如柱状图、雷达图）等，适合复现主要建模与分析流程。
- `PCA.ipynb`：主成分分析（PCA）相关代码，包含数据降维、相关性分析、贡献率分析等。
- `data process.ipynb`：数据清洗、特征工程、缺失值处理、独热编码、基础可视化等辅助脚本。
- `data/`：数据文件夹，包含官方提供的原始数据表（Excel）。
  - `Appendix 1.xlsx`、`Appendix 2.xlsx`：原始数据。
- `Competition_problem/`：赛题文件夹，包含官方赛题PDF。
  - `2024_“ShuWei Cup”D_Problem.pdf`：本次比赛的赛题原文。

## 依赖环境

建议使用 Python 3.8 及以上，主要依赖如下：
- numpy
- pandas
- matplotlib
- seaborn
- openpyxl
- scikit-learn
- statsmodels
- tqdm

可通过如下命令安装：
```
pip install numpy pandas matplotlib seaborn openpyxl scikit-learn statsmodels tqdm
```

## 运行与复现

1. 准备好所有数据文件（data/、Competition_problem/）与代码文件，建议在 Jupyter Notebook 环境下逐步运行。
2. 推荐先运行 `data process.ipynb` 进行数据清洗和特征工程。
3. 如需降维分析，可运行 `PCA.ipynb`。
4. 主要建模与可视化分析请运行 `main.ipynb`，可复现多指标对比、雷达图等核心结果。

如有问题请结合代码注释与单元格说明理解各部分功能。

---

本项目为 2024 数维杯数学建模竞赛 D 题赛题分析代码，仅供学习与交流使用。
