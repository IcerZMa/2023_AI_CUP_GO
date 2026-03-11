# 2023 AI CUP - Go Competition (Top 15 / 580)

本專案參加 **2023 AI CUP 圍棋棋力模仿與棋風辨識競賽**，開發一套整合「棋手實力預測」、「落子預測」與「下棋風格分析」的深度學習分析系統。

## 核心目標 (Core Objectives)
* **實力評估 (Rank Prediction)**：精確預測對局者的級位與段位。
* **落子預測 (Move Prediction)**：模擬棋盤局勢，預測對手最可能的下一手位置。
* **風格辨識 (Playstyle Analysis)**：分析並分類不同棋手的對弈策略與習慣。

## 技術方法 (Methodology)

### 1. 深度殘差網路 (Deep Residual Policy Network)
* **殘差模組 (Residual Blocks)**：利用跳躍連接 (Skip Connections) 克服深層網路在 19x19 棋盤上的梯度消失問題。
* **瓶頸結構 (Bottleneck Layers)**：引入 $1 \times 1$ 卷積進行降維與特徵壓縮，在維持表達能力的同時提升推理效率。

### 2. 多維度狀態編碼 (State Representation)
* **特徵平面 (Feature Planes)**：針對不同任務整合 3 層（黑白分布、最後一手）或 17 層（含前 8 步歷史軌跡與持方資訊）的特徵平面。
* **時序 Padding 演算法**：針對開局階段開發自動補足機制，確保模型能獲得穩定的歷史上下文資訊。

### 3. 機率建模 (Label Encoding)
* **One-hot 標籤編碼**：將落子目標轉化為 361 維（19*19）向量，將預測落點建模為空間機率分布問題。

## 專案結構 (Project Structure)
```text
notebooks/
├── dan_model.ipynb           # 段位實力預測模型
├── kyu_model.ipynb           # 級位實力預測模型
├── style_analysis.ipynb      # 風格分類辨識模型
└── submission_pipeline.ipynb  # 整合推論與繳交流程

final_rank.png
```
##  Result

Final Ranking: Top 15 / 580 teams


![image](https://github.com/IcerZMa/2023_AI_CUP_GO/blob/main/final_rank.png?raw=true)







