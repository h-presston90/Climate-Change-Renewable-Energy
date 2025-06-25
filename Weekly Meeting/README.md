
# 📅 Weekly Meeting and Work Report Rules

不同於一般「先報告後討論」的週會形式，**本計畫的咪聽採行事前繳交制**，你必須在會議前繳交簡報與週誌，並**確保內容完整具體**。我將會**於會前閱讀你的報告與簡報**，並在會議中**直接針對內容進行深入討論與回饋**，不會再重複簡報流程。

> 🔔 簡報與週誌的提前繳交為**強制要求**，不得延後。請確保你在報告中清楚呈現所有資訊，包含：本週進度、資料成果、遇到的困難、以及希望討論的問題等。你的內容越具體，會議中能提供的回饋與幫助就越到位。

為了提升每週咪聽的效率並促進彼此之間的有效溝通，請務必遵守以下規範。

---

📌 **Reminder**：All reports and latest progress must be committed and pushed to GitHub before **23:59** on the day **before** the weekly meeting.

---

### 1. Upload Presentation Slides 

Before each **weekly meeting**, upload your slides to the `weekly_meeting/` folder.


**The presentation should include (if applicable, but not limited to):**  
- Papers or materials you reviewed ｜這週讀了哪些文獻／資料  
- Data collected or processed ｜收集或處理了哪些資料  
- Algorithms or methods studied ｜了解了哪些演算法或技術  
- Current progress or results (Required) ｜目前進度與成果（**強制**）  
- Challenges encountered (Required) ｜遇到的問題或困難（**強制**）  
- Topics you want to discuss (Required) ｜想要討論的內容（**強制**）  
- Planned progress and expected outcomes for next week (Required) ｜下週預計的工作進度與預期成果（**強制**）
---

### 2. Update the Weekly Journal 

- Please update your **weekly journal** (in markdown format) in the same folder each week.  

- Use **bullet points** to clearly organize your content, with **concise section titles** followed by **brief but informative explanations**. For example:

```text
- 📖 Paper Reading：分析了 XX 論文的資料來源與假設，發現作者使用的是平均碳排，可能低估尖峰負載的影響。  
  該研究以整體年度平均代表碳排強度，未考慮邊際機組隨負載變動的實際調度邏輯。我認為若改用邊際碳排因子（MEF）可能更貼近實際情況，將作為後續分析方向。

- 🔍 資料處理：完成某資料集的欄位統一與前處理，轉換成 hourly 格式以利後續比對 ERA5。  
  原始資料來自台電發電機組紀錄與潮流資料，解析度為 10 分鐘，已聚合為每小時平均並標準化能源別欄位。

- 📊 初步成果：使用 rule-based 方法初步分類邊際機組，與預期趨勢相符。  
  透過 ΔLoad 對應 ΔGen 的方式推估邊際反應單元，初步結果顯示燃氣機組於負載上升時具有高 ramp-up 比例，符合實務調度趨勢。

- ❓ 討論事項：想了解 baseline 負載變動與儲能調度是否能區分，可能影響邊際碳排的推論。  
  儲能裝置參與調度時，其放電行為可能被誤判為其他機組反應，而 baseline 排程造成的變化也可能誤導 ΔGen 判讀，需討論是否納入儲能狀態或 baseline 模擬輔助辨識。

- 🗓️ 下週預計的工作進度與預期成果：將實作以 MEF 為基礎的碳排估算流程，並與 AEF 結果進行差異比較。  
  預期完成：建立每小時邊際碳排資料表格、繪製日內變化趨勢圖，以及撰寫初步觀察摘要。
```

#### ✍️ Guidelines for Writing:
1. You may write in either **Mandarin** or **English**, based on your preference.

2. We **strongly encourage the use of LLMs (e.g., ChatGPT)** to assist with journal writing — for tasks such as summarizing papers, refining thoughts, or organizing structure.

3. ⚠️ **Important**: Always **review and revise the generated content** to ensure it accurately reflects your own understanding, interpretation, and thinking. Do not copy blindly.




---

### 3. Add Personal Insights on Literature 

When reviewing papers, go beyond summary. Add:
- Your critique
- Ideas on how the paper connects to your research

✅ Example：  

> “This paper evaluates carbon emissions using **average emission factors**, which assumes all units contribute equally to emission intensity. However, in real power systems, only a subset of dispatchable units responds to marginal changes in load. Therefore, I believe **marginal emission factors (MEFs)** offer a more accurate representation of the system's operational behavior. Applying MEFs instead of average values may significantly alter the results and policy implications, particularly for short-term interventions or demand-side programs. In my research, I plan to re-evaluate the core analysis using MEFs to better capture the emission dynamics associated with incremental load changes.”

---

> 「這篇文獻採用 **平均碳排放因子（Average Emission Factors）** 來評估碳排，但該方法假設所有機組的碳排貢獻是等量平均，這在實際電網運作中並不成立。 實務上，只有少數具調度能力的機組會對負載變動作出邊際反應，因此我認為 **邊際碳排放因子（Marginal Emission Factors, MEFs）** 更能反映真實的系統運作特性。 若將分析方法從平均因子改為邊際因子，結果與其政策涵義可能會產生顯著差異，特別是針對短期的調度或需量反應措施。因此，我打算在後續研究中嘗試改用 MEFs，重新評估其對碳排表現與決策建議的影響。」


---

### 4. Quantify and Visualize Results 

Avoid vague comparisons. Be specific and visual.


❌ 不建議：  
> Model A is better than Model B

✅ 建議寫法：  
> Model A outperformed Model B by **20%** in MAE  
> 並搭配圖表呈現，如折線圖或誤差分布圖等

---

### 5. Clearly State Challenges and Questions 

Don’t be afraid to raise questions. The more you list, the more targeted help you’ll receive.

請務必**列出面臨的挑戰或卡住的問題**，這是每週咪聽中獲得幫助的關鍵。

---



