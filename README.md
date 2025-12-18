# 🚗 Automotive Market Segmentation and Consumer Insights (Dangchedi Platform)  
# 🚗 汽车市场细分与消费者洞察（懂车帝平台）

---

## 📌 Project Background | 项目背景
This project analyzes consumer attention and market segmentation in China’s automotive industry using data from the **Dangchedi platform**. By applying clustering and decision tree models, the study aims to break the deadlock of ambiguous segmentation and uncover the drivers behind high-potential vehicle models.  

本项目基于 **懂车帝平台** 数据，研究中国汽车市场的消费者关注度与细分结构。通过聚类分析与决策树模型，解决市场细分模糊的问题，并揭示高潜力车型背后的核心驱动因素。

**Business Goals | 商业目标**  
- Clarify blurred market segment boundaries | 明确模糊的市场细分边界  
- Identify high-potential models and their drivers | 识别高潜力车型及其驱动因素  
- Provide actionable insights for automakers and platforms | 为车企与平台提供可执行的战略洞察  

---

## 🛠 Tech Stack | 技术栈
- **Language**: Python  
- **Libraries**: pandas, numpy, scikit-learn, matplotlib, seaborn, requests  
- **Methods**: Web scraping, Data cleaning, Clustering (K-means + PCA), Decision Tree  

---

## 📊 Data | 数据
- **Source**: Dangchedi web interface `/motor/pc/car/rank_data`  
- **Dataset**: 743 valid vehicle entries (`dongchedi_rank_data.csv`)  
- **Features**: Vehicle series, brand, min/max price, user engagement count, score, rank  
- **Usage**: Cleaning → Clustering → Decision Tree  

---

## 📈 Visualization | 可视化
- Correlation Matrix: Price range vs. popularity  
- Quadrant Analysis: Price distribution, popularity distribution, rank histogram, brand coverage  
- Key Insight: Most popular models are **new energy vehicles**, showing rising consumer interest in EVs  

---

## 🔍 Cluster Analysis | 聚类分析
- Optimal K = 3 (tested with silhouette coefficient)  
- **Group 1 (56%)**: Low price, low attention (Honda, Wuling)  
- **Group 2 (23%)**: Low price, high attention (BYD, Toyota)  
- **Group 3 (20%)**: Mid-to-high price, high attention (Audi, Denza)  

**Business Suggestion | 商业建议**  
- Platforms: Stratified user operations, targeted promotion  
- Automakers: Focus resources on high-potential segments  
- Brands: Clarify positioning and optimize competitive strategies  

---

## 🌳 Decision Tree | 决策树
- **Core Features**: Brand type (mainstream vs. others), Minimum price  
- **Key Rules**:  
  1. Min price ≤ 139k + mainstream brand → High Attention (Coverage 68.9%)  
  2. Min price ≤ 139k + other brand → Low Attention (Coverage 53.5%)  
  3. Min price > 452k → Low Attention (Coverage 100%)  

**Business Value | 商业价值**  
- Quickly screen promotional models  
- Eliminate low-potential high-priced models  
- Balance brand and price dimensions for strategic layout  

---

## ✅ Conclusion | 结论
- Market can be divided into **three clear segments**: affordable daily-use vehicles, mid-to-high-end new energy vehicles, and premium models.  
- Price ≤ 250,000 yuan is the **core threshold** for distinguishing user attention.  
- Leading brands succeed with **multi-model coverage + targeted pricing** strategies.  
- Data-driven segmentation enables automakers to **reduce marketing costs and optimize positioning**.  

---

## 📘 Notebook Link | Notebook 链接
📘 Notebook: [Dangchedi Platform.ipynb]([https://github.com/你的用户名/你的仓库名/blob/main/Seoul_Bike_Prediction.ipynb](https://github.com/25422138/Automotive-Market-Segmentation-and-Consumer-Insights-Dangchedi-Platform-/blob/main/Automotive%20Market%20Segmentation%20and%20Consumer%20Insights%20(Dangchedi%20Platform)/Dangchedi%20Platform.ipynb))
