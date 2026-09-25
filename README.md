# learning-map

## 中文

`learning-map` 是一套把「我想學某個主題」逐步變成**可操作的互動式學習簡報**的通用 Skill。

你不需要先知道完整課綱，也不需要知道教材應該包含哪些內容。可以從一句「我想學 X」開始，讓 Skill 協助研究主題、規劃課綱、確認教材內容，再設計與實作互動簡報。

它不限定技術、AI 或 System Design，可用於技術與工程、科學、歷史與人文、語言學習、專業訓練、流程制度、概念模型、數量與因果關係等主題。

核心原則：

> **先確定要學會什麼，再決定教材要教什麼，最後選擇最適合讓人理解的互動方式。**

### 第一次使用

如果只有一個想學的主題，可以直接說：

> 使用 learning-map 幫我製作「OAuth」的互動式學習教材。我是初學者，不知道應該學哪些內容，請先跟我規劃課綱。

也可以補充學習目的：

> 使用 learning-map 幫我學「供需曲線」。我希望最後能看懂新聞裡價格、供給與需求變化的討論。請先規劃課綱，再設計互動教材。

不需要先準備教材。Skill 會協助釐清想學什麼、學完希望做到什麼、目前程度、適合深度，以及是否有指定來源。不知道的問題可以直接回答「不知道」或「從零開始」。

### 如果已經有教材或參考資料

可以提供 PDF、文章、網站、影片、筆記、既有課綱等材料，並指定用途，例如：

> 這本 PDF 是主要教材，可以補充其他可靠來源。

> 只使用我提供的教材，不要加入外部內容。

> 內容請自行研究。這個網站只參考互動方式和視覺呈現，不要把它當教材來源。

Skill 會區分五種角色：

- **Source-constrained**：只能使用指定材料。
- **Source-led**：指定材料是主要內容來源，可在允許時補充。
- **Source-informed**：指定材料是多個參考來源之一。
- **Open research**：由 Skill 自行尋找可靠來源。
- **Presentation reference**：只參考圖解、視覺、互動或教學方式。

不同材料可以同時扮演不同角色。

### 如果已經有課綱

直接提供課綱即可。

預設不會把「已有課綱」視為「不能修改」。Skill 會先理解原本的組織方式，再用金字塔原理檢查最高層學習目標、單元支撐關係、重複與缺漏、學習順序及各單元真正要學會的內容，提出調整方向後和你確認。

如果課綱已確定，請直接說：

> 完全按照這份課綱製作，不要調整課綱。

這時會把課綱視為 locked curriculum。

### 初學者不需要負責判斷教材是否完整

Skill 會依指定材料與允許的研究範圍建立 subject model，負責檢查：

- 內容正確性與必要完整性；
- 先備知識；
- 重要概念關係；
- 常見誤解與必要邊界條件；
- 來源支持；
- 不確定性或不同觀點。

使用者主要確認：

- 這是不是想學的方向；
- 範圍和深度是否合適；
- 哪些已經會了；
- 哪些希望深入或略過；
- 案例是否符合需求。

### 製作流程

```text
學習目的
   ↓
來源與參考資料
   ↓
主題研究 / Subject Model
   ↓
金字塔原理規劃課綱
   ↓
確認範圍與深度
   ↓
Learning Objectives
   ↓
Canonical Content
   ↓
內容正確性與完整性檢查
   ↓
Interaction Storyboard
   ↓
畫面文案 / Learning Copy
   ↓
實作互動簡報
   ↓
技術驗收
   ↓
人工學習驗收
```

**Canonical Content** 是「教材真正需要正確傳達什麼」。

**Learning Copy** 是「學習者在某個互動階段實際看到哪些文字」。

兩者分開處理，避免為了畫面簡短而把概念講錯。

### 互動方式依內容決定

| 要理解的內容 | 可能使用的方式 |
| --- | --- |
| 關係、結構 | Interactive Diagram |
| 流程、順序 | Flow Simulator、Timeline |
| 因果關係 | 變數控制、情境模擬 |
| 數量關係 | Slider、Calculator、Chart |
| 分類與差異 | Sorting、Comparison、Boundary Cases |
| 空間概念 | 可操作圖解、Layer、Zoom |
| 證據與解讀 | Evidence Explorer |
| 決策與取捨 | Scenario、Design Comparison |
| 程序與技能 | Guided Practice |

互動必須真的改變學習者能觀察、比較、推論、建立或驗證的內容，不為了「看起來有互動」增加按鈕或動畫。

### 成品

預設目標是 presentation-first 的互動教材：一次聚焦一個學習問題，透過操作、圖解、動畫、比較或模擬逐步理解；文字精簡；支援清楚導覽、桌面與手機，以及 reduced-motion。

一個主題通常可以是一份獨立 interactive deck，多個主題也可以組成系列。

### 常用起手式

**完全從零開始**

> 使用 learning-map 幫我學「___」。我目前對這個主題沒有概念，請先研究，再跟我用金字塔原理規劃課綱。課綱確認後再進行教材內容與互動設計。

**有指定教材**

> 使用 learning-map 製作「___」互動教材。以我提供的資料為主要內容來源，可以補充可靠外部資料。先檢查並規劃課綱，不要直接開始做畫面。

**已有課綱，可以討論**

> 使用 learning-map 製作這份課綱。先檢查學習目標、結構、缺漏與順序，和我確認後再進行教材設計。

**課綱已鎖定**

> 使用 learning-map 完全按照這份課綱製作，不要調整章節與順序。從 canonical content 與 interaction design 開始。

**指定呈現參考**

> 使用 learning-map 製作「___」。內容來源是 A；B 只作為圖解與互動呈現參考，不要把 B 當成教材內容來源。

### Skill 與 Reference

完整規格：`SKILL.md`

第一個已完成 UI 驗收的 reference implementation：

- Repository：`gcake119/agent-system-design-learning-map`
- Route：`#/deck/token-profiler`

這個 reference 只示範已驗證的互動節奏與 presentation-first 呈現方式。Agent、Token Profiler、System Design 都不是 `learning-map` 的必要內容。

---

## English

`learning-map` is a general-purpose skill for turning **“I want to learn this topic”** into an interactive learning deck.

You do not need to know the curriculum in advance or know what the course should contain. Start with a topic and let the skill help research the subject, structure the curriculum, establish the instructional content, and design and implement the interactive experience.

It is not limited to technology, AI, or System Design. It can be used for science, history and humanities, language learning, professional training, processes, conceptual models, quantitative relationships, and other subjects.

Core principle:

> **First determine what the learner should learn, then establish what the material needs to teach, and only then choose the interaction that makes the concept easiest to understand.**

### Quick start

> Use learning-map to create an interactive learning deck about OAuth. I am a beginner and do not know what I need to learn yet. Start by planning the curriculum with me.

You may add a learning goal:

> Use learning-map to teach me supply and demand. I want to understand discussions about price, supply, and demand in the news. Plan the curriculum first, then design the interactive material.

You do not need to prepare teaching material in advance.

### Using your own materials

You may provide PDFs, articles, websites, videos, notes, or an existing curriculum and assign each source a role:

- **Source-constrained** — only specified material may define course content.
- **Source-led** — supplied material is the primary source.
- **Source-informed** — supplied material is one reference among others.
- **Open research** — the skill finds appropriate reliable sources.
- **Presentation reference** — material is used only for visual, interaction, illustration, or teaching-style reference.

Different materials may use different roles in the same project.

### Existing curriculum

An existing curriculum is not locked by default. The skill reviews its top-level learning outcome, supporting structure, gaps, overlaps, sequence, and unit-level objectives using the Pyramid Principle, then discusses proposed adjustments with you.

To lock it, say:

> Follow this curriculum exactly. Do not change its structure or order.

### Beginners do not need to validate subject completeness

The skill is responsible for source-grounded subject-matter validation: correctness, sufficient coverage, prerequisites, conceptual relationships, misconceptions, boundary cases, source support, and relevant uncertainty.

The learner primarily confirms learning intent: desired scope, depth, emphasis, prior knowledge, and useful examples.

### Workflow

```text
Learning intent
   ↓
Sources and references
   ↓
Subject research / Subject Model
   ↓
Pyramid-based curriculum design
   ↓
Scope and depth confirmation
   ↓
Learning Objectives
   ↓
Canonical Content
   ↓
Subject-matter validation
   ↓
Interaction Storyboard
   ↓
Presentation / Learning Copy
   ↓
Implementation
   ↓
Technical QA
   ↓
Human learning review
```

**Canonical Content** defines what the lesson must communicate accurately.

**Learning Copy** defines what the learner sees at a particular moment in the interactive experience.

### Interaction follows the learning problem

| Learning need | Possible interaction |
| --- | --- |
| Relationships and structure | Interactive Diagram |
| Process and sequence | Flow Simulator, Timeline |
| Cause and effect | Variable controls, scenario simulation |
| Quantitative relationships | Slider, Calculator, Chart |
| Classification and distinction | Sorting, Comparison, Boundary Cases |
| Spatial concepts | Manipulable diagrams, Layers, Zoom |
| Evidence and interpretation | Evidence Explorer |
| Decisions and trade-offs | Scenario, Design Comparison |
| Procedures and skills | Guided Practice |

Interaction should change what the learner can observe, compare, infer, construct, or verify. It should not exist only as decoration.

### Expected output

The default target is a presentation-first interactive learning experience: one learning problem at a time, progressive understanding through interaction and visualization, concise text, clear navigation, responsive use, and complete information in reduced-motion mode.

A focused topic will usually become one independent interactive deck. Multiple topics may form a series.

### Prompt examples

**Starting from zero**

> Use learning-map to teach me ___. I am new to the subject. Research it first, then plan the curriculum with me using the Pyramid Principle. After I confirm the curriculum, continue with content and interaction design.

**With source material**

> Use learning-map to create an interactive deck about ___. Treat the material I provide as the primary content source and supplement it with reliable outside sources when needed. Review the curriculum before designing screens.

**Existing curriculum, open to review**

> Use learning-map with this curriculum. Review its learning goals, structure, gaps, and sequence first. Confirm changes with me before designing the learning experience.

**Locked curriculum**

> Use learning-map and follow this curriculum exactly. Do not change its units or order. Start from canonical content and interaction design.

**Presentation reference**

> Use learning-map to create ___. Source A defines the content. Use B only as a visual and interaction reference, not as a subject-matter source.

### Skill and reference

Full specification: `SKILL.md`

First UI-validated reference implementation:

- Repository: `gcake119/agent-system-design-learning-map`
- Route: `#/deck/token-profiler`

The reference demonstrates a validated interaction rhythm and presentation-first experience. Agents, token profiling, and System Design are not requirements of `learning-map`.
