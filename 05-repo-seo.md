# 仓库 SEO 与元信息

GitHub 仓库本身是一个高权重页面。仓库名、About、Topics、README 前 3 行，共同决定它在 GitHub 站内搜索和 Google 的可见度。

---

## 一、仓库名候选

名字要能被人搜到，也要像人话。优先「关键词 + 用途」，不要用纯品牌名。

| 候选 | 说明 |
|---|---|
| `tiktok-shop-seller-toolkit` | 关键词最全，搜 `tiktok shop` 的人容易命中，推荐 |
| `tiktok-shop-tools` | 短、好记，适合以免费工具为主的仓库 |
| `tiktok-shop-calculators` | 只做计算器时最精准 |
| `starway-global` | 纯品牌名，适合作为组织/品牌主页仓库，SEO 弱 |
| `cross-border-ecommerce-tools` | 泛关键词，能吃到跨境流量但不精准 |

建议：**一个关键词仓库（主推广）+ 一个品牌仓库（品牌沉淀）**，互相在 README 里链接。

---

## 二、About 描述（GitHub 右侧那句话）

限制约 160 字符，超了会被截断。把最重要的信息放前半句。

**中文版（推荐）**

```text
TikTok Shop 卖家运营后台：多店铺数据、订单履约、AI 素材、选品榜单、GMV Max 投流，含 5 个免登录免费算账工具。
```

**备选**

```text
免费 TikTok 跨境工具 + 多店铺运营后台。利润、保本 ROAS、ROI、定价计算器与 Hook 生成器，免登录可用。
```

**英文版**（如果要面向海外用户）

```text
TikTok Shop seller ops console: multi-shop dashboards, order fulfillment, AI creative tools, product research and GMV Max ads. Includes 5 free no-login calculators.
```

**Website 字段**：填 `https://www.fz567.cn`

---

## 三、Topics（最多 20 个）

Topics 是 GitHub 站内检索的主要入口。按「平台词 → 场景词 → 技术词」排序。

```text
tiktok-shop
tiktok-shop-api
ecommerce
cross-border-ecommerce
dropshipping
seller-tools
profit-calculator
roas-calculator
roi-calculator
pricing-calculator
ai-video
ai-content-generation
product-research
shop-management
order-management
ads-management
gm-max
1688
temu
nextjs
```

注意事项：

- 一次不要堆 20 个不相关的词，Topics 的相关性会影响排序
- 不要用 `tiktok` 单独一个词硬蹭，容易被判定为无关
- 中文词组在 GitHub Topics 里搜不到，一律用英文

---

## 四、徽章（shields.io）

只放**真实**的徽章。放虚假的 build passing / 下载量会被指出来。

```markdown
![Platform](https://img.shields.io/badge/platform-TikTok%20Shop-000000?style=flat-square)
![Free tools](https://img.shields.io/badge/free%20tools-5%20no%20login-brightgreen?style=flat-square)
![Official API](https://img.shields.io/badge/data-official%20API-lightgrey?style=flat-square)
![Lang](https://img.shields.io/badge/lang-中文-red?style=flat-square)
![Updated](https://img.shields.io/badge/updated-2026--11-blue?style=flat-square)
```

如果要放 License 徽章，**先在仓库里真的加一个 `LICENSE` 文件**（MIT 或 Apache-2.0），否则徽章指向一个不存在的文件。

---

## 五、README 关键词布局

GitHub 的 README 会被搜索引擎索引。布局原则：**关键词出现在该出现的地方，不要堆。**

| 位置 | 放什么 | 说明 |
|---|---|---|
| 一级标题 | 品牌 + 品类 | `星途出海 · TikTok Shop 卖家运营工具箱` |
| 首段 100 字 | 核心关键词自然出现 1–2 次 | `TikTok Shop`、`多店铺`、`跨境卖家` |
| 各二级标题 | 场景关键词 | 选品、投流、GMV Max、利润计算 |
| 工具表格 | 每个工具的名称 + 一句话用途 | 让「利润计算器」这类长尾词有落点 |
| 结尾链接区 | 官网 / 工具页 / 博客 | 保证每个页面都有入口 |

**要避免的：**

- 首段塞 10 个关键词，读起来不像人话
- 用 HTML 注释藏关键词，GitHub 会渲染但搜索引擎降权
- 同一段重复出现同一个词 5 次以上

---

## 六、文件与目录建议

```text
tiktok-shop-seller-toolkit/
├── README.md              # 用 01-main-readme.md
├── LICENSE                # MIT 或 Apache-2.0
├── docs/
│   ├── faq.md             # 用 04-faq.md 的一部分
│   └── tools.md           # 五个免费工具的详细用法
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── feedback.md    # 用 03-snippets.md 里的 Issue 模板
│   └── workflows/
└── screenshots/
    ├── dashboard.png
    ├── ai-tools.png
    └── tools.png
```

有 `docs/`、`LICENSE`、Issue 模板、截图的仓库，看起来是认真维护的，转化率明显高于只有一个 README 的空壳。

---

## 七、截图清单（需要你补充真图）

README 里放 2–3 张真实截图，比十段文字有效。建议：

1. **多店铺看板** —— 体现「一屏管多店」，注意打码店铺名与真实 GMV
2. **免费工具页** —— 体现「免登录就能用」，最好带计算结果
3. **AI 工作台** —— 体现素材生产能力

注意：

- 截图里的真实店铺名、订单号、买家信息必须打码
- 图片放仓库内 `screenshots/`，不要外链到官网（外链会失效，也不被 GitHub 缓存）
- 单张控制在 500KB 内，用 PNG 或 WebP

---

## 八、发布节奏建议

GitHub 对「一次性建仓然后不管」的仓库几乎不给流量。保持活跃的做法：

| 频率 | 动作 |
|---|---|
| 每周 | 更新 README 里的工具列表或 FAQ；发一条 Release 说明 |
| 每两周 | 新增一篇 `docs/` 下的使用指南，并在 README 加链接 |
| 每月 | 整理一次「本期新增工具 / 修复问题」的 Discussion |
| 按需 | 回复 Issue，即使是「暂不支持」也要回 |

Release 不需要真有版本号，用日期标签即可（如 `2026.11`）。
