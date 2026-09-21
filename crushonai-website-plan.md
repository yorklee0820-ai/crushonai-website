# crushonai.website — 站点规划文档

> 目标域名：crushonai.website
> 主关键词：**crushon ai**
> 形态：纯静态站点（HTML + CSS，零后端、零 JS 渲染依赖）
> 语言：英文
> 文档版本：v1（规划阶段，未开工）

---

## 0. 一句话定位

crushonai.website 是 CrushOn AI 的**独立内容站**：以「crushon ai」品牌词为核心，用「评测 + 指南 + 对比 + 角色库」四类内容承接搜索意图，把 landing page 做成转化终点。

---

## 1. 关键词策略

### 1.1 关键词矩阵

| 层级 | 关键词 | 搜索意图 | 承载页面 |
|---|---|---|---|
| **主词** | crushon ai / crushon.ai / crushon ai chat | 品牌导航 | `/`（H1/Title/首段） |
| **品牌长尾** | crushon ai review | 评测对比 | `/review` |
| | crushon ai pricing / crushon ai cost | 商业调研 | `/pricing` |
| | is crushon ai free / crushon ai free tier | 疑虑确认 | `/pricing` + FAQ |
| | crushon ai login / crushon ai sign up | 导航 | `/`（多 CTA） |
| | crushon ai apk / crushon ai app | 下载 | `/review` 章节 + `/blog/crushon-ai-app-apk` |
| | crushon ai not working / crushon ai down | 故障 | `/blog/crushon-ai-not-working` |
| **对比词** | crushon ai vs character ai | 对比 | `/vs-character-ai` |
| | crushon ai vs janitor ai | 对比 | `/vs-janitor-ai` |
| | crushon ai alternatives | 对比 | `/alternatives` |
| | crushon ai vs candy ai / vs nomi ai | 对比 | `/alternatives` 章节 |
| **品类词** | unfiltered ai chat | 品类 | `/` + `/review` |
| | ai character chat / ai roleplay chat | 品类 | `/` + `/characters` |
| | nsfw ai chat / nsfw character ai | 品类 | `/characters` |
| | ai girlfriend chat / ai companion chat | 品类 | `/characters` 分类页 |
| **角色长尾** | best crushon ai characters | 资源 | `/characters` + blog cluster C |
| **使用长尾** | how to create a character on crushon ai | 教程 | `/blog/how-to-create-character-crushon-ai` |
| | crushon ai memory / crushon ai models | 功能 | `/blog/crushon-ai-models-explained` |

### 1.2 关键词密度与分布原则

- 主词 "crushon ai"：首页自然出现 15–25 次（含 title / H1 / 首 100 词 / 尾段 / 图片 alt / 内链锚文本）
- **禁止堆砌**：H2/H3 中主词出现不超过 6 次，其余用代词（the platform / it）和品类词替代
- 锚文本配比：exact match ≤ 30%，其余为品牌+修饰（"CrushOn AI pricing"、"read our CrushOn AI review"）、品类词、裸 URL

### 1.3 搜索量数据

本文档**不填搜索量数字**——需你在 Ahrefs / Semrush / GSC 中拉真实数据后回填，避免用估算值做优先级排序。回填字段建议：`volume / KD / SERP 特征（是否有 featured snippet、是否有 PAA）`。

---

## 2. 站点架构

### 2.1 页面清单（共 20 页：12 核心页 + 8 支撑页）

#### A. 核心页（SEO 主力）

| # | URL | 页面 | 目标词 | 目标字数 |
|---|---|---|---|---|
| 1 | `/` | Landing Page（长内容） | crushon ai | 3,500–5,000 |
| 2 | `/review` | CrushOn AI Review 2026 | crushon ai review | 2,500–3,000 |
| 3 | `/pricing` | Pricing & Plans | crushon ai pricing | 1,500–2,000 |
| 4 | `/characters` | Character Library Guide | ai character chat / best crushon ai characters | 2,000–2,500 |
| 5 | `/alternatives` | 7 Best Alternatives | crushon ai alternatives | 2,000–2,500 |
| 6 | `/vs-character-ai` | vs Character.AI | crushon ai vs character ai | 1,800–2,200 |
| 7 | `/vs-janitor-ai` | vs Janitor AI | crushon ai vs janitor ai | 1,800–2,200 |
| 8 | `/blog` | Blog 索引（按 cluster 分组） | crushon ai guides | 600–800 |

#### B. 支撑页（信任 + 收录 + 长尾兜底）

| # | URL | 用途 |
|---|---|---|
| 9 | `/about` | E-E-A-T：编辑标准、评测方法、作者署名 |
| 10 | `/privacy` | 隐私政策（必须，广告/联盟与 GSC 信任信号） |
| 11 | `/terms` | 使用条款 |
| 12 | `/18-plus` | 成人内容声明 + 年龄政策（合规与信任） |
| 13 | `/contact` | 联系页 |
| 14 | `/editorial-policy` | 评测方法论（E-E-A-T，AI 站点尤其重要） |
| 15 | `/sitemap.html` | 人类可读站点地图，内链枢纽 |
| 16 | `/404.html` | 404 页（含搜索框 + 热门页内链） |

> 每篇 blog 完成后追加到清单（见第 4 节，共 12 篇）。

### 2.2 URL 规范

- 全小写、连字符分词、无参数、无日期
- 目录结尾统一带 `/`（静态站需目录 + `index.html`）
- 博客 slug：`/blog/<primary-keyword-slug>/`，例：`/blog/how-to-create-character-crushon-ai/`
- canonical 全部自引用

---

## 3. Landing Page（`/`）详细内容大纲

> 结构顺序即为 SEO 权重顺序：主词信号集中在首屏与前三屏。

### Section 1 — Hero
- **H1**：`CrushOn AI: Unfiltered AI Character Chat & Roleplay`（主词开头）
- 副标题：2 个品类词（unfiltered / ai character chat）+ 一句话价值主张
- 双 CTA：`Start Chatting Free` / `Read the 2026 Review`
- 18+ badge
- 内容量：60–80 词

### Section 2 — Trust Bar
- 数据条（**数值待你确认，见第 7 节**）：8M+ characters / 13+ AI models / up to 24K memory / cross-device sync
- 每个数字下方一行小字说明

### Section 3 — What is CrushOn AI?（SEO 语义核心）
- **H2**：`What Is CrushOn AI?`
- 400 词定义段：平台是什么、面向谁、与主流 chatbot 的差异、免费与付费边界
- 主词在首句与末句各出现一次
- 目标：抢 featured snippet（段落式答案）

### Section 4 — Key Features（8 张卡）
- **H2**：`CrushOn AI Features`
- 每卡 100 词，H3 用小标题（含长尾）：
  1. Unfiltered AI Chat（无内容过滤）
  2. Long-Term Memory（24K context）
  3. 13+ AI Models（可中途切换）
  4. Custom Character Creator
  5. Multi-Character Group Chat（3–4 角色同场）
  6. AI Voice（40+ 预设 / 9 语言）
  7. Cross-Device Sync（Web / Android）
  8. NSFW Toggle（用户自控开关）

### Section 5 — AI Models Table
- **H2**：`CrushOn AI Models Compared`
- 13 行表格：模型名 / 定位 / 适用档位（数据取自官网 2026 列表）
  - Claude Opus 4.7、GPT 5.2、Gemini 3.1 Pro、DeepSeek R1、GLM 5.1、Claude Sonnet 4.6、Claude Opus 4.6、GLM 5、DeepSeek V4 Flash、Crushon Mochi V3、Crushon Mira、GLM 4.6、Crushon Leo
- 表格 → 高概率抢表格式 snippet

### Section 6 — Character Categories（12–16 格）
- **H2**：`Browse AI Characters by Category`
- 每格：分类名 + 一句话 + 锚文本链接到 `/characters`
- 分类示例：AI Girlfriend / AI Boyfriend / Anime / Fantasy / Sci-Fi / Original OC / Villain / Mentor / Slice of Life / Horror

### Section 7 — How It Works（3 步）
- **H2**：`How to Start a CrushOn AI Chat`
- HowTo schema
- Step 1 Sign up free → Step 2 Pick a character → Step 3 Start chatting

### Section 8 — Comparison Table
- **H2**：`CrushOn AI vs Character.AI vs Janitor.AI`
- 表格维度：过滤政策 / 模型数量 / 记忆长度 / 群聊 / 语音 / 免费额度 / 起价
- 底部内链到 `/vs-character-ai`、`/vs-janitor-ai`

### Section 9 — Pricing
- **H2**：`CrushOn AI Pricing`
- Free / Standard / Premium / Luxe 四档卡片
- **价格留空待确认**（第 7 节）
- 底部 CTA → `/pricing`

### Section 10 — What's New in 2026
- 24K long-term memory / group chat / mid-chat model switching / 40+ voices / annual save up to 47%
- 作用：内容新鲜度信号（freshness）

### Section 11 — Who It's For
- 4 类人群卡：NSFW roleplayers / 自定义角色创作者 / 多模型尝鲜用户 / 预算敏感用户
- 同时写明「谁不适合」（增强可信度，降低跳出）

### Section 12 — Privacy & Safety
- 加密、不用于训练、匿名使用建议
- 内链到 `/privacy`、`/18-plus`

### Section 13 — What Reviewers Say
- 引用第三方评分（**需标来源 + 日期**），配 3 条引述
- 内链到 `/review`

### Section 14 — FAQ（12–15 问）
- **H2**：`CrushOn AI FAQ`
- FAQPage schema
- 选题：Is it free? / Is it safe? / Can I create characters? / NSFW allowed? / Character limit? / Does it have an app? / Memory length? / Which model is best? / Group chat? / Voice? / Refund? / Language support? / Delete account? / APK safe? / vs Character.AI?

### Section 15 — From the Blog
- 6 篇精选卡片，cluster 各取一篇（内链分发权重）

### Section 16 — Final CTA + Footer
- 重复主 CTA
- Footer：核心页全量内链 + `/sitemap.html` + 18+ 声明

### 顶部 TOC（额外）
- 锚点目录 14 项 → 提升长页可爬取性与 sitelinks 概率

---

## 4. 博客内容规划（12 篇，4 个 Cluster）

### Cluster A — 使用指南（How-to）

| # | Slug | 目标词 | 字数 | H2 骨架 |
|---|---|---|---|---|
| A1 | `/blog/how-to-create-character-crushon-ai` | how to create a character on crushon ai | 1,600 | 准备 → 字段填写 → 示例对话 → 发布/私有 → 常见错误 |
| A2 | `/blog/crushon-ai-models-explained` | crushon ai models | 1,800 | 三档模型 → 逐模型定位 → 怎么选 → 切换技巧 |
| A3 | `/blog/crushon-ai-memory-how-it-works` | crushon ai memory | 1,400 | 上下文窗口 → 各档位差异 → 提升记忆的 5 个做法 |

### Cluster B — 对比评测（Commercial）

| # | Slug | 目标词 | 字数 |
|---|---|---|---|
| B1 | `/blog/crushon-ai-vs-candy-ai` | crushon ai vs candy ai | 1,600 |
| B2 | `/blog/crushon-ai-vs-nomi-ai` | crushon ai vs nomi ai | 1,500 |
| B3 | `/blog/best-unfiltered-ai-chat-platforms` | unfiltered ai chat | 2,200 |

### Cluster C — 角色库（Resource，流量型）

| # | Slug | 目标词 | 字数 |
|---|---|---|---|
| C1 | `/blog/best-crushon-ai-characters` | best crushon ai characters | 2,000 |
| C2 | `/blog/crushon-ai-anime-characters` | crushon ai anime characters | 1,600 |
| C3 | `/blog/crushon-ai-nsfw-characters-guide` | nsfw ai chat characters | 1,800 |

### Cluster D — 故障与账号（Support，低竞争高转化）

| # | Slug | 目标词 | 字数 |
|---|---|---|---|
| D1 | `/blog/crushon-ai-not-working` | crushon ai not working | 1,200 |
| D2 | `/blog/crushon-ai-app-apk` | crushon ai apk | 1,400 |
| D3 | `/blog/is-crushon-ai-safe` | is crushon ai safe | 1,500 |

### 每篇统一模板
1. 直接答案段（前 60 词，抢 snippet）
2. H2 主体（含 1 个表格 / 1 个列表）
3. 内链块：→ `/`（主词锚文本）→ `/pricing` 或 `/review` → 同 cluster 1–2 篇
4. 作者署名 + 更新日期（E-E-A-T）

---

## 5. 内链策略（Hub-and-Spoke）

```
                    /  (Hub - 主词)
                     |
   +---------+---------+---------+
 /review   /pricing  /characters /alternatives
   |          |          |            |
   +---- /vs-character-ai, /vs-janitor-ai ---+
                     |
                  /blog
          (A/B/C/D 四个 cluster 内部互链)
```

**规则**
- 每个 spoke 页**必须**有一条锚文本含 "crushon ai" 的链接回首页
- 对比页与 `/alternatives`、`/review` 三向互链
- 同 cluster 博客互链 1–2 条，跨 cluster 至少 1 条
- `/sitemap.html` 全站可达，Footer 每页都放
- **外链**：评测页引用 2–3 个权威源（官网 + 第三方评测），`rel="nofollow"` 处理联盟链接

---

## 6. 技术 SEO 清单

### 6.1 每页必配（模板）

| 元素 | 规格 |
|---|---|
| `<title>` | ≤ 60 字符，主词靠前。首页：`CrushOn AI: Unfiltered AI Character Chat (2026)` |
| `<meta description>` | ≤ 155 字符，含主词 + CTA |
| `<h1>` | 全页唯一，含主词（首页）/ 含目标词（子页） |
| `<link rel=canonical>` | 自引用绝对 URL |
| OG / Twitter Card | og:title / og:description / og:image / og:type |
| 图片 | WebP、`alt` 含上下文关键词、非首屏 `loading="lazy"`、显式 width/height |
| 语言 | `<html lang="en">` |

### 6.2 结构化数据（JSON-LD）

| 页面 | Schema 类型 |
|---|---|
| `/` | `SoftwareApplication` + `FAQPage` + `HowTo` + `BreadcrumbList` + `Organization` |
| `/review` | `Review` / `ItemList` + `BreadcrumbList` |
| `/pricing` | `Product` / `Offer` + `FAQPage` |
| `/vs-*` | `ItemList` + `FAQPage` |
| 所有 blog | `Article`（含 author、datePublished、dateModified） |
| 全站 | `WebSite`（`SearchAction` 可选） |

### 6.3 站点级

- `sitemap.xml`（全部 URL + lastmod）+ `robots.txt`（显式指向 sitemap）
- **纯静态**：HTML/CSS 直出，正文不依赖 JS 渲染；Critical CSS 内联
- Core Web Vitals 目标：LCP < 2.0s、CLS < 0.05、INP < 150ms
- 字体：`font-display: swap` + 自托管子集
- 18+ 处理：`meta name="rating" content="adult"`，**不做 JS 年龄门拦截爬虫**（会阻断索引）
- 图片素材：不出现裸露内容，用抽象/插画视觉
- 部署后：GSC + Bing WMT 提交 sitemap，验证索引覆盖率

### 6.4 内容新鲜度

- 每页底部显示 `Last updated` 日期
- 每季度复查：价格、模型列表、功能（该品类迭代极快，过期数据直接掉排名）

---

## 7. 数据待你确认清单（我不填编造值）

| 字段 | 现状 | 需要你提供 |
|---|---|---|
| 定价 | 多源冲突（$4.99 / $5.99 / $14.99 等） | 官方当前 Free / Standard / Premium / Luxe 各档月付与年付真实价 |
| 模型数量与名称 | 官网显示 13+ | 是否以官网为准、是否还需列已下线模型 |
| 角色库规模 | 官网称 8M+ | 确认是否沿用 |
| 记忆长度 | Ultra 24K / Standard 16K / Free 8K | 确认 |
| 免费额度 | 免费模型不限量，Pro 模型 100 credits/月 | 确认 |
| 移动端 | Android APK 有；iOS 各源说法不一 | 确认是否有 iOS |
| 第三方评分引用 | 7.6/10、4.1/5、4.3/5 等 | 确认是否引用 + 引用哪几家 + 是否标注日期 |
| 联盟/外链关系 | 未知 | 是否带 aff 参数（决定 nofollow 策略） |

---

## 8. 执行排期（建议 4 批）

| 批次 | 内容 | 说明 |
|---|---|---|
| P1 | `/` landing + `/privacy` + `/terms` + `/18-plus` + `sitemap.xml` + `robots.txt` | 先上线主词阵地，可立即提交索引 |
| P2 | `/review` + `/pricing` + `/characters` | 商业意图页，转化主力 |
| P3 | `/alternatives` + `/vs-character-ai` + `/vs-janitor-ai` + `/blog` 索引 | 对比词覆盖 |
| P4 | Cluster A–D 共 12 篇 | 长尾流量池，分批发布（每周 2–3 篇） |

---

## 9. 验收标准

- [ ] 全站 20 个 URL 无死链、无重复 title/description
- [ ] 每个 JSON-LD 通过 Rich Results Test
- [ ] 首页 Lighthouse SEO 100 / Performance ≥ 95
- [ ] 主词 "crushon ai" 首页自然出现 15–25 次，无堆砌
- [ ] 每页至少 3 条指向其他页的内链
- [ ] GSC 提交后 2 周内复查索引覆盖率
