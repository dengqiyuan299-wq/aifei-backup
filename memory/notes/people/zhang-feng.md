---
display_name: "张凤"
first_name: "凤"
last_name: "张"
summary: "WeChat contact who gets the user's daily morning tea poster; OpenClaw WeChat was disconnected on 2026-11-02, so the 企业微信 route (in the user's hands) is now pending."
rank: 5
updated: "2026-11-02"
---

# 张凤

## Facts
- 张凤 is a contact on the user's WeChat. The user has not named the relationship, so it stays unnamed. The user's own words on 2026-10-20 ~14:30 CST: "那你现在接管了微信以后，你能把每天你生成的图片发给他，让他再发给我那个微信的张凤。" (window 2026-10-20T06:30:43+00:00, message:3a930a30-7c87-4480-ac0b-adb23407959a)
- The user first asked on 2026-10-20 (~01:17 CST) for the daily morning tea poster to be sent directly to 张凤 via WeChat every day — the first time 张凤 appears in the record. (window 2026-10-19T17:17:55+00:00, message:78345b9c-71eb-45ec-9e18-9e8c623017c7)
- The delivery automation is built but not yet live: cron `daily-poster-to-zhangfeng` runs daily ~08:53 Asia/Shanghai, finds that day's poster, SCPs it to the VPS, and sends it via the OpenClaw WeChat channel; reports go to the 工作 side chat. It is BLOCKED on her receiving identity — `~/workspace/goals/goal/hidden_files/zhangfeng-wechat.conf` still holds an empty placeholder. (memory://md:MEMORY.md)
- The OpenClaw WeChat bot (ilink `openclaw-weixin`) is passive-only: no contacts list, no name search, `sendmessage` needs the explicit `xxx@im.wechat` ID. Capturing her ID by having her message the bot was tried twice on 2026-10-20 and failed; sharing the ClawBot with her is impossible — it is a plugin, not a shareable contact. (memory://md:memory/2026-10-20.md:26–29)
- The user rejected any semi-auto fallback on 2026-10-20 (~01:42 CST): "肯定是你完全接管呀！否则我要你干嘛呢？你这转来转去的。" — full automation is the stated expectation. (memory://md:memory/2026-10-20.md:33)
- The WeChat account swap completed on 2026-10-20 ~14:35 CST: new account `85ccf63fb5c1-im-bot` verified working bidirectionally (test message delivered ~14:29 CST), old account `c4f7f5f8dc01-im-bot` fully removed. The user's own `to_user_id` is known/working. (memory://md:MEMORY.md; window 2026-10-20T06:29:13+00:00, message:assistant-msg-271c5bd8-6031-4757-ad74-c7fc32cb61f6)
- On 2026-10-20 (~17:44–17:49 CST) the user asked for alternatives beyond the passive bot; the assistant proposed 企业微信 (VPS plugin ready, full address book, truly automatic), PC-WeChat automation (grey-area), and a service account (license + yearly fee), recommended 企业微信, and the user asked how to set it up. (window 2026-10-20T09:47:42.313+00:00, message:fee04bda-1d2b-4c9c-812e-2f01795b9fd5)
- The 企业微信 plan (2026-10-20 ~17:49 CST): Step 1 (user, ~10 min) — app login, enterprise with company license photo + face verification. Step 2 (user) — self-built app, record 企业ID / AgentId / Secret, add VPS IP `81.70.12.165` as trusted IP. Step 3 (assistant) — VPS configuration via secure credential entry. Step 4 — 张凤 added as a *member* for full automation (plugin authorization in her WeChat, no separate app); as a mere external contact, each send needs the user to tap confirm. Awaiting Step 1. (window 2026-10-20T09:49:40.989+00:00, message:assistant-msg-4a2c14ed-aab3-412d-ad19-e8fb2e4fcb3e)
- On 2026-11-02 (evening, window message:e18059e1-9d27-4a87-9d86-a6f1969a5a07) the user ordered the OpenClaw WeChat connection disconnected, verified the same evening: channel entry deleted, login data sealed, gateway restarted, new logs showed no WeChat start or polling and no data directory rebuilt. The ClawBot no longer sends or receives. That route to 张凤 is therefore closed unless the user later rescans to reconnect; the 企业微信 route remains pending.

## History
- 2026-10-20 ~01:11 CST: the user enabled OpenClaw's WeChat channel and scanned the QR code with their personal WeChat. (memory://md:MEMORY.md)
- 2026-10-20 ~01:17 CST: the user asked for the daily morning tea poster to be auto-sent to 张凤 every day — her first appearance in the record. (window 2026-10-19T17:17:55+00:00, message:78345b9c-71eb-45ec-9e18-9e8c623017c7)
- 2026-10-20 ~01:30–01:42 CST: the passive-only bot could not look her up by name; sharing the ClawBot turned out impossible. Delivery automation was built with a placeholder for her ID; the user rejected the semi-auto fallback. (memory://md:memory/2026-10-20.md:25–40)
- 2026-10-20 ~12:57–14:35 CST: the user swapped the OpenClaw-bound WeChat account to a new one — completed, verified bidirectional, old binding fully removed. (memory://md:MEMORY.md)
- 2026-10-20 ~14:30–14:35 CST: the user reconfirmed the request after the swap — the poster must go to 张凤 — and reported the ClawBot cannot be shared; two ilink-based routes were proposed. (window 2026-10-20T06:30:43+00:00, message:3a930a30-7c87-4480-ac0b-adb23407959a)
- 2026-10-20 ~17:44–17:49 CST: the user asked for alternatives beyond the passive bot; the assistant proposed 企业微信 / PC automation / service account, recommended 企业微信, the user chose it, and the four-step setup was laid out. Awaiting the user's Step 1. (window 2026-10-20T09:47:42.313+00:00, message:fee04bda-1d2b-4c9c-812e-2f01795b9fd5)
- 2026-11-02 (evening): the user ordered the OpenClaw WeChat connection disconnected (window message:e18059e1-9d27-4a87-9d86-a6f1969a5a07); disconnection was completed and verified the same evening — channel deleted, login data sealed, gateway restarted clean, no WeChat start or polling in new logs.

## The relationship
- The user has not named the relationship, so it stays unnamed. What the evidence shows: 张凤 is a WeChat contact the user wants to reach every morning with the daily 初羽茶盧 poster — important enough for a dedicated daily automation, the user pushed hard against any half-measure ("肯定是你完全接管呀"), reconfirmed the request after the WeChat swap, and when the passive bot blocked full automation settled on the 企业微信 route.
- Nothing else is known yet: how they met, what ties them, how often they talk. The contact so far is entirely through the user's intent to send her the poster.

## In common
- The 初羽茶盧 daily tea poster: the user wants 张凤 to receive it every morning. Nothing more is evidenced.

## Open threads
- [x] 2026-10-20: the OpenClaw-bound WeChat account swap — completed ~14:35 CST; new account verified bidirectional, old account fully removed. (memory://md:MEMORY.md)
- [x] 2026-10-20: route decision between the two ilink-based routes — closed; the user asked for alternatives and chose 企业微信. (window 2026-10-20T09:47:42.313+00:00, message:fee04bda-1d2b-4c9c-812e-2f01795b9fd5)
- [ ] 2026-10-20: 企业微信 SETUP — the user is to complete Step 1 (register the enterprise in the app with the company license) and Step 2 (create the self-built app, record 企业ID/AgentId/Secret, add VPS IP 81.70.12.165 as trusted IP), then tell the assistant, which configures the VPS and walks the 张凤-as-member setup so the daily poster goes to her automatically. (window 2026-10-20T09:49:40.989+00:00, message:assistant-msg-4a2c14ed-aab3-412d-ad19-e8fb2e4fcb3e)
- [ ] Conditional on the OpenClaw WeChat channel being reconnected (it was disconnected 2026-11-02): fill 张凤's receiving identity into `~/workspace/goals/goal/hidden_files/zhangfeng-wechat.conf` so the daily poster automation goes live the next morning. Until a reconnect, the 企业微信 thread above is the live route. (memory://md:MEMORY.md)
- [ ] RETIRED 2026-10-20: the ilink-based routes (one-time auth link for 张凤; semi-auto user forward) and the "user shares the ClawBot" plan — superseded by the 企业微信 path the user chose; the bot's passive-only protocol and non-shareable plugin nature made them dead ends. (window 2026-10-20T09:47:56.520+00:00, message:assistant-msg-4930d84d-3658-4532-b72a-40f66715d36b)

## Strengthening
