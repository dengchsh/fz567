# 仓库怎么设置

GitHub 仓库本身不算个高权重页面，但搜得到搜不到，差别挺大。名字、简介、标签、README 前几行，基本上决定了它能不能被搜到。

---

## 仓库名

能被人搜到，又得像人话。别用纯品牌名，那玩意儿没人搜。

`tiktok-shop-seller-toolkit` —— 关键词最全，搜 tiktok shop 的人容易撞上。推荐这个。

`tiktok-shop-tools` —— 短好记，适合以免费工具为主的仓库。

`tiktok-shop-calculators` —— 只做计算器的话最精准。

`starway-global` —— 纯品牌，适合当组织主页，SEO 基本为零。

建议开两个：一个关键词仓库当主推广，一个品牌仓库攒东西，互相在 README 里链一下。

---

## 简介

GitHub 右边那句话，160 字符左右，超了会截断。重要的放前面。

中文：

```
TikTok Shop 卖家运营后台：多店铺数据、订单发货、AI 素材、选品榜单、GMV Max 投流，含五个免费算账工具。
```

```
免费 TikTok 跨境工具 + 多店铺运营后台。利润、保本 ROAS、ROI、定价计算器与 Hook 生成器免登录可用。
```

英文：

```
TikTok Shop seller ops console: multi-shop dashboards, order fulfillment, AI creative tools, product research and GMV Max ads. Includes 5 free no-login calculators.
```

Website 填 `https://www.fz567.cn`。

---

## 标签

最多 20 个。按「平台词 → 场景词 → 技术词」排，别一股脑堆。

```
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

两点：别塞无关热词，相关性影响排序；中文词组在 Topics 里搜不到，一律写英文。

---

## 徽章

只放真的。假的 build passing 或者下载量，一眼就看出来。

```markdown
![Platform](https://img.shields.io/badge/platform-TikTok%20Shop-black?style=flat-square)
![Free](https://img.shields.io/badge/free%20tools-5-brightgreen?style=flat-square)
![Lang](https://img.shields.io/badge/docs-中文-red?style=flat-square)
```

要放 License 徽章，先真的加个 `LICENSE` 文件（MIT 就行），不然徽章指向一个不存在的东西。

---

## README 里关键词怎么放

原则是「该出现的地方出现，别堆」。堆得多了读起来不像人话，搜索引擎现在也识别得出来。

- 一级标题：品牌 + 品类，比如「星途出海 · TikTok Shop 卖家的运营后台」
- 开头一百字：核心词自然出现一两次就行
- 小标题：用场景词，选品、投流、GMV Max、利润计算
- 工具那一段：每个工具名字 + 一句话用途，长尾词就有落点了
- 结尾：官网、工具页、博客都留入口

别做的事：第一段塞十个关键词；用 HTML 注释藏词；同一段把同一个词重复五遍。

---

## 目录长什么样

```
tiktok-shop-seller-toolkit/
├── README.md
├── LICENSE
├── docs/
│   ├── faq.md
│   └── tools.md
├── .github/
│   └── ISSUE_TEMPLATE/
│       └── feedback.md
└── screenshots/
    ├── dashboard.png
    ├── ai-tools.png
    └── tools.png
```

有 docs、有 LICENSE、有 Issue 模板、有截图的仓库，看起来是有人在维护的。只有一个 README 的空壳，转化率差很多。

---

## 截图

放两三张真的，比十段文字有用。

建议拍：多店铺看板（体现一屏管多店）、免费工具页（体现免登录能直接用，最好带算出来的结果）、AI 工作台（体现素材能批量出）。

注意几点：真实店铺名、订单号、买家信息必须打码；图片放仓库里，别外链官网（外链会失效，GitHub 也不缓存）；单张压到 500KB 以内。

---

## 发版节奏

建完仓就不管，GitHub 基本不给流量。让它看起来还活着：

一周更新一次 README 的工具列表或 FAQ，顺手发个 Release 说明。两周左右往 docs 里加一篇使用指南，README 里挂个链接。一个月整理一次「这次加了什么、修了什么」的 Discussion。有人提 Issue 就回，哪怕是「暂时不支持」也要回一句。

Release 不用真有什么版本号，用日期也行，`2026.11` 这样。
