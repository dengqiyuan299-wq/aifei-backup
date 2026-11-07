---
display_name: "张凤"
first_name: "凤"
last_name: "张"
summary: "WeChat contact who gets the user's daily morning tea poster; a Muse account the user created for her on 2026-11-06 is on the waitlist; the 企业微信 route for the poster is still pending."
rank: 5
updated: "2026-11-06"
---

# 张凤

## Facts
- 张凤 is a contact on the user's WeChat; the user has not named the relationship, so it stays unnamed. On 2026-10-20 ~14:30 CST the user said: "那你现在接管了微信以后，你能把每天你生成的图片发给他，让他再发给我那个微信的张凤。" (window 2026-10-20T06:30:43+00:00, message:3a930a30-7c87-4480-ac0b-adb23407959a)
- The user first asked on 2026-10-20 (~01:17 CST) for the daily morning tea poster to be sent directly to 张凤 via WeChat every day — her first appearance in the record. (window 2026-10-19T17:17:55+00:00, message:78345b9c-71eb-45ec-9e18-9e8c623017c7)
- Delivery automation is built but not live: cron `daily-poster-to-zhangfeng` runs ~08:53 Asia/Shanghai, finds that day's poster, SCPs it to the VPS, sends it via OpenClaw WeChat; reports go to the 工作 side chat. BLOCKED on her receiving identity — the conf file holds an empty placeholder. (memory://md:MEMORY.md)
- The OpenClaw WeChat bot is passive-only: no contacts list, no name search; sending needs her explicit ID. Capturing her ID by having her message the bot was tried twice on 2026-10-20 and failed; sharing the ClawBot is impossible — it is a plugin, not a shareable contact. (memory://md:memory/2026-10-20.md:26–29)
- The user rejected any semi-auto fallback on 2026-10-20 (~01:42 CST): "肯定是你完全接管呀！否则我要你干嘛呢？你这转来转去的。" — full automation is the stated expectation. (memory://md:memory/2026-10-20.md:33)
- The WeChat account swap completed on 2026-10-20 ~14:35 CST: new account verified working bidirectionally, old account fully removed; the user's own `to_user_id` is known/working. (memory://md:MEMORY.md)
- On 2026-10-20 (~17:44–17:49 CST) the user asked for alternatives beyond the passive bot; the assistant proposed 企业微信, PC-WeChat automation, and a service account, recommended 企业微信, and the user chose it. Plan: user registers the enterprise and builds a self-built app (recording 企业ID / AgentId / Secret, adding the VPS IP as trusted IP); assistant then configures the VPS; 张凤 is added as a *member* for full automation (as a mere external contact, each send needs the user to tap confirm). Awaiting Step 1. (window 2026-10-20T09:49:40.989+00:00, message:assistant-msg-4a2c14ed-aab3-412d-ad19-e8fb2e4fcb3e)
- On 2026-11-02 (evening) the user ordered the OpenClaw WeChat connection disconnected, verified the same evening: channel entry deleted, login data sealed, gateway restarted, no WeChat start or polling in new logs. The ClawBot no longer sends or receives; that route is closed unless the user later rescans to reconnect; the 企业微信 route remains pending. (memory://md:MEMORY.md)
- On 2026-11-06 ~16:46 CST the user created a Muse account for 张凤 in the Muse iPad app (under her name, Zhang Feng); it landed on the waitlist, she joined it, and a retry on a Singapore node still did not get in. It is one of three accounts waiting for Meta to expand access or release the waitlist. (memory://md:memory/2026-11-06.md)

## History
- 2026-10-20 morning: the user enabled OpenClaw's WeChat channel and asked for the daily poster to be auto-sent to 张凤 every day. The passive-only bot could not look her up by name and sharing the ClawBot proved impossible; delivery automation was built with a placeholder for her ID, and the user rejected the semi-auto fallback. (memory://md:memory/2026-10-20.md:25–40)
- 2026-10-20 ~12:57–14:35 CST: the user swapped the OpenClaw-bound WeChat account to a new one — completed, verified bidirectional, old binding fully removed — and reconfirmed the poster must go to 张凤. (memory://md:MEMORY.md)
- 2026-10-20 ~17:44–17:49 CST: the user asked for alternatives; the assistant proposed 企业微信 / PC automation / service account, recommended 企业微信, the user chose it, and the four-step setup was laid out. Awaiting Step 1. (window 2026-10-20T09:47:42.313+00:00, message:fee04bda-1d2b-4c9c-812e-2f01795b9fd5)
- 2026-11-02 (evening): the user ordered the OpenClaw WeChat connection disconnected; completed and verified the same evening. (memory://md:MEMORY.md)
- 2026-11-04 morning: that day's poster was not sent — the WeChat channel was still disconnected since 2026-11-02 and her WeChat ID still unconfigured, so the script skipped it by rule. The push stays paused; earlier posters can be backfilled once 企业微信 is connected. (window 2026-11-04T05:12:37.036913+00:00, message:assistant-msg-da3fdc60-8c1c-5961-7e6e-b38ca2a735b2)
- 2026-11-06 ~16:46 CST: the user created a Muse account for 张凤 in the Muse iPad app; it landed on the waitlist, she joined it, and a Singapore-node retry still did not get in. (memory://md:memory/2026-11-06.md)

## The relationship
- The user has not named the relationship, so it stays unnamed. What the evidence shows: 张凤 is a WeChat contact the user wants to reach every morning with the daily 初羽茶盧 poster — important enough for a dedicated daily automation; the user pushed hard against any half-measure ("肯定是你完全接管呀"), reconfirmed the request after the WeChat swap, and when the passive bot blocked full automation settled on the 企业微信 route.
- Nothing else is known yet: how they met, what ties them, how often they talk. The contact so far is entirely through the user's intent to send her the poster.

## In common
- The 初羽茶盧 daily tea poster: the user wants 张凤 to receive it every morning. Nothing more is evidenced.

## Open threads
- [x] 2026-10-20: the OpenClaw-bound WeChat account swap — completed ~14:35 CST; new account verified bidirectional, old account fully removed. (memory://md:MEMORY.md)
- [x] 2026-10-20: route decision — closed; the user asked for alternatives and chose 企业微信. (window 2026-10-20T09:47:42.313+00:00, message:fee04bda-1d2b-4c9c-812e-2f01795b9fd5)
- [ ] 2026-10-20: 企业微信 SETUP — the user completes Step 1 (register the enterprise) and Step 2 (self-built app, record 企业ID/AgentId/Secret, add VPS IP as trusted IP), then tells the assistant, which configures the VPS and walks the 张凤-as-member setup. (window 2026-10-20T09:49:40.989+00:00, message:assistant-msg-4a2c14ed-aab3-412d-ad19-e8fb2e4fcb3e)
- [ ] Conditional on the OpenClaw WeChat channel being reconnected (disconnected 2026-11-02): fill 张凤's receiving identity into the conf file so the daily poster automation goes live the next morning. Until a reconnect, the 企业微信 thread above is the live route. (memory://md:MEMORY.md)
- [ ] 2026-11-06: her Muse account is on the waitlist — created in-app that afternoon, joined the list, still not admitted after a Singapore-node retry; waits on Meta expanding access or releasing the waitlist. (memory://md:memory/2026-11-06.md)
- [ ] RETIRED 2026-10-20: the ilink-based routes and the "user shares the ClawBot" plan — superseded by the 企业微信 path the user chose; the bot's passive-only protocol and non-shareable plugin nature made them dead ends. (window 2026-10-20T09:47:56.520+00:00, message:assistant-msg-4930d84d-3658-4532-b72a-40f66715d36b)

## Strengthening
