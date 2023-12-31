Cloudflare Block Bad Bot Ruleset

Block bad, possibly even malicious web crawlers (automated bots) using Cloudflare Firewall Rules
使用 Cloudflare Firewall Rules 拦截恶意网络爬虫（自动机器人）和其它恶意流量

Introduction 简介
Cloudflare Block Bad Bot Ruleset projects stop and block Bad Bot, Spam Referrer, Adware, Malware and any other kinds of bad internet traffic ever reaching your web sites. Inspired by nginx-badbot-blocker & worked with Cloudflare Firewall Rules.

Cloudflare Block Bad Bot Ruleset 可以阻止恶意爬虫、垃圾引荐来源、广告、恶意软件以及任何其他类型的恶意互联网流量到达您的网站。灵感来自 nginx-badbot-blocker 并与 Cloudflare Firewall Rules 搭配使用。

Precautions 注意事项
Cloudflare Block Bad Bot Ruleset mainly based on User-Agent, which is known to all that could be changed easily. So the project can not replace the Web Application Firewall.

Cloudflare Block Bad Bot Ruleset 主要基于 User-Agent，但是众所周知 User-Agent 可以伪装，所以本项目并不能取代正规的 Web Application Firewall。

Ruleset 规则
Rule Name	File Name	Action	What For
Good Bot	good-bot.rules	Allow	Match known good bot.
匹配已知的正常爬虫
IDC ASN List	idcasnlist.rules	JS Challenge	Based on known partial IDC ASN number.
基于已知的部分IDC ASN号（包含阿里云盾）
Basic Crawler	basic-crawler.rules	Block/Challenge	Block some known bad bot.
匹配一些基本的 HTTP Request 库
Bad Crawler	bad-crawler.rules	Block/Challenge	Match mostly known bad bot, basic ruleset not included.
匹配绝大部分已知的恶意爬虫
Usage 用法

![360截图20230924202018539](https://github.com/chenxi008/-cloudflare-block-bad-bot-ruleset/assets/117857008/bf442894-1ce1-43f4-b5b4-627793e26e59)

![360截图20230924202340485](https://github.com/chenxi008/-cloudflare-block-bad-bot-ruleset/assets/117857008/dfc06d28-d818-44c1-89ad-4886711bb1e6)

![360截图20230924202405420](https://github.com/chenxi008/-cloudflare-block-bad-bot-ruleset/assets/117857008/ed724e2c-65b8-4ee8-ae2d-39cbf0ce6d8d)

![360截图20230924202451477](https://github.com/chenxi008/-cloudflare-block-bad-bot-ruleset/assets/117857008/f5bff6cd-0978-4726-adc5-2496aee013fe)

![360截图20230924202516860](https://github.com/chenxi008/-cloudflare-block-bad-bot-ruleset/assets/117857008/3fd219ec-7e50-421f-b047-0d60c2600d1a)

![360截图20230924202545869](https://github.com/chenxi008/-cloudflare-block-bad-bot-ruleset/assets/117857008/b9fea33a-2a32-4e26-b0c1-03f884f3eedf)

