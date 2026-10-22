# 使用示例

[接入指南](agent.md) · [返回 README](../README.md)

匿名范围为原发最近7天 News 短摘要及少量论文标题/链接。下面先给一次线上返回节选，再列常用调用形态。

## 想试什么

取一条近期 News 简报。样本读取时间：2026-10-11T18:06:56.013Z。

### 怎么用

```json
{"name":"aisafetyhot_get_latest","arguments":{"window":"7d","mode":"selected","limit":1}}
```

### 结果

以下是该次返回的一条新闻及相关范围字段节选，省略 `page.nextCursor`、其他元数据和 5 条论文链接；未改写返回文本。

```json
{
  "items": [
    {
      "id": "viya4o8jw5jrry0ft85l2wgqt",
      "title": "open-multi-agent 的 file_write 工具存在悬空符号链接漏洞，可向工作区外写文件",
      "summary": "NVD 登记 CVE-2026-108600：@open-multi-agent/core 1.5.0 至 1.21.2 的 file_write 工具沙箱会跟随符号链接，攻击者在工作区放置悬空符号链接并引导 agent 写入，即可在工作区根目录之外创建文件。该缺陷属于多 agent 框架工具沙箱的路径安全校验问题。",
      "publishedAt": null,
      "publishedDate": "2026-10-10",
      "links": {
        "aihot": "https://aisafetyhot.com/items/viya4o8jw5jrry0ft85l2wgqt",
        "original": "https://nvd.nist.gov/vuln/detail/CVE-2026-108600"
      }
    }
  ],
  "page": {
    "count": 1,
    "hasMore": true
  },
  "access": {
    "scope": "recent_news_and_paper_links",
    "newsWindowDays": 7,
    "summaryMaxChars": 160,
    "paperPickLimit": 5,
    "fullReadingRequiresAuthorization": true
  }
}
```

`page.hasMore=true` 时，将同次返回的 `page.nextCursor` 原样填入下一次调用的 `arguments.cursor`，保持其他参数不变。例如，继续上面 `limit=1` 的调用：

```json
{"name":"aisafetyhot_get_latest","arguments":{"window":"7d","mode":"selected","limit":1,"cursor":"替换为上次返回的 page.nextCursor"}}
```

`cursor` 的值是占位说明，调用前须替换为实际返回的游标；不要把字段名 `nextCursor` 当作请求参数。每次继续翻页都使用上一页返回的新游标，直到 `page.hasMore=false`；不能只因返回条数少于 `limit` 就判断已经读完。

`publishedAt=null`、`publishedDate=2026-10-10` 表示原文只精确到日，不补造时刻。

## 最新与搜索

```json
{"name":"aisafetyhot_get_latest","arguments":{"window":"7d","mode":"selected","limit":10}}
```

```json
{"name":"aisafetyhot_search","arguments":{"q":"prompt injection","window":"7d","mode":"selected","limit":10}}
```

同一筛选沿返回的 `page.nextCursor` 翻页，直到 `page.hasMore=false`。`paperPicks` 只提供标题与链接。

## 单条与事件

```json
{"name":"aisafetyhot_get_content","arguments":{"id":"返回的id","depth":"summary"}}
```

```json
{"name":"aisafetyhot_get_story","arguments":{"public_id":"返回的publicId","depth":"summary"}}
```

## 日报

```json
{"name":"aisafetyhot_get_daily","arguments":{"period":"daily","mode":"list","limit":7}}
```

```json
{"name":"aisafetyhot_get_daily","arguments":{"period":"daily","mode":"read"}}
```

完整阅读在网站进行。历史、`window=all`、`depth=full`、周/月报与精选快照/增量需要只读授权；联系 wuy7117@gmail.com。授权后使用相同工具及既有协议，并携带 `Authorization: Bearer <token>`。
