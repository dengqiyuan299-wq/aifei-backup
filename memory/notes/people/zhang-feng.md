---
display_name: 张凤
first_name: 凤
last_name: 张
summary: WeChat contact who gets the user's daily morning tea poster; on 2026-10-20 the user picked the 企业微信 route to her (registration now in the user's hands) after the passive bot blocked direct auto-send.
rank: 2
updated: 2026-10-20
---

# 张凤

## Facts
- 张凤 is a contact on the user's WeChat. The user has not named the relationship, so it stays unnamed. The user's own words on 2026-10-20 ~14:30 CST: "那你现在接管了微信以后，你能把每天你生成的图片发给他，让他再发给我那个微信的张凤。" (window 2026-10-20T06:30:43+00:00, message:3a930a30-7c87-4480-ac0b-adb23407959a)
- The user first asked on 2026-10-20 (~01:17 CST) for the daily morning tea poster to be sent directly to 张凤 via WeChat every day — the first time 张凤 appears in the record. (window 2026-10-19T17:17:55+00:00, message:78345b9c-71eb-45ec-9e18-9e8c623017c7)
- The delivery automation is built but not yet live: cron `daily-poster-to-zhangfeng` runs daily ~08:53 Asia/Shanghai, finds that day's poster, SCPs it to the VPS, and sends it via the OpenClaw WeChat channel; reports go to the 工作 side chat. It is BLOCKED on her receiving identity — `~/workspace/goals/goal/hidden_files/zhangfeng-wechat.conf` still holds an empty placeholder. (memory://md:MEMORY.md)
- The OpenClaw WeChat bot (ilink `openclaw-weixin`) is passive-only: no contacts list, no name search, `sendmessage` needs the explicit `xxx@im.wechat` ID. Capturing her ID by having her message the bot was tried twice on 2026-10-20 and failed (messages went to the user's personal WeChat; three empty `getUpdates` polls); sharing the ClawBot with her is impossible — it is a plugin, not a shareable contact. (memory://md:memory/2026-10-20.md:26–29; window 2026-10-20T06:33:54+00:00, message:fd5377c8-a6a7-4e93-8900-7e7089c60301)
- The user rejected any semi-auto fallback on 2026-10-20 (~01:42 CST): "肯定是你完全接管呀！否则我要你干嘛呢？你这转来转去的。" — full automation is the stated expectation. (memory://md:memory/2026-10-20.md:33)
- The WeChat account swap completed on 2026-10-20 ~14:35 CST: new account `85ccf63fb5c1-im-bot` verified working bidirectionally (test message delivered ~14:29 CST), old account `c4f7f5f8dc01-im-bot` fully removed. The user's own `to_user_id` is known/working. (memory://md:MEMORY.md; window 2026-10-20T06:29:13+00:00, message:assistant-msg-271c5bd8-6031-4757-ad74-c7fc32cb61f6)
- On 2026-10-20 (~17:44–17:49 CST) the user asked for alternatives beyond the passive bot; the assistant proposed three — **(1) 企业微信** (VPS plugin ready, full address book, truly automatic), **(2) PC-WeChat automation** (script driving a logged-in desktop WeChat; grey-area), **(3) service account** (high bar: license + yearly fee, templates may not pass) — recommended 企业微信, and the user asked how to set it up. (window 2026-10-20T09:47:42.313+00:00, message:fee04bda-1d2b-4c9c-812e-2f01795b9fd5; window 2026-10-20T09:47:56.520+00:00, message:assistant-msg-4930d84d-3658-4532-b72a-40f66715d36b)
- The 企业微信 plan (2026-10-20 ~17:49 CST): **Step 1** (user, ~10 min) — download the 企业微信 app, log in with their WeChat, create an enterprise with the company license photo + face verification. **Step 2** (user) — create a self-built app, record 企业ID / AgentId / Secret, add VPS IP `81.70.12.165` as trusted IP. **Step 3** (assistant) — configure on the VPS via a secure credential entry. **Step 4** — 张凤 must be added as a *member* for full automation (she authorizes a plugin in her WeChat, no separate app needed); as a mere external contact, each send needs the user to tap confirm in the app. Awaiting the user's Step 1. (window 2026-10-20T09:49:40.989+00:00, message:assistant-msg-4a2c14ed-aab3-412d-ad19-e8fb2e4fcb3e)

## History
- 2026-10-20 ~01:11 CST: the user enabled OpenClaw's WeChat channel and scanned the QR code with their personal WeChat. (memory://md:MEMORY.md)
- 2026-10-20 ~01:17 CST: the user asked for the daily morning tea poster to be auto-sent to 张凤 every day — her first appearance in the record. (window 2026-10-19T17:17:55+00:00, message:78345b9c-71eb-45ec-9e18-9e8c623017c7)
- 2026-10-20 ~01:30–01:42 CST: the passive-only bot could not look her up by name; her messages went to the wrong account; sharing the ClawBot turned out impossible. Delivery automation was built with a placeholder for her ID; the user rejected the semi-auto fallback. (memory://md:memory/2026-10-20.md:25–40)
- 2026-10-20 ~12:57–14:35 CST: the user swapped the OpenClaw-bound WeChat account to a new one — completed; new account verified bidirectional, old binding fully removed. (memory://md:MEMORY.md)
- 2026-10-20 ~14:30–14:35 CST: the user reconfirmed the request after the swap — the poster must go to 张凤 — and reported the ClawBot cannot be shared; two ilink-based routes (full-auto auth link vs semi-auto forward) were proposed. (window 2026-10-20T06:30:43+00:00, message:3a930a30-7c87-4480-ac0b-adb23407959a; window 2026-10-20T06:34:57+00:00, message:assistant-msg-ff6ed64a-5cc1-4574-b1b3-9cc63f31a9e6)
- 2026-10-20 ~17:44–17:49 CST: the user asked for alternatives beyond the passive bot; the assistant proposed 企业微信 / PC automation / service account and recommended 企业微信; the user chose it, and the assistant laid out the four-step setup (user registers the enterprise + creates a self-built app; assistant configures the VPS; 张凤 added as a member for full automation). Awaiting the user's Step 1. (window 2026-10-20T09:47:42.313+00:00, message:fee04bda-1d2b-4c9c-812e-2f01795b9fd5; window 2026-10-20T09:49:40.989+00:00, message:assistant-msg-4a2c14ed-aab3-412d-ad19-e8fb2e4fcb3e)

## The relationship
- The user has not named the relationship, so it stays unnamed. What the evidence shows: 张凤 is a WeChat contact the user wants to reach every single morning with the daily 初羽茶盧 poster — she is important enough to have a dedicated daily automation built around her, the user pushed hard against any half-measure ("肯定是你完全接管呀"), reconfirmed the request unprompted after the WeChat swap, and when the passive bot blocked full automation asked for alternatives and settled on the 企业微信 route. This is a contact the user takes seriously.
- Nothing else is known yet: how they met, what ties them, how often they talk. The contact so far is entirely through the user's intent to send her the poster.

## In common
- The 初羽茶盧 daily tea poster: the user wants 张凤 to receive it every morning. Nothing more is evidenced.

## Open threads
- [x] 2026-10-20: the OpenClaw-bound WeChat account swap — completed ~14:35 CST; new account verified bidirectional, old account fully removed. (memory://md:MEMORY.md)
- [x] 2026-10-20: route decision between the two ilink-based routes — closed; the user asked for alternatives and chose 企业微信. (window 2026-10-20T09:47:42.313+00:00, message:fee04bda-1d2b-4c9c-812e-2f01795b9fd5)
- [ ] 2026-10-20: 企业微信 SETUP — the user is to complete Step 1 (register the enterprise in the app with the company license) and Step 2 (create the self-built app, record 企业ID/AgentId/Secret, add VPS IP 81.70.12.165 as trusted IP), then tell the assistant, which configures the VPS and walks the 张凤-as-member setup so the daily poster goes to her automatically. (window 2026-10-20T09:49:40.989+00:00, message:assistant-msg-4a2c14ed-aab3-412d-ad19-e8fb2e4fcb3e)
- [ ] Conditional on 企业微信 going live: fill 张凤's receiving identity into `~/workspace/goals/goal/hidden_files/zhangfeng-wechat.conf` so the daily poster automation goes live the next morning. (memory://md:MEMORY.md)
- [ ] RETIRED 2026-10-20: the ilink-based routes (one-time auth link for 张凤; semi-auto user forward) and the "user shares the ClawBot" plan — superseded by the 企业微信 path the user chose; the bot's passive-only protocol and non-shareable plugin nature made them dead ends. (window 2026-10-20T09:47:56.520+00:00, message:assistant-msg-4930d84d-3658-4532-b72a-40f66715d36b)

## Strengthening
