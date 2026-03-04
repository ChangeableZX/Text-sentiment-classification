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
- **开发环境**: Jupyter Notebook

## 工作流程
1. **环境初始化与数据准备**：利用 GPU 硬件加速训练；读取本地 TSV 训练集与测试集，并精准分离特征与标签。
2. **数据清洗与文本分词**：使用 `Jieba` 进行中文分词，并引入外部停用词典 (`hit_stopwords.txt`) 过滤噪声。
3. **特征工程与张量转换**：利用 `Gensim` 训练 Word2Vec 获取词向量并转化为句向量；同时使用 `BertTokenizer` 对文本进行编码、截断与填充，生成 BERT 所需的输入张量矩阵。
4. **模型构建与递进式训练**：依次构建并训练了隐层为 50 的基础 **LSTM**、双向拼接隐状态序列的 **Bi-LSTM**，以及引入 `BertForSequenceClassification` 预训练模型执行二分类任务的 **BERT**。

## 模型性能对比
在独立的测试集上，各模型的分类准确率（Accuracy）表现如下：
* **LSTM**: ~90.86%
* **Bi-LSTM**: ~91.02%
* **BERT (Fine-tuned)**: ~97.09%

## 如何使用
1. 克隆仓库：
   ```bash
   git clone https://github.com/ChangeableZX/Text-sentiment-classification.git
2. 安装依赖：
   ```bash
   pip install pandas numpy jieba smart_open gensim torch torchvision torchaudio transformers 
3. 运行 Jupyter Notebook 查看详细步骤。
