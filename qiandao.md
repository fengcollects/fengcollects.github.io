# 签到脚本折腾记

我的签到脚本是 Fork 别人的，仓库叫 feng，每天早上 8 点自动帮我给机场签到，白嫖流量。

最折腾的是通知。第一个 Telegram 机器人怎么配都不推送，干脆删了重来：找 @BotFather 新建 @feng_qi_bot，给它发个 /start，再找 @userinfobot 要到 chat_id，把 TG_TOKEN 和 TG_ID 塞进仓库的 Secrets 里——当晚推送就来了，通了！

还有个坑：GitHub 的定时任务经常迟到几小时，有天早上的运行干脆就没出现。学乖了：每天手动点一下触发，最稳。

现在每天醒来，签到结果准时躺在 Telegram 里，爽。
