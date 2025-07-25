# 碳足跡計算機 (Carbon Footprint Calculator)

這是一個互動式網頁應用，旨在幫助研究人員、開發人員和學生估算其 AI 及其他演算任務所產生的碳足跡。本工具的計算模型主要基於 _Green Algorithms_ 論文的框架，並整合了台灣在地的碳排係數，讓數據更具參考價值。
## ✨ 主要功能
- **互動式表單**：使用者可以根據自身的硬體規格（CPU、GPU）、使用時間、電力效率 (PUE) 等參數進行輸入。
- **即時碳強度 (CI) 數據**：
    - **自動偵測**：當地點設定為「台灣」時，會自動透過 API 抓取即時的電力碳強度數據。
    - **手動輸入**：使用者也可以選擇「其他地區」，並手動輸入從 [Electricity Maps](https://app.electricitymaps.com/map "null") 查得的碳強度數值。
- **視覺化圖表**：運算結果中的「排放來源分析」會以動態圓餅圖呈現，清楚展示 CPU、GPU 與記憶體各自的碳排佔比。
- **在地化換算指標**：為了讓碳排放數據更有感，計算結果會自動換算為多種台灣民眾熟悉的日常項目，例如：
    - 🌳 樹月的碳吸收量
    - 🚄 每人搭乘高鐵的公里數
    - 🚌 每人搭乘公車的公里數
    - 🧻 捲筒衛生紙的製造量
    - 💧 瓶裝水的製造量
    - 🍺 罐裝台灣啤酒的製造量
## 🛠️ 技術來源與參考資料
本專案的開發與數據引用基於以下來源：
- **網頁生成方式**:
    - Gemini 2.5 pro canvas
- **核心計算模型來源**:
    - **論文**: Lannelongue, L., Grealey, J., & Inouye, M. (2021). Green Algorithms: Quantifying the Carbon Footprint of Computation. _Advanced Science, 8_(12). [https://doi.org/10.1002/advs.202100707](https://doi.org/10.1002/advs.202100707 "null")
    - **論文網站**: [https://www.green-algorithms.org/](https://www.green-algorithms.org/ "null")
- **單位換算數據來源**:
    - **環境部碳足跡排放係數**: [https://data.moenv.gov.tw/dataset/detail/CFP_P_02](https://data.moenv.gov.tw/dataset/detail/CFP_P_02 "null")
    - **台灣高速鐵路股份有限公司**: [https://www.thsrc.com.tw/ArticleContent/5a1f4c72-b564-4706-bcdd-efbda93c3d93](https://www.thsrc.com.tw/ArticleContent/5a1f4c72-b564-4706-bcdd-efbda93c3d93 "null")