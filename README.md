# 文本情感分类项目 (Text Sentiment Classification)

本项目是一个基于 Python 和自然语言处理（NLP）技术的情感分析实践。通过对文本数据进行清洗、分词、特征提取，并利用机器学习模型实现对文本情感（如积极/消极）的自动分类。

## 项目背景
情感分析是自然语言处理领域的核心任务之一。本项目旨在探索如何利用传统的机器学习算法或深度学习模型来理解人类语言中的情绪倾向，可应用于舆情监测、产品评价分析等实际场景。

## 核心文件说明
- **NLP.ipynb**: 
  - 包含完整的代码实现：数据预处理、探索性数据分析 (EDA)、模型训练及评估。
  - 使用了常见的 NLP 工具库进行文本向量化处理。
  - 展示了模型在测试集上的准确率、召回率等核心指标。

## 技术栈
- **编程语言**: Python
- **核心库**:
  - `Pandas` / `Numpy`: 数据清洗与矩阵运算
  - `Scikit-learn`: 机器学习模型构建与评估
  - `NLTK` / `Jieba`: 文本分词与停用词处理
  - `Matplotlib` / `Seaborn`: 训练结果可视化
- **开发环境**: Jupyter Notebook

## 工作流程
1. **数据预处理**: 去除噪声符号、分词、去除停用词。
2. **特征工程**: 采用 TF-IDF 或 Word2Vec 将文本转换为数值向量。
3. **模型训练**: 尝试了多种分类器（如朴素贝叶斯、SVM 或随机森林）并进行调参。
4. **结果评估**: 通过混淆矩阵和分类报告分析模型性能。

## 运行结果
在 Notebook 结尾处，你可以查看到模型对样本数据的预测结果以及最终的准确率表现。

## 如何使用
1. 克隆仓库：
   ```bash
   git clone [https://github.com/ChangeableZX/Text-sentiment-classification.git](https://github.com/ChangeableZX/Text-sentiment-classification.git)
2. 安装依赖：
   ```bash
   pip install pandas numpy scikit-learn nltk
3. 运行 Jupyter Notebook 查看详细步骤。
