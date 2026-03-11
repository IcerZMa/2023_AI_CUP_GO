# 2023_AI_CUP_GO
參與2023 AI CUP 秋季賽的抉擇確實是一項極具挑戰性的冒險，特別是在我之前未曾嘗試過的領域，例如圍棋。在這樣的情境下，我深刻體會到建立一個有效的資料集並進行模型訓練的重要性。

首先，資料集的建立可謂是整個探索的關鍵一環。在圍棋這個複雜的遊戲中，每一步棋都可能對整場比賽產生巨大的影響，因此必須仔細處理提供的資料，使得模型能夠輕鬆地學習到關鍵特徵。

其次，我需要仔細考慮選擇哪種模型進行訓練。在圍棋領域，深度學習模型如卷積神經網路（CNN）通常是被廣泛應用的選擇。然而，我不僅僅止步於此，還嘗試了多種不同的架構，如Resnet、強化學習（RL）等。儘管並非每個架構都最終被納入最終模型，一些在中途被淘汰的架構可能是因效能、成效或技術問題而被淘汰。

這個過程不僅僅是技術層面上的挑戰，更是一場對創造力和解決問題能力的考驗。透過不斷的實驗和調整，我努力找到最適合解決這個棘手問題的方法，並在比賽中展現出我所積累的技能和洞察力。這次參賽經歷不僅擴展了我的專業知識，也讓我深刻體會到在未知領域中挑戰自我的價值。期待在比賽中展現出色的表現，同時也期許這次經驗能夠成為我未來探索更多新領域的良好基石。
# 2023 AI CUP - Go Competition

本專案參加 2023 AI CUP Go Competition，目標是建立一個 AI 模型來分析棋手的棋局，進而預測棋手的實力、下一步棋動作，並判斷棋手的下棋風格。

## Objective
- 根據棋局手法預測棋手實力

- 預測棋手的下一步棋

- 分析棋手的下棋風格

## Methods
- Convolutional Neural Networks (CNN)
- Reinforcement Learning (RL)
- Rank-based modeling

## Project Structure

notebooks/
    dan_model.ipynb
    kyu_model.ipynb
    style_analysis.ipynb
    submission_pipeline.ipynb

final_rank.png

## Result

Final Ranking: Top 15 / 580 teams


![image](https://github.com/IcerZMa/2023_AI_CUP_GO/blob/main/final_rank.png?raw=true)


