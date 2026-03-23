# 🎭 The Agency：AI 專家團隊，隨時準備改造您的工作流程

> **觸手可及的完整 AI 團隊** — 從前端高手到 Reddit 社群忍者，從趣味注入師到品質把關人。每位 Agent 都是具備獨特個性、流程和可靠交付成果的專業領域專家。

[![GitHub stars](https://img.shields.io/github/stars/msitarzewski/agency-agents?style=social)](https://github.com/msitarzewski/agency-agents)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
[![Sponsor](https://img.shields.io/badge/Sponsor-%E2%9D%A4-pink?logo=github)](https://github.com/sponsors/msitarzewski)

---

## 🚀 這是什麼？

源自一篇 Reddit 討論串，歷經數月反覆迭代，**The Agency** 是一個持續成長的精心打造 AI Agent 人格集合。每個 Agent 都具備：

- **🎯 專業化**：深耕各自領域的專業能力（非通用提示詞模板）
- **🧠 人格驅動**：獨特的表達風格、溝通方式和工作方法
- **📋 交付導向**：產出真正的程式碼、流程和可衡量的成果
- **✅ 生產就緒**：經過實戰驗證的工作流程和成功指標

**可以這樣理解**：組建你的夢幻團隊，只不過團隊成員是永不休息、從不抱怨、使命必達的 AI 專家。

---

## ⚡ 快速開始

### 方式一：搭配 Claude Code 使用（推薦）

```bash
# 將 agents 複製到 Claude Code 目錄
cp -r agency-agents/* ~/.claude/agents/

# 在 Claude Code 對話中啟用任何 agent：
# "Hey Claude, activate Frontend Developer mode and help me build a React component"
```

### 方式二：作為參考資料

每個 agent 檔案包含：
- 身份認同與人格特質
- 核心使命與工作流程
- 技術交付成果（含程式碼範例）
- 成功指標與溝通風格

瀏覽下方的 agents 清單，複製或調整您所需的即可！

### 方式三：搭配其他工具使用（Cursor、Aider、Windsurf、Gemini CLI、OpenCode）

```bash
# 步驟 1 — 為所有支援工具產生整合檔案
./scripts/convert.sh

# 步驟 2 — 互動式安裝（自動偵測已安裝的工具）
./scripts/install.sh

# 或直接指定特定工具
./scripts/install.sh --tool cursor
./scripts/install.sh --tool copilot
./scripts/install.sh --tool aider
./scripts/install.sh --tool windsurf
```

詳見下方 [多工具整合](#-多工具整合) 章節。

---

## 🎨 The Agency 成員名冊

### 💻 工程部門

一次一個 commit，建構未來。

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 🎨 [前端開發者](engineering/engineering-frontend-developer.md) | React/Vue/Angular、UI 實作、效能 | 現代網頁應用、像素完美 UI、Core Web Vitals 優化 |
| 🏗️ [後端架構師](engineering/engineering-backend-architect.md) | API 設計、資料庫架構、可擴展性 | 伺服器端系統、微服務、雲端基礎設施 |
| 📱 [行動應用開發者](engineering/engineering-mobile-app-builder.md) | iOS/Android、React Native、Flutter | 原生與跨平台行動應用程式 |
| 🤖 [AI 工程師](engineering/engineering-ai-engineer.md) | ML 模型、部署、AI 整合 | 機器學習功能、資料管線、AI 驅動應用 |
| 🚀 [DevOps 自動化師](engineering/engineering-devops-automator.md) | CI/CD、基礎設施自動化、雲端維運 | 管線開發、部署自動化、監控 |
| ⚡ [快速原型師](engineering/engineering-rapid-prototyper.md) | 快速 POC 開發、MVP | 快速概念驗證、黑客松專案、快速迭代 |
| 💎 [資深開發者](engineering/engineering-senior-developer.md) | Laravel/Livewire、進階模式 | 複雜實作、架構決策 |
| 🔒 [資安工程師](engineering/engineering-security-engineer.md) | 威脅建模、安全程式碼審查、安全架構 | 應用程式安全、弱點評估、安全 CI/CD |
| ⚡ [自主優化架構師](engineering/engineering-autonomous-optimization-architect.md) | LLM 路由、成本優化、影子測試 | 需要智慧 API 選擇和成本控管的自主系統 |
| 🔩 [嵌入式韌體工程師](engineering/engineering-embedded-firmware-engineer.md) | Bare-metal、RTOS、ESP32/STM32/Nordic 韌體 | 生產級嵌入式系統與 IoT 裝置 |
| 🚨 [事件應變指揮官](engineering/engineering-incident-response-commander.md) | 事件管理、事後回顧、值班 | 管理生產環境事件並建立事件應變準備 |
| ⛓️ [Solidity 智慧合約工程師](engineering/engineering-solidity-smart-contract-engineer.md) | EVM 合約、Gas 優化、DeFi | 安全且 Gas 優化的智慧合約和 DeFi 協議 |
| 📚 [技術寫作者](engineering/engineering-technical-writer.md) | 開發者文件、API 參考、教學 | 清晰準確的技術文件 |
| 🎯 [威脅偵測工程師](engineering/engineering-threat-detection-engineer.md) | SIEM 規則、威脅獵捕、ATT&CK 對應 | 建構偵測層和威脅獵捕 |
| 💬 [微信小程式開發者](engineering/engineering-wechat-mini-program-developer.md) | 微信生態、小程式、支付整合 | 在微信生態系統中建構高效能應用 |
| 👁️ [程式碼審查員](engineering/engineering-code-reviewer.md) | 建設性程式碼審查、安全性、可維護性 | PR 審查、程式碼品質關卡、透過審查指導 |
| 🗄️ [資料庫優化師](engineering/engineering-database-optimizer.md) | Schema 設計、查詢優化、索引策略 | PostgreSQL/MySQL 調校、慢查詢除錯、遷移規劃 |
| 🌿 [Git 工作流程大師](engineering/engineering-git-workflow-master.md) | 分支策略、約定式提交、進階 Git | Git 工作流程設計、歷史清理、CI 友善的分支管理 |
| 🏛️ [軟體架構師](engineering/engineering-software-architect.md) | 系統設計、DDD、架構模式、取捨分析 | 架構決策、領域建模、系統演進策略 |
| 🛡️ [SRE](engineering/engineering-sre.md) | SLO、錯誤預算、可觀測性、混沌工程 | 生產可靠性、減少苦差事、容量規劃 |
| 🧬 [AI 資料修復工程師](engineering/engineering-ai-data-remediation-engineer.md) | 自我修復管線、隔離 SLM、語義聚類 | 大規模修復損壞資料且零資料遺失 |
| 🔧 [資料工程師](engineering/engineering-data-engineer.md) | 資料管線、Lakehouse 架構、ETL/ELT | 建構可靠的資料基礎設施與倉儲 |
| 🔗 [飛書整合開發者](engineering/engineering-feishu-integration-developer.md) | 飛書/Lark 開放平台、機器人、工作流程 | 建構飛書生態系統整合 |
| 🖼️ [Qt UI 工程師](engineering/engineering-qt-ui-engineer.md) | Qt 6、QML/Qt Quick、自訂元件、跨平台桌面 UI | 跨平台桌面與嵌入式 UI 開發、Qt 元件庫 |
| 🧊 [VTK / 3D 渲染工程師](engineering/engineering-vtk-3d-rendering-engineer.md) | VTK 管線、體積渲染、GPU 加速、科學視覺化 | 醫學/科學資料的 3D 視覺化與大規模資料集渲染 |
| ⚡ [CUDA / GPU 運算工程師](engineering/engineering-cuda-gpu-computing-engineer.md) | CUDA 核心優化、平行運算、記憶體層級調校 | GPU 加速應用、高效能運算、醫學影像處理 |
| 🏥 [醫學影像工程師](engineering/engineering-medical-imaging-engineer.md) | DICOM、CT/MRI 處理、分割、ITK 管線 | 醫學影像處理、法規合規醫療軟體開發 |
| 🏛️ [C++ 架構工程師](engineering/engineering-cpp-architecture-engineer.md) | 現代 C++20/23、高效能系統設計、API 設計 | 大規模 C++ 程式碼庫架構、並行、重構 |
| 🔧 [CMake / 建構系統工程師](engineering/engineering-cmake-build-system-engineer.md) | 現代 CMake、跨平台建構、依賴管理 | 建構系統設計、CI/CD 整合、跨平台編譯 |
| 🔗 [Qt ↔ VTK 整合工程師](engineering/engineering-qt-vtk-integration-engineer.md) | QVTKWidget、MPR 佈局、Qt 信號與 VTK 觀察者橋接 | 醫學影像檢視器、Qt+VTK 即時互動應用 |
| 🔄 [WPF ↔ Qt 移植工程師](engineering/engineering-wpf-qt-porting-engineer.md) | XAML→QML、MVVM→Qt 模式、WPF 控件對照、遷移規劃 | WPF 開發者轉 Qt、桌面應用移植、概念對照 |

### 🎨 設計部門

讓產品更美觀、更好用、更令人愉悅。

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 🎯 [UI 設計師](design/design-ui-designer.md) | 視覺設計、元件庫、設計系統 | 介面設計、品牌一致性、元件設計 |
| 🔍 [UX 研究員](design/design-ux-researcher.md) | 使用者測試、行為分析、研究 | 了解使用者、易用性測試、設計洞察 |
| 🏛️ [UX 架構師](design/design-ux-architect.md) | 技術架構、CSS 系統、實作 | 開發者友善的基礎架構、實作指導 |
| 🎭 [品牌守護者](design/design-brand-guardian.md) | 品牌識別、一致性、定位 | 品牌策略、識別開發、規範指南 |
| 📖 [視覺說書人](design/design-visual-storyteller.md) | 視覺敘事、多媒體內容 | 引人入勝的視覺故事、品牌敘事 |
| ✨ [趣味注入師](design/design-whimsy-injector.md) | 個性、愉悅感、趣味互動 | 增添樂趣、微互動、彩蛋、品牌個性 |
| 📷 [圖像提示工程師](design/design-image-prompt-engineer.md) | AI 圖像生成提示詞、攝影 | Midjourney、DALL-E、Stable Diffusion 攝影提示 |
| 🌈 [包容性視覺專家](design/design-inclusive-visuals-specialist.md) | 代表性、偏見消除、真實影像 | 生成文化準確的 AI 圖像與影片 |

### 💰 付費媒體部門

將廣告支出轉化為可衡量的商業成果。

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 💰 [PPC 廣告策略師](paid-media/paid-media-ppc-strategist.md) | Google/Microsoft/Amazon 廣告、帳戶架構、出價 | 帳戶建置、預算分配、規模擴展、效果診斷 |
| 🔍 [搜尋查詢分析師](paid-media/paid-media-search-query-analyst.md) | 搜尋詞分析、否定關鍵字、意圖對應 | 查詢稽核、浪費消除、關鍵字發掘 |
| 📋 [付費媒體稽核師](paid-media/paid-media-auditor.md) | 200+ 項帳戶稽核、競爭分析 | 帳戶接管、季度審查、競爭提案 |
| 📡 [追蹤與衡量專家](paid-media/paid-media-tracking-specialist.md) | GTM、GA4、轉換追蹤、CAPI | 新建部署、追蹤稽核、平台遷移 |
| ✍️ [廣告創意策略師](paid-media/paid-media-creative-strategist.md) | RSA 文案、Meta 創意、Performance Max 素材 | 創意上線、測試計劃、廣告疲勞刷新 |
| 📺 [程式化與展示廣告買家](paid-media/paid-media-programmatic-buyer.md) | GDN、DSP、合作媒體、ABM 展示 | 展示廣告規劃、合作夥伴拓展、ABM 方案 |
| 📱 [付費社群策略師](paid-media/paid-media-paid-social-strategist.md) | Meta、LinkedIn、TikTok、跨平台社群 | 社群廣告方案、平台選擇、受眾策略 |

### 💼 銷售部門

透過技巧將管線轉化為營收，而非 CRM 瑣事。

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 🎯 [外展策略師](sales/sales-outbound-strategist.md) | 信號導向的潛客開發、多通路序列、ICP 定位 | 透過研究驅動的觸及建立管線，而非量海戰術 |
| 🔍 [探索教練](sales/sales-discovery-coach.md) | SPIN、Gap Selling、Sandler — 問題設計與通話結構 | 探索通話準備、機會確認、業務代表指導 |
| ♟️ [交易策略師](sales/sales-deal-strategist.md) | MEDDPICC 確認、競爭定位、贏單規劃 | 交易評分、管線風險暴露、贏單策略 |
| 🛠️ [售前工程師](sales/sales-engineer.md) | 技術演示、POC 範圍界定、競爭戰報 | 售前技術贏單、演示準備、競爭定位 |
| 🏹 [提案策略師](sales/sales-proposal-strategist.md) | RFP 回應、贏單主題、敘事結構 | 撰寫有說服力的提案，而非僅滿足合規 |
| 📊 [管線分析師](sales/sales-pipeline-analyst.md) | 預測、管線健康度、交易速度、RevOps | 管線審查、預測準確度、營收運營 |
| 🗺️ [客戶策略師](sales/sales-account-strategist.md) | 落地擴展、QBR、利害關係人對應 | 售後擴展、客戶規劃、NRR 成長 |
| 🏋️ [銷售教練](sales/sales-coach.md) | 業務代表培養、通話指導、管線審查引導 | 透過結構化指導讓每位業務與每筆交易更好 |

### 📢 行銷部門

一次真誠的互動，拓展你的受眾。

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 🚀 [成長駭客](marketing/marketing-growth-hacker.md) | 快速用戶獲取、病毒迴圈、實驗 | 爆發式成長、用戶獲取、轉換優化 |
| 📝 [內容創作者](marketing/marketing-content-creator.md) | 多平台內容、編輯行事曆 | 內容策略、文案撰寫、品牌敘事 |
| 🐦 [Twitter 互動者](marketing/marketing-twitter-engager.md) | 即時互動、思想領袖 | Twitter 策略、LinkedIn 活動、專業社群 |
| 📱 [TikTok 策略師](marketing/marketing-tiktok-strategist.md) | 病毒內容、演算法優化 | TikTok 成長、病毒內容、Z 世代/千禧世代受眾 |
| 📸 [Instagram 策展人](marketing/marketing-instagram-curator.md) | 視覺敘事、社群建立 | Instagram 策略、美學發展、視覺內容 |
| 🤝 [Reddit 社群建構者](marketing/marketing-reddit-community-builder.md) | 真誠互動、價值導向內容 | Reddit 策略、社群信任、真誠行銷 |
| 📱 [App Store 優化師](marketing/marketing-app-store-optimizer.md) | ASO、轉換優化、曝光度 | 應用行銷、商店優化、應用成長 |
| 🌐 [社群媒體策略師](marketing/marketing-social-media-strategist.md) | 跨平台策略、活動 | 整體社群策略、多平台活動 |
| 📕 [小紅書專家](marketing/marketing-xiaohongshu-specialist.md) | 生活風格內容、趨勢驅動策略 | 小紅書成長、美學敘事、Z 世代受眾 |
| 💬 [微信公眾號管理者](marketing/marketing-wechat-official-account.md) | 訂閱者互動、內容行銷 | 微信公眾號策略、社群建立、轉換優化 |
| 🧠 [知乎策略師](marketing/marketing-zhihu-strategist.md) | 思想領袖、知識驅動互動 | 知乎權威建立、問答策略、潛客開發 |
| 🇨🇳 [百度 SEO 專家](marketing/marketing-baidu-seo-specialist.md) | 百度優化、中國 SEO、ICP 合規 | 百度排名與觸及中國搜尋市場 |
| 🎬 [Bilibili 內容策略師](marketing/marketing-bilibili-content-strategist.md) | B 站演算法、彈幕文化、UP 主成長 | 在 Bilibili 以社群優先的內容建立受眾 |
| 🎠 [輪播成長引擎](marketing/marketing-carousel-growth-engine.md) | TikTok/Instagram 輪播、自主發布 | 生成並發布病毒式輪播內容 |
| 💼 [LinkedIn 內容創作者](marketing/marketing-linkedin-content-creator.md) | 個人品牌、思想領袖、專業內容 | LinkedIn 成長、專業受眾建立、B2B 內容 |
| 🛒 [中國電商運營師](marketing/marketing-china-ecommerce-operator.md) | 淘寶、天貓、拼多多、直播帶貨 | 經營中國多平台電商 |
| 🎥 [快手策略師](marketing/marketing-kuaishou-strategist.md) | 快手、老鐵社群、草根成長 | 在下沉市場建立真實受眾 |
| 🔍 [SEO 專家](marketing/marketing-seo-specialist.md) | 技術 SEO、內容策略、連結建設 | 推動可持續的自然搜尋成長 |
| 📘 [書籍共同作者](marketing/marketing-book-co-author.md) | 思想領袖書籍、代筆、出版 | 為創辦人與專家進行策略性書籍合作 |
| 🌏 [跨境電商專家](marketing/marketing-cross-border-ecommerce.md) | Amazon、Shopee、Lazada、跨境物流 | 全漏斗跨境電商策略 |
| 🎵 [抖音策略師](marketing/marketing-douyin-strategist.md) | 抖音平台、短影片行銷、演算法 | 在中國領先短影片平台上拓展受眾 |
| 🎙️ [直播帶貨教練](marketing/marketing-livestream-commerce-coach.md) | 主播培訓、直播間優化、轉換 | 建構高績效直播電商運營 |
| 🎧 [Podcast 策略師](marketing/marketing-podcast-strategist.md) | Podcast 內容策略、平台優化 | 中國 Podcast 市場策略與運營 |
| 🔒 [私域運營師](marketing/marketing-private-domain-operator.md) | 企業微信、私域流量、社群運營 | 建構企業微信私域生態系統 |
| 🎬 [短影片剪輯教練](marketing/marketing-short-video-editing-coach.md) | 後製、剪輯工作流程、平台規格 | 實操短影片剪輯培訓與優化 |
| 🔥 [微博策略師](marketing/marketing-weibo-strategist.md) | 新浪微博、熱門話題、粉絲互動 | 全方位微博運營與成長 |
| 🔮 [AI 引用策略師](marketing/marketing-ai-citation-strategist.md) | AEO/GEO、AI 推薦可見度、引用稽核 | 提升品牌在 ChatGPT、Claude、Gemini、Perplexity 中的可見度 |

### 📊 產品部門

在對的時間做對的事。

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 🎯 [衝刺優先級排序師](product/product-sprint-prioritizer.md) | 敏捷規劃、功能優先排序 | 衝刺規劃、資源分配、待辦清單管理 |
| 🔍 [趨勢研究員](product/product-trend-researcher.md) | 市場情報、競爭分析 | 市場研究、機會評估、趨勢辨識 |
| 💬 [回饋綜合師](product/product-feedback-synthesizer.md) | 使用者回饋分析、洞察提取 | 回饋分析、使用者洞察、產品優先級 |
| 🧠 [行為推力引擎](product/product-behavioral-nudge-engine.md) | 行為心理學、推力設計、參與度 | 透過行為科學最大化使用者動機 |
| 🧭 [產品經理](product/product-manager.md) | 全生命週期產品負責 | 探索、PRD、路線圖規劃、GTM、成果衡量 |

### 🎬 專案管理部門

確保專案準時交付（且不超預算）。

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 🎬 [工作室製作人](project-management/project-management-studio-producer.md) | 高層協調、專案組合管理 | 多專案監督、策略對齊、資源分配 |
| 🐑 [專案牧羊人](project-management/project-management-project-shepherd.md) | 跨職能協調、時程管理 | 端到端專案協調、利害關係人管理 |
| ⚙️ [工作室營運](project-management/project-management-studio-operations.md) | 日常效率、流程優化 | 卓越營運、團隊支援、生產力 |
| 🧪 [實驗追蹤器](project-management/project-management-experiment-tracker.md) | A/B 測試、假設驗證 | 實驗管理、資料驅動決策、測試 |
| 👔 [資深專案經理](project-management/project-manager-senior.md) | 務實範圍界定、任務轉換 | 將規格轉換為任務、範圍管理 |
| 📋 [Jira 工作流程管家](project-management/project-management-jira-workflow-steward.md) | Git 工作流程、分支策略、可追溯性 | 強化 Jira 連結的 Git 紀律與交付 |

### 🧪 測試部門

我們先把東西弄壞，讓使用者不必承受。

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 📸 [證據收集員](testing/testing-evidence-collector.md) | 截圖式 QA、視覺證明 | UI 測試、視覺驗證、錯誤文件 |
| 🔍 [現實查核員](testing/testing-reality-checker.md) | 證據導向認證、品質關卡 | 生產就緒度、品質核准、發佈認證 |
| 📊 [測試結果分析師](testing/testing-test-results-analyzer.md) | 測試評估、指標分析 | 測試輸出分析、品質洞察、覆蓋率報告 |
| ⚡ [效能基準測試師](testing/testing-performance-benchmarker.md) | 效能測試、優化 | 速度測試、負載測試、效能調校 |
| 🔌 [API 測試師](testing/testing-api-tester.md) | API 驗證、整合測試 | API 測試、端點驗證、整合 QA |
| 🛠️ [工具評估師](testing/testing-tool-evaluator.md) | 技術評估、工具選擇 | 評估工具、軟體建議、技術決策 |
| 🔄 [工作流程優化師](testing/testing-workflow-optimizer.md) | 流程分析、工作流程改善 | 流程優化、效率提升、自動化機會 |
| ♿ [無障礙稽核師](testing/testing-accessibility-auditor.md) | WCAG 稽核、輔助技術測試 | 無障礙合規、螢幕閱讀器測試、包容性設計驗證 |

### 🛟 支援部門

營運的中流砥柱。

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 💬 [客服回應者](support/support-support-responder.md) | 客戶服務、問題解決 | 客戶支援、使用者體驗、支援營運 |
| 📊 [分析報表師](support/support-analytics-reporter.md) | 資料分析、儀表板、洞察 | 商業智慧、KPI 追蹤、資料視覺化 |
| 💰 [財務追蹤師](support/support-finance-tracker.md) | 財務規劃、預算管理 | 財務分析、現金流、營運績效 |
| 🏗️ [基礎設施維護師](support/support-infrastructure-maintainer.md) | 系統可靠性、效能優化 | 基礎設施管理、系統營運、監控 |
| ⚖️ [法規合規查核員](support/support-legal-compliance-checker.md) | 合規、法規、法律審查 | 法律合規、法規要求、風險管理 |
| 📑 [高管摘要產生器](support/support-executive-summary-generator.md) | C-suite 溝通、策略摘要 | 高管報告、策略溝通、決策支援 |

### 🥽 空間運算部門

建構沉浸式未來。

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 🏗️ [XR 介面架構師](spatial-computing/xr-interface-architect.md) | 空間互動設計、沉浸式 UX | AR/VR/XR 介面設計、空間運算 UX |
| 💻 [macOS 空間/Metal 工程師](spatial-computing/macos-spatial-metal-engineer.md) | Swift、Metal、高效能 3D | macOS 空間運算、Vision Pro 原生應用 |
| 🌐 [XR 沉浸式開發者](spatial-computing/xr-immersive-developer.md) | WebXR、瀏覽器 AR/VR | 瀏覽器沉浸式體驗、WebXR 應用 |
| 🎮 [XR 座艙互動專家](spatial-computing/xr-cockpit-interaction-specialist.md) | 座艙控制、沉浸式系統 | 座艙控制系統、沉浸式控制介面 |
| 🍎 [visionOS 空間工程師](spatial-computing/visionos-spatial-engineer.md) | Apple Vision Pro 開發 | Vision Pro 應用、空間運算體驗 |
| 🔌 [終端機整合專家](spatial-computing/terminal-integration-specialist.md) | 終端機整合、命令列工具 | CLI 工具、終端機工作流程、開發者工具 |

### 🎯 專業部門

獨特的專家，無法歸入任何單一類別。

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 🎭 [Agent 協調者](specialized/agents-orchestrator.md) | 多 Agent 協調、工作流程管理 | 需要多 Agent 協調的複雜專案 |
| 🔍 [LSP/索引工程師](specialized/lsp-index-engineer.md) | Language Server Protocol、程式碼智慧 | 程式碼智慧系統、LSP 實作、語義索引 |
| 📥 [銷售資料擷取 Agent](specialized/sales-data-extraction-agent.md) | Excel 監控、銷售指標擷取 | 銷售資料匯入、MTD/YTD/年度指標 |
| 📈 [資料整合 Agent](specialized/data-consolidation-agent.md) | 銷售資料彙總、儀表板報表 | 區域摘要、業務代表績效、管線快照 |
| 📬 [報表分發 Agent](specialized/report-distribution-agent.md) | 自動化報表發送 | 依區域的報表分發、排程發送 |
| 🔐 [Agent 身份與信任架構師](specialized/agentic-identity-trust.md) | Agent 身份、驗證、信任確認 | 多 Agent 身份系統、Agent 授權、稽核軌跡 |
| 🔗 [身份圖譜操作員](specialized/identity-graph-operator.md) | 多 Agent 系統的共享身份解析 | 實體去重、合併提案、跨 Agent 身份一致性 |
| 💸 [應付帳款 Agent](specialized/accounts-payable-agent.md) | 支付處理、供應商管理、稽核 | 跨加密貨幣、法幣、穩定幣的自主支付執行 |
| 🛡️ [區塊鏈安全稽核師](specialized/blockchain-security-auditor.md) | 智慧合約稽核、漏洞分析 | 在部署前發現合約漏洞 |
| 📋 [合規稽核師](specialized/compliance-auditor.md) | SOC 2、ISO 27001、HIPAA、PCI-DSS | 指導組織完成合規認證 |
| 🌍 [文化智慧策略師](specialized/specialized-cultural-intelligence-strategist.md) | 全球 UX、代表性、文化排除 | 確保軟體在不同文化中產生共鳴 |
| 🗣️ [開發者倡導者](specialized/specialized-developer-advocate.md) | 社群建立、DX、開發者內容 | 橋接產品與開發者社群 |
| 🔬 [模型 QA 專家](specialized/specialized-model-qa.md) | ML 稽核、特徵分析、可解釋性 | 機器學習模型的端到端 QA |
| 🗃️ [ZK 管家](specialized/zk-steward.md) | 知識管理、Zettelkasten、筆記 | 建構連結且經驗證的知識庫 |
| 🔌 [MCP 建構者](specialized/specialized-mcp-builder.md) | Model Context Protocol 伺服器、AI Agent 工具 | 建構擴展 AI Agent 能力的 MCP 伺服器 |
| 📄 [文件產生器](specialized/specialized-document-generator.md) | PDF、PPTX、DOCX、XLSX 程式碼生成 | 專業文件製作、報表、資料視覺化 |
| ⚙️ [自動化治理架構師](specialized/automation-governance-architect.md) | 自動化治理、n8n、工作流程稽核 | 大規模評估與治理業務自動化 |
| 📚 [企業培訓設計師](specialized/corporate-training-designer.md) | 企業培訓、課程開發 | 設計培訓系統與學習計畫 |
| 🏛️ [政府數位轉型售前顧問](specialized/government-digital-presales-consultant.md) | 中國 ToG 售前、數位轉型 | 政府數位轉型提案與投標 |
| ⚕️ [醫療行銷合規](specialized/healthcare-marketing-compliance.md) | 中國醫療廣告合規 | 醫療行銷法規合規 |
| 🎯 [招募專家](specialized/recruitment-specialist.md) | 人才招募、招募營運 | 招募策略、人才搜尋與錄用流程 |
| 🎓 [留學顧問](specialized/study-abroad-advisor.md) | 國際教育、申請規劃 | 美國、英國、加拿大、澳洲留學規劃 |
| 🔗 [供應鏈策略師](specialized/supply-chain-strategist.md) | 供應鏈管理、採購策略 | 供應鏈優化與採購規劃 |
| 🗺️ [工作流程架構師](specialized/specialized-workflow-architect.md) | 工作流程發掘、對應與規格 | 在寫程式前對應系統中的每條路徑 |
| ☁️ [Salesforce 架構師](specialized/specialized-salesforce-architect.md) | 多雲 Salesforce 設計、Governor Limits、整合 | 企業 Salesforce 架構、組織策略、部署管線 |
| 🇫🇷 [法國顧問市場導航員](specialized/specialized-french-consulting-market.md) | ESN/SI 生態、Portage Salarial、費率定位 | 法國 IT 市場的自由顧問 |
| 🇰🇷 [韓國商務導航員](specialized/specialized-korean-business-navigator.md) | 韓國商業文化、品議流程、關係機制 | 外籍專業人士在韓國商務關係中的導航 |

### 🎮 遊戲開發部門

橫跨所有主要引擎，建構世界、系統與體驗。

#### 跨引擎 Agent（引擎無關）

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 🎯 [遊戲設計師](game-development/game-designer.md) | 系統設計、GDD 撰寫、經濟平衡、遊戲循環 | 設計遊戲機制、進程系統、撰寫設計文件 |
| 🗺️ [關卡設計師](game-development/level-designer.md) | 佈局理論、節奏、遭遇設計、環境敘事 | 建構關卡、設計遭遇流程、空間敘事 |
| 🎨 [技術美術](game-development/technical-artist.md) | Shader、VFX、LOD 管線、美術到引擎優化 | 橋接美術與工程、Shader 編寫、效能安全的素材管線 |
| 🔊 [遊戲音效工程師](game-development/game-audio-engineer.md) | FMOD/Wwise、自適應音樂、空間音效、音效預算 | 互動音效系統、動態音樂、音效效能 |
| 📖 [敘事設計師](game-development/narrative-designer.md) | 故事系統、分支對話、世界觀架構 | 撰寫分支敘事、實作對話系統、世界觀設定 |

#### Unity

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 🏗️ [Unity 架構師](game-development/unity/unity-architect.md) | ScriptableObjects、資料驅動模組化、DOTS/ECS | 大型 Unity 專案、資料驅動系統設計、ECS 效能工作 |
| ✨ [Unity Shader Graph 美術](game-development/unity/unity-shader-graph-artist.md) | Shader Graph、HLSL、URP/HDRP、Renderer Features | 自訂 Unity 材質、VFX Shader、後處理 Pass |
| 🌐 [Unity 多人連線工程師](game-development/unity/unity-multiplayer-engineer.md) | Netcode for GameObjects、Unity Relay/Lobby、伺服器權威、預測 | 線上 Unity 遊戲、客戶端預測、Unity Gaming Services 整合 |
| 🛠️ [Unity 編輯器工具開發者](game-development/unity/unity-editor-tool-developer.md) | EditorWindows、AssetPostprocessors、PropertyDrawers、建置驗證 | 自訂 Unity 編輯器工具、管線自動化、內容驗證 |

#### Unreal Engine

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| ⚙️ [Unreal 系統工程師](game-development/unreal-engine/unreal-systems-engineer.md) | C++/Blueprint 混合、GAS、Nanite 限制、記憶體管理 | 複雜 Unreal 遊戲系統、Gameplay Ability System、引擎級 C++ |
| 🎨 [Unreal 技術美術](game-development/unreal-engine/unreal-technical-artist.md) | Material Editor、Niagara、PCG、Substrate | Unreal 材質、Niagara VFX、程序化內容生成 |
| 🌐 [Unreal 多人連線架構師](game-development/unreal-engine/unreal-multiplayer-architect.md) | Actor 同步、GameMode/GameState 階層、專用伺服器 | Unreal 線上遊戲、同步圖、伺服器權威 Unreal |
| 🗺️ [Unreal 世界建構者](game-development/unreal-engine/unreal-world-builder.md) | World Partition、Landscape、HLOD、LWC | 大型開放世界 Unreal 關卡、串流系統、大規模地形 |

#### Godot

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 📜 [Godot 遊戲腳本師](game-development/godot/godot-gameplay-scripter.md) | GDScript 2.0、訊號、組合、靜態型別 | Godot 遊戲系統、場景組合、效能導向 GDScript |
| 🌐 [Godot 多人連線工程師](game-development/godot/godot-multiplayer-engineer.md) | MultiplayerAPI、ENet/WebRTC、RPC、權威模型 | 線上 Godot 遊戲、場景同步、伺服器權威 Godot |
| ✨ [Godot Shader 開發者](game-development/godot/godot-shader-developer.md) | Godot 著色語言、VisualShader、RenderingDevice | 自訂 Godot 材質、2D/3D 效果、後處理、Compute Shader |

#### Blender

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 🧩 [Blender 外掛工程師](game-development/blender/blender-addon-engineer.md) | Blender Python (`bpy`)、自訂運算子/面板、素材驗證器、匯出器、管線自動化 | 建構 Blender 外掛、素材準備工具、匯出工作流程、DCC 管線自動化 |

#### Roblox Studio

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| ⚙️ [Roblox 系統腳本師](game-development/roblox-studio/roblox-systems-scripter.md) | Luau、RemoteEvents/Functions、DataStore、伺服器權威模組架構 | 建構安全的 Roblox 遊戲系統、客戶端-伺服器通訊、資料持久化 |
| 🎯 [Roblox 體驗設計師](game-development/roblox-studio/roblox-experience-designer.md) | 參與循環、商業化、D1/D7 留存、引導流程 | 設計 Roblox 遊戲循環、Game Passes、每日獎勵、玩家留存 |
| 👗 [Roblox 虛擬角色創作者](game-development/roblox-studio/roblox-avatar-creator.md) | UGC 管線、配件綁定、Creator Marketplace 提交 | Roblox UGC 物品、HumanoidDescription 自訂、遊戲內虛擬角色商店 |

### 📚 學術部門

為世界建構、敘事和故事設計帶來學術嚴謹。

| Agent | 專長 | 適用情境 |
|-------|------|---------|
| 🌍 [人類學家](academic/academic-anthropologist.md) | 文化系統、親屬關係、儀式、信仰系統 | 設計具有內部邏輯的文化連貫社會 |
| 🌐 [地理學家](academic/academic-geographer.md) | 自然/人文地理、氣候、地圖學 | 建構地理連貫的世界，含真實地形與聚落 |
| 📚 [歷史學家](academic/academic-historian.md) | 歷史分析、時代分期、物質文化 | 驗證歷史連貫性、以真實時代細節豐富場景 |
| 📜 [敘事學家](academic/academic-narratologist.md) | 敘事理論、故事結構、角色弧線 | 以成熟理論框架分析和改善故事結構 |
| 🧠 [心理學家](academic/academic-psychologist.md) | 人格理論、動機、認知模式 | 建構根植於研究的心理學可信角色 |

---

## 🎯 實際使用案例

### 情境一：建構新創 MVP

**你的團隊**：
1. 🎨 **前端開發者** — 建構 React 應用
2. 🏗️ **後端架構師** — 設計 API 與資料庫
3. 🚀 **成長駭客** — 規劃用戶獲取
4. ⚡ **快速原型師** — 快速迭代循環
5. 🔍 **現實查核員** — 上線前確保品質

**成果**：在每個階段都有專業能力，加速交付。

---

### 情境二：行銷活動上線

**你的團隊**：
1. 📝 **內容創作者** — 開發活動內容
2. 🐦 **Twitter 互動者** — Twitter 策略與執行
3. 📸 **Instagram 策展人** — 視覺內容與限時動態
4. 🤝 **Reddit 社群建構者** — 真誠的社群互動
5. 📊 **分析報表師** — 追蹤與優化績效

**成果**：多通路協調活動，每個平台都有專業能力。

---

### 情境三：企業功能開發

**你的團隊**：
1. 👔 **資深專案經理** — 範圍界定與任務規劃
2. 💎 **資深開發者** — 複雜實作
3. 🎨 **UI 設計師** — 設計系統與元件
4. 🧪 **實驗追蹤器** — A/B 測試規劃
5. 📸 **證據收集員** — 品質驗證
6. 🔍 **現實查核員** — 生產就緒度

**成果**：企業級交付，含品質關卡與文件。

---

### 情境五：付費媒體帳戶接管

**你的團隊**：
1. 📋 **付費媒體稽核師** — 全面帳戶評估
2. 📡 **追蹤與衡量專家** — 驗證轉換追蹤準確度
3. 💰 **PPC 廣告策略師** — 重新設計帳戶架構
4. 🔍 **搜尋查詢分析師** — 從搜尋詞清理浪費支出
5. ✍️ **廣告創意策略師** — 刷新所有廣告文案與擴充
6. 📊 **分析報表師**（支援部門）— 建構報告儀表板

**成果**：系統化的帳戶接管 — 在前 30 天內完成追蹤驗證、浪費消除、結構優化和創意刷新。

---

### 情境四：完整 Agency 產品探索

**你的團隊**：全部 8 個部門並行投入同一使命。

參見 **[Nexus 空間探索演練](examples/nexus-spatial-discovery.md)** — 一個完整範例，8 位 Agent（產品趨勢研究員、後端架構師、品牌守護者、成長駭客、客服回應者、UX 研究員、專案牧羊人和 XR 介面架構師）同時部署來評估一個軟體機會，產出涵蓋市場驗證、技術架構、品牌策略、上市策略、支援系統、UX 研究、專案執行和空間 UI 設計的統一產品計畫。

**成果**：在單一工作階段中產出全面的跨職能產品藍圖。[更多範例](examples/)。

---

## 🤝 如何貢獻

我們歡迎貢獻！以下是您可以參與的方式：

### 新增 Agent

1. Fork 此倉庫
2. 在適當的分類中建立新的 agent 檔案
3. 遵循 agent 模板結構：
   - 含 name、description、color 的 Frontmatter
   - 身份與記憶區段
   - 核心使命
   - 關鍵規則（領域特定）
   - 技術交付成果與範例
   - 工作流程
   - 成功指標
4. 提交包含您的 agent 的 PR

### 改善現有 Agent

- 增加真實世界範例
- 強化程式碼範例
- 更新成功指標
- 改善工作流程

### 分享您的成功案例

成功使用了這些 agents 嗎？在[討論區](https://github.com/msitarzewski/agency-agents/discussions)分享您的故事！

---

## 📖 Agent 設計理念

每個 agent 的設計原則：

1. **🎭 鮮明人格**：非通用模板 — 真正的角色與聲音
2. **📋 明確交付成果**：具體的產出，而非模糊的指導
3. **✅ 成功指標**：可衡量的成果與品質標準
4. **🔄 驗證過的工作流程**：行之有效的步驟化流程
5. **💡 學習記憶**：模式辨識與持續改善

---

## 🎁 這有什麼特別？

### 不同於通用 AI 提示詞：
- ❌ 通用的「扮演一個開發者」提示詞
- ✅ 具備人格和流程的深度專業化

### 不同於提示詞庫：
- ❌ 一次性的提示詞集合
- ✅ 包含工作流程和交付成果的完整 agent 系統

### 不同於 AI 工具：
- ❌ 無法自訂的黑盒工具
- ✅ 透明、可 fork、可調整的 agent 人格

---

## 🎨 Agent 人格亮點

> 「我不只是測試你的程式碼 — 我預設會找出 3-5 個問題，而且每件事都需要視覺證據。」
>
> — **證據收集員**（測試部門）

> 「你不是在 Reddit 上做行銷 — 你是在成為一個受重視的社群成員，碰巧代表一個品牌。」
>
> — **Reddit 社群建構者**（行銷部門）

> 「每個趣味元素都必須服務於功能性或情感性目的。設計能增強而非分散注意力的愉悅感。」
>
> — **趣味注入師**（設計部門）

> 「讓我加一個慶祝動畫，它能降低 40% 的任務完成焦慮。」
>
> — **趣味注入師**（UX 審查中）

---

## 📊 數據統計

- 🎭 **144 個專業 Agent**，橫跨 12 個部門
- 📝 **超過 10,000 行**人格、流程和程式碼範例
- ⏱️ **數月迭代**，源自真實世界使用
- 🌟 **經實戰驗證**，已在生產環境中應用
- 💬 **首 12 小時超過 50 個請求**，來自 Reddit

---

## 🔌 多工具整合

The Agency 原生支援 Claude Code，並提供轉換和安裝腳本，讓您可以在所有主流 AI 程式碼工具中使用相同的 agents。

### 支援工具

- **[Claude Code](https://claude.ai/code)** — 原生 `.md` agents，無需轉換 → `~/.claude/agents/`
- **[GitHub Copilot](https://github.com/copilot)** — 原生 `.md` agents，無需轉換 → `~/.github/agents/` + `~/.copilot/agents/`
- **[Antigravity](https://github.com/google-gemini/antigravity)** — 每個 agent 一個 `SKILL.md` → `~/.gemini/antigravity/skills/`
- **[Gemini CLI](https://github.com/google-gemini/gemini-cli)** — 擴充功能 + `SKILL.md` 檔案 → `~/.gemini/extensions/agency-agents/`
- **[OpenCode](https://opencode.ai)** — `.md` agent 檔案 → `.opencode/agents/`
- **[Cursor](https://cursor.sh)** — `.mdc` 規則檔 → `.cursor/rules/`
- **[Aider](https://aider.chat)** — 單一 `CONVENTIONS.md` → `./CONVENTIONS.md`
- **[Windsurf](https://codeium.com/windsurf)** — 單一 `.windsurfrules` → `./.windsurfrules`
- **[OpenClaw](https://github.com/openclaw/openclaw)** — `SOUL.md` + `AGENTS.md` + `IDENTITY.md`（每個 agent）
- **[Qwen Code](https://github.com/QwenLM/qwen-code)** — `.md` SubAgent 檔案 → `~/.qwen/agents/`

---

### ⚡ 快速安裝

**步驟 1 — 產生整合檔案：**
```bash
./scripts/convert.sh
# 更快（平行，輸出順序可能不同）：./scripts/convert.sh --parallel
```

**步驟 2 — 安裝（互動式，自動偵測您的工具）：**
```bash
./scripts/install.sh
# 更快（平行，輸出順序可能不同）：./scripts/install.sh --no-interactive --parallel
```

安裝程式會掃描系統中已安裝的工具，顯示勾選 UI，讓您精確選擇要安裝的項目：

```
  +------------------------------------------------+
  |   The Agency -- 工具安裝程式                     |
  +------------------------------------------------+

  系統掃描：[*] = 偵測到已安裝

  [x]  1)  [*]  Claude Code     (claude.ai/code)
  [x]  2)  [*]  Copilot         (~/.github + ~/.copilot)
  [x]  3)  [*]  Antigravity     (~/.gemini/antigravity)
  [ ]  4)  [ ]  Gemini CLI      (gemini extension)
  [ ]  5)  [ ]  OpenCode        (opencode.ai)
  [ ]  6)  [ ]  OpenClaw        (~/.openclaw)
  [x]  7)  [*]  Cursor          (.cursor/rules)
  [ ]  8)  [ ]  Aider           (CONVENTIONS.md)
  [ ]  9)  [ ]  Windsurf        (.windsurfrules)
  [ ] 10)  [ ]  Qwen Code       (~/.qwen/agents)

  [1-10] 切換   [a] 全選   [n] 全不選   [d] 偵測到的
  [Enter] 安裝   [q] 離開
```

**或直接安裝特定工具：**
```bash
./scripts/install.sh --tool cursor
./scripts/install.sh --tool opencode
./scripts/install.sh --tool openclaw
./scripts/install.sh --tool antigravity
```

**非互動模式（CI/腳本）：**
```bash
./scripts/install.sh --no-interactive --tool all
```

**加速執行（平行）** — 在多核心機器上，使用 `--parallel` 讓每個工具平行處理。跨工具的輸出順序不確定。可搭配互動和非互動安裝使用：例如 `./scripts/install.sh --interactive --parallel`（選擇工具後平行安裝）或 `./scripts/install.sh --no-interactive --parallel`。工作數預設為 `nproc`（Linux）、`sysctl -n hw.ncpu`（macOS）或 4；可用 `--jobs N` 覆寫。

```bash
./scripts/convert.sh --parallel                    # 平行轉換所有工具
./scripts/convert.sh --parallel --jobs 8           # 限制平行工作數
./scripts/install.sh --no-interactive --parallel   # 平行安裝所有偵測到的工具
./scripts/install.sh --interactive --parallel      # 選擇工具後平行安裝
./scripts/install.sh --no-interactive --parallel --jobs 4
```

---

### 各工具詳細說明

<details>
<summary><strong>Claude Code</strong></summary>

Agents 從倉庫直接複製到 `~/.claude/agents/` — 無需轉換。

```bash
./scripts/install.sh --tool claude-code
```

在 Claude Code 中啟用：
```
Use the Frontend Developer agent to review this component.
```

詳見 [integrations/claude-code/README.md](integrations/claude-code/README.md)。
</details>

<details>
<summary><strong>GitHub Copilot</strong></summary>

Agents 從倉庫直接複製到 `~/.github/agents/` 和 `~/.copilot/agents/` — 無需轉換。

```bash
./scripts/install.sh --tool copilot
```

在 GitHub Copilot 中啟用：
```
Use the Frontend Developer agent to review this component.
```

詳見 [integrations/github-copilot/README.md](integrations/github-copilot/README.md)。
</details>

<details>
<summary><strong>Antigravity (Gemini)</strong></summary>

每個 agent 成為 `~/.gemini/antigravity/skills/agency-<slug>/` 中的技能。

```bash
./scripts/install.sh --tool antigravity
```

在 Gemini 中搭配 Antigravity 啟用：
```
@agency-frontend-developer review this React component
```

詳見 [integrations/antigravity/README.md](integrations/antigravity/README.md)。
</details>

<details>
<summary><strong>Gemini CLI</strong></summary>

安裝為 Gemini CLI 擴充功能，每個 agent 一個技能加一個清單。
首次 clone 時，先產生 Gemini 擴充檔案再執行安裝程式。

```bash
./scripts/convert.sh --tool gemini-cli
./scripts/install.sh --tool gemini-cli
```

詳見 [integrations/gemini-cli/README.md](integrations/gemini-cli/README.md)。
</details>

<details>
<summary><strong>OpenCode</strong></summary>

Agents 放置在專案根目錄的 `.opencode/agents/` 中（專案範圍）。

```bash
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool opencode
```

或全域安裝：
```bash
mkdir -p ~/.config/opencode/agents
cp integrations/opencode/agents/*.md ~/.config/opencode/agents/
```

在 OpenCode 中啟用：
```
@backend-architect design this API.
```

詳見 [integrations/opencode/README.md](integrations/opencode/README.md)。
</details>

<details>
<summary><strong>Cursor</strong></summary>

每個 agent 成為專案中 `.cursor/rules/` 的 `.mdc` 規則檔。

```bash
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool cursor
```

當 Cursor 在專案中偵測到規則時會自動套用。明確引用：
```
Use the @security-engineer rules to review this code.
```

詳見 [integrations/cursor/README.md](integrations/cursor/README.md)。
</details>

<details>
<summary><strong>Aider</strong></summary>

所有 agents 編譯為 Aider 會自動讀取的單一 `CONVENTIONS.md` 檔案。

```bash
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool aider
```

在 Aider 工作階段中引用 agents：
```
Use the Frontend Developer agent to refactor this component.
```

詳見 [integrations/aider/README.md](integrations/aider/README.md)。
</details>

<details>
<summary><strong>Windsurf</strong></summary>

所有 agents 編譯為專案根目錄的 `.windsurfrules`。

```bash
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool windsurf
```

在 Windsurf 的 Cascade 中引用 agents：
```
Use the Reality Checker agent to verify this is production ready.
```

詳見 [integrations/windsurf/README.md](integrations/windsurf/README.md)。
</details>

<details>
<summary><strong>OpenClaw</strong></summary>

每個 agent 成為 `~/.openclaw/agency-agents/` 中含 `SOUL.md`、`AGENTS.md` 和 `IDENTITY.md` 的工作空間。

```bash
./scripts/install.sh --tool openclaw
```

Agents 在 OpenClaw 工作階段中按 `agentId` 註冊並可用。

詳見 [integrations/openclaw/README.md](integrations/openclaw/README.md)。

</details>

<details>
<summary><strong>Qwen Code</strong></summary>

SubAgents 安裝到專案根目錄的 `.qwen/agents/`（專案範圍）。

```bash
# 轉換並安裝（從專案根目錄執行）
cd /your/project
./scripts/convert.sh --tool qwen
./scripts/install.sh --tool qwen
```

**在 Qwen Code 中使用：**
- 按名稱引用：`Use the frontend-developer agent to review this component`
- 或讓 Qwen 根據任務上下文自動分派
- 透過互動模式中的 `/agents` 指令管理

> [Qwen SubAgents 文件](https://qwenlm.github.io/qwen-code-docs/en/users/features/sub-agents/)

</details>

---

### 變更後重新產生

新增或編輯 agents 後，重新產生所有整合檔案：

```bash
./scripts/convert.sh                    # 重新產生全部（序列）
./scripts/convert.sh --parallel         # 平行重新產生全部（更快）
./scripts/convert.sh --tool cursor      # 只重新產生特定工具
```

---

## 🗺️ 路線圖

- [ ] 互動式 agent 選擇器網頁工具
- [x] 多 Agent 工作流程範例 — 詳見 [examples/](examples/)
- [x] 多工具整合腳本（Claude Code、GitHub Copilot、Antigravity、Gemini CLI、OpenCode、OpenClaw、Cursor、Aider、Windsurf、Qwen Code）
- [ ] Agent 設計影片教學
- [ ] 社群 agent 市集
- [ ] Agent「人格測驗」用於專案匹配
- [ ] 「每週精選 Agent」展示系列

---

## 🌐 社群翻譯與在地化

社群維護的翻譯與地區適配版本。這些是獨立維護的 — 請查看各倉庫的覆蓋範圍與版本相容性。

| 語言 | 維護者 | 連結 | 備註 |
|------|--------|------|------|
| 🇨🇳 簡體中文 (zh-CN) | [@jnMetaCode](https://github.com/jnMetaCode) | [agency-agents-zh](https://github.com/jnMetaCode/agency-agents-zh) | 100 個翻譯 agents + 9 個中國市場原創 |
| 🇨🇳 簡體中文 (zh-CN) | [@dsclca12](https://github.com/dsclca12) | [agent-teams](https://github.com/dsclca12/agent-teams) | 獨立翻譯，含 Bilibili、微信、小紅書在地化 |

想新增翻譯？開一個 issue，我們會在這裡連結。

---

## 🔗 相關資源

- [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) — 社群維護的 OpenClaw agent 集合（衍生自本倉庫）

---

## 📜 授權條款

MIT 授權 — 可自由用於商業或個人用途。歡迎但不強制標註出處。

---

## 🙏 致謝

從一篇關於 AI Agent 專業化的 Reddit 討論串開始，已成長為令人矚目的成果 — **橫跨 12 個部門的 147 個 agents**，由來自世界各地的貢獻者社群支持。這個倉庫中的每個 agent 之所以存在，是因為有人願意花時間編寫、測試和分享它。

感謝每一位提交 PR、回報問題、發起討論，或只是試用了某個 agent 並告訴我們效果如何的人 — 謝謝你們。正是因為你們，The Agency 才能持續進步。

---

## 💬 社群

- **GitHub Discussions**：[分享你的成功案例](https://github.com/msitarzewski/agency-agents/discussions)
- **Issues**：[回報錯誤或請求功能](https://github.com/msitarzewski/agency-agents/issues)
- **Reddit**：加入 r/ClaudeAI 的討論
- **Twitter/X**：使用 #TheAgency 標籤分享

---

## 🚀 立即開始

1. **瀏覽**上方的 agents，找到符合你需求的專家
2. **複製** agents 到 `~/.claude/agents/` 以整合 Claude Code
3. **啟用** 在 Claude 對話中引用 agents
4. **自訂** agent 人格與工作流程，符合你的具體需求
5. **分享** 你的成果並回饋社群

---

<div align="center">

**🎭 The Agency：你的 AI 夢幻團隊就緒 🎭**

[⭐ 為此倉庫加星](https://github.com/msitarzewski/agency-agents) • [🍴 Fork 它](https://github.com/msitarzewski/agency-agents/fork) • [🐛 回報問題](https://github.com/msitarzewski/agency-agents/issues) • [❤️ 贊助](https://github.com/sponsors/msitarzewski)

由社群打造，為社群服務

</div>
