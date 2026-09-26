# learning-map

## 中文

`learning-map` 是一套製作**以互動式簡報為主、可混搭閱讀文本**的通用學習教材 Skill。

你可以只從一句「我想學 X」開始。它會協助：

```text
學習目的
→ 研究／整理來源
→ 用金字塔原理規劃課綱
→ 確定教材內容
→ 設計互動
→ 實作與驗收
```

不限定技術或 AI，也可以用於科學、人文、語言、專業訓練等主題。

### 快速開始

**從零開始**

> 使用 learning-map 幫我學「___」。我對這個主題沒有概念，請先研究，再跟我用金字塔原理規劃課綱。課綱確認後再進行教材內容與互動設計。

**有自己的教材**

> 使用 learning-map 製作「___」互動教材。以我提供的資料為主要內容來源，可以補充可靠外部資料。先規劃課綱，不要直接開始做畫面。

**已有課綱**

> 使用 learning-map 製作這份課綱。先檢查學習目標、結構、缺漏與順序，和我確認後再進行教材設計。

如果不希望調整課綱，直接說：

> 完全按照這份課綱製作，不要調整章節與順序。

完整工作規則見 [`SKILL.md`](./SKILL.md)。

## 三層架構

`learning-map` 把「怎麼做教材」、「教材本身」和「個人怎麼學」分開：

```text
① learning-map Skill                 Public
   怎麼規劃、製作、維護與調整教材
                 ↓
② Course Repository                 Public
   課綱、教材內容、互動式簡報與練習
                 ↓
③ Personal Learning Progress        Private
   個人學習回饋、Learning Handoff、Learner Path
```

### ① Skill：共用方法

這個 repo 就是第一層。

它定義：

- 如何研究與整理教材來源
- 如何用金字塔原理討論課綱
- Learning Objectives 與 Canonical Content
- 如何依概念選擇互動方式
- Learning Copy、實作與 QA
- 如何記錄 Learning Handoff 並依學習狀況調整路線

Skill 不保存特定課程，也不保存個人學習紀錄。

### ② Course：公開教材

每門課可以有自己的公開 repo，例如：

- [Agent System Design Learning Map](https://github.com/gcake119/agent-system-design-learning-map)
- [Cybersecurity Learning Map](https://github.com/gcake119/cybersecurity-learning-map)

公開教材可以**直接使用**，不需要安裝 `learning-map`。

想做自己的版本時，可以 Fork 教材，再讓 Agent 使用 `learning-map` 修改自己的 fork。

### ③ Progress：私人學習紀錄

個人學習狀況另外保存在私人位置，例如 private repo：

```text
目前學到哪裡
已建立的理解
仍不確定的地方
Learning Evidence
Learner Feedback
Agent Working Interpretation
目前 Learner Path
下一步
```

Learning Handoff 讓新的對話或 Agent 可以快速接續學習，不必把整段歷史重新整理一次。

**不要把私人 Learning Handoff 或個人學習紀錄 commit 到公開教材 fork。**

如果個人學習過程發現的是共通教材問題，可以去除個人資訊後，再用 issue / PR 回饋公開教材。

## 教材內容與互動怎麼決定？

使用者不需要先知道「完整教材應該包含什麼」。

Skill 會依指定來源或可靠研究建立 Subject Model，負責內容正確性、必要完整性與先備知識；使用者主要確認學習方向、範圍、深度與想強調的內容。

教材內容確認後，再判斷每一段最適合用互動、視覺、閱讀、練習或 transfer 呈現。預設以互動式簡報作為主體；當完整解釋、背景、證據、推導、限制或參考資訊用文字更清楚時，可以在同一個 HTML 課程中加入閱讀文本。

例如：

| 學習內容 | 可能的互動 |
| --- | --- |
| 關係／結構 | Interactive Diagram |
| 流程／順序 | Flow Simulator、Timeline |
| 因果／數量 | Variable Explorer、Chart |
| 分類／差異 | Sorting、Comparison |
| 證據／解讀 | Evidence Explorer |
| 決策／取捨 | Scenario、Design Comparison |
| 程序／技能 | Guided Practice |
| 完整解釋／背景／推導 | Focused Reading |
| 證據限制／來源脈絡 | Reading + Evidence Explorer |

目標是讓互動本身幫助理解，也讓閱讀文本承擔它更適合的工作。不要為了維持「互動感」把文章切成大量點擊揭露；也不要把可以操作理解的內容全部退回長文。

一個單元可以混搭：

```text
情境／問題
→ 互動觀察
→ 結果或差異出現
→ 閱讀：解釋機制、背景或限制
→ 回到互動調整另一個條件
→ Transfer
→ 可重用原則
```

所有形式最後都做在同一套 HTML 教材體驗中。

## Fork 後個人化學習

進階使用可以是：

```text
Public Course
     ↓ Fork
My Course Fork
     ↑
learning-map Skill
     ↑
Private Learning Handoff
```

Agent 可以根據實際學習回饋，在自己的 fork 增加案例、改寫說明、補充練習、略過已熟悉內容或調整 Learner Path。

可泛化的改善再去除個人資訊後回饋 upstream；只適合自己的修改留在 fork。

## 開源與貢獻

本專案採 **MIT License**。

歡迎 issue 與 pull request。這個 repo 只收跨主題可重用的方法；單一課程內容應提交到對應 course repo，私人 Learning Handoff 不應提交到公開 repo。

- [貢獻指南](./CONTRIBUTING.md)
- [MIT License](./LICENSE)

---

## English

`learning-map` is a general-purpose skill for creating **presentation-first learning materials that can mix interaction with focused reading**.

Start with a topic:

> Use learning-map to teach me ___. I am new to the subject. Research it first, then plan the curriculum with me using the Pyramid Principle. After I confirm the curriculum, continue with content and interaction design.

The workflow is:

```text
Learning intent
→ Sources / research
→ Pyramid-based curriculum
→ Canonical content
→ Mixed-mode presentation / interaction design
→ Implementation and QA
```

See [`SKILL.md`](./SKILL.md) for the full workflow.

## Three-layer architecture

```text
1. learning-map Skill             Public
   reusable learning-design method
              ↓
2. Course Repository             Public
   curriculum + content + interactive decks
              ↓
3. Personal Learning Progress    Private
   feedback + Learning Handoff + Learner Path
```

**Skill** defines how courses are researched, structured, designed, implemented, and adapted.

**Course repositories** contain reusable public learning material and can be used independently without installing the skill.

**Personal learning progress** stays private. A Learning Handoff records current position, evidence, feedback, provisional Agent interpretations, learner-path changes, and next steps.

Do not commit private Learning Handoffs to a public course fork.

## Personalized learning

For learner-specific adaptation:

```text
Public Course
     ↓ Fork
Your Course Fork
     ↑
learning-map
     ↑
Private Learning Handoff
```

An Agent can use the skill plus your private handoff to adapt your fork with additional examples, revised explanations, extra practice, skipped material, or a different learner path.

Generalizable improvements can be de-identified and contributed upstream; learner-specific changes can remain in the fork.

## Open source

MIT licensed. Issues and pull requests are welcome.

Reusable, topic-agnostic methods belong here. Course-specific content belongs in its course repository. Personal learning records remain private.

- [Contributing Guide](./CONTRIBUTING.md)
- [MIT License](./LICENSE)
