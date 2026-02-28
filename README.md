# 文本情感分类项目 (Text Sentiment Classification)

本项目是一个基于 Python 和自然语言处理（NLP）技术的情感分析实践。通过对文本数据进行清洗、分词、特征提取，并利用机器学习模型实现对文本情感（如积极/消极）的自动分类。

## 项目背景
情感分析是自然语言处理领域的核心任务之一。本项目旨在探索如何利用传统的机器学习算法或深度学习模型来理解人类语言中的情绪倾向，可应用于舆情监测、产品评价分析等实际场景。

## 核心文件说明
- **NLP.ipynb**: 
  - 包含完整的代码实现：数据预处理、探索性数据分析 (EDA)、模型训练及评估。
  - 使用了常见的 NLP 工具库进行文本向量化处理。
  - 展示了模型在测试集上的准确率、召回率等核心指标。

Gemini 说
根据你代码中实际用到的库（特别是你已经从传统的 Scikit-learn 进化到了 BERT 和 PyTorch 深度学习框架），我为你重写了更精准、更具技术含量的“技术栈”部分。

作为一名计算机相关专业的硕士生，在技术栈中区分“深度学习”和“自然语言处理”会显得你的专业背景更加扎实。

## 技术栈
- **编程语言**: Python (3.8+)
- **深度学习框架**:
  - PyTorch: 核心计算引擎，用于构建和训练神经网络模型。
  - Transformers (Hugging Face): 调用预训练的 BERT (BertForSequenceClassification) 模型进行迁移学习。
- **自然语言处理 (NLP)**:
  - Gensim (Word2Vec): 词向量训练与文本语义表示。
  - Jieba: 中文分词与预处理。
  - Smart_open: 高效处理大规模文本流数据。
- **数据科学与工程**:
  - Pandas / Numpy: 结构化数据清洗、矩阵运算及 Tensor 转换。
-**开发环境**: Jupyter Notebook

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
   pip install pandas numpy jieba smart_open gensim torch torchvision torchaudio transformers 
3. 运行 Jupyter Notebook 查看详细步骤。
