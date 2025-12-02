# 电商客户RFM价值分层分析 | E-commerce Customer RFM Segmentation

## 📊 项目简介 | Project Overview

**中文**：基于英国跨境电商平台交易数据（2010-2011），使用RFM模型对5,339名客户进行价值分层，识别高价值客户群体与流失风险客户，为精准营销提供数据支持。

**English**: Performed RFM analysis on 5,339 customers from UK e-commerce platform (2010-2011), segmented customers by value, identified high-value and churn-risk groups for targeted marketing.

## 🎯 核心发现 | Key Insights

- **VIP客户**：962人（18%）贡献 **65%营收** ($5.8M) → 帕累托法则验证
- **流失客户**：1,065人（20%），历史价值$519K，**预期召回价值$52K**（按10%成功率）
- **运营建议**：
  - VIP客户：专属客服 + 新品优先体验
  - At Risk客户：20%定向优惠券召回
  - Lost客户：放弃治疗，节省成本

## 🛠️ 技术栈 | Tech Stack

- **数据处理**：Pandas, NumPy
- **可视化**：Matplotlib, Seaborn
- **文件格式**：Excel (45MB) → CSV (清洗后)

## 📂 数据集 | Dataset

由于原始数据较大（45MB），请从Kaggle自行下载：  
[Online Retail Dataset]([https://www.kaggle.com/datasets/vijayuv/onlineretail])

**文件放置**：下载后重命名为 `Online Retail.xlsx` 放入项目根目录即可运行。

## 🚀 快速开始 | Quick Start

```bash
# 安装依赖
pip install -r requirements.txt

# 运行分析
python rfm_analysis.py
📈 输出结果 | Outputs
rfm_results.csv：每个客户的RFM分数与分层标签
reports/segment_pie.png：客户分层饼图
reports/top100_scatter.png：TOP100客户RFM分布
reports/pareto_chart_fixed.png：帕累托分析图（横轴1-1000）

RFM-Customer-Segmentation/
├── rfm_analysis.py
├── requirements.txt
├── reports/
│   ├── segment_pie.png
│   ├── top100_scatter.png
│   └── pareto_chart_fixed.png
└── README.md
🎓 分析方法 | Methodology
数据清洗：删除缺失值、退货订单，转换日期格式
RFM计算：Recency（最近购买）、Frequency（订单数）、Monetary（总金额）
客户分层：基于RFM总分划分为6个层级（VIP, Loyal, New, Potential, At Risk, Lost）
可视化：饼图、散点图、帕累托图展示分层结果
👔 业务价值 | Business Value
For Interviewers:
Demonstrated end-to-end data analysis capability
Transformed raw transaction data into actionable business insights
Identified $52K recoverable revenue from churned customers
Visualized results for non-technical stakeholders
📬 联系方式 | Contact
Email: z2050039274@outlook.com

