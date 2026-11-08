# NeatFeed

**把你关注的站点，攒成一个能翻、能搜、能信、能带走的资料库。**

*A local library for creators: crawls the sites you follow, extracts the articles, and gives you a table you can search, filter and export.*

> 🚧 **Status: skeleton stage.** Nothing here is installable yet. The design is settled; code starts at M0.
> Design → [`docs/SPEC.md`](docs/SPEC.md)

## Why

信息散在几十个标签页、微信收藏和笔记软件里，真正要写东西的时候，找不回来。

NeatFeed 的做法很朴素：**先把信息攒进自己的库，再谈怎么用。**

- **持续采集** — RSS / 静态网页 / 你已登录的浏览器（通过 CDP，凭据不进插件）
- **一个库** — 表格可翻、全文可搜、按来源 / 时间 / 互动量收窄
- **能带走** — 选中素材，导出 Markdown（带出处）/ CSV / JSON

## Roadmap

| Version | What |
|---|---|
| v0.1 | 采集 + 可读的库（翻 / 找 / 信 / 带走） |
| v0.2 | 库内问答：基于你自己的库成文，每条论断带出处；缺料时明说"库里没有" |
| v0.3 | 每日选题流：规则粗筛 + 模型精排（"今天值得写什么"） |
| later | Word 简报、小红书、多库、对标账号监控 |

## Three non-negotiables

1. **可读优先于可采** — "采进去了但看不见"不算完成。
2. **每一条都可回溯** — 来源、原始 URL、抓取时间。
3. **凭据不进插件** — 不读 cookie 库 / Keychain；登录态只存在于浏览器 profile 内部，插件通过 CDP 发指令。

## Requirements

DeepSeek Harness 0.2.1+ (plugin manifest `dsh.bundle`), plus Chrome or Edge on macOS / Windows.

## License

MIT
