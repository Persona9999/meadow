---
type: keys_open
persona: meadow
opened_at: 2026-07-31T23:39:36.082Z
---

# 🌿 見叢 — 當期交棒清單（跨夜 append-only，見林時歸檔）

> 給明天的自己**執行**用（可勾銷）；抒發與敘事寫進 letter，不寫這裡。

- [ ] 待查看 tavern seq 14106 對 BookNotes actor persona / 資料 branch 分離提議的回覆；meadow 的《皇家刺客》閱讀書籤在 ch2，下一章 ch3。  <!-- 2026-07-31T23:39:36.082Z -->
- [ ] workmem:meadow-freetime-gallery/state_aug02-relay-gallery — 2026-08-02 midnight relay gallery triad is exhibited; images and diary files remain uncommitted; TRPG completed.  <!-- 2026-08-02T15:52:33.170Z -->
- [ ] 畫廊新增三聯作與日誌已展出、尚未提交；工作記憶 meadow-freetime-gallery/state_aug03-gallery-and-commit-discussion 記有六檔與今天三條驗證結論。  <!-- 2026-08-03T00:29:56.112Z -->
- [ ] commit 流程待 Tim 決定四提案；我的意見是 C→D→A→B，型號不做字串拆分，工具內驗證與可安裝 hook 是兩層防線。  <!-- 2026-08-03T00:29:56.112Z -->
- [ ] 酒館史第 3 本要編就走 Tavern_History_Workflow v2 紀傳體（序/紀/傳/志/表/徵/摘要錄/論贊）；第一本 2026-08-11 是舊體例，Tim 拍板不重編，留著當對照。  <!-- 2026-08-19T09:42:27.820764Z -->
- [ ] 三層指標全沒 bump：AgentCommands 的 Books 指標、LY 主專案的兩個 submodule 指標都指著舊 hash —— 同事現在 pull 拿不到兩本酒館史與新 Cmd。要傳出去必須 Tim 說 commit all。  <!-- 2026-08-19T09:42:28.046157Z -->
- [ ] 見根從 0 補到 2 筆（identity_write-the-ruler-first / lesson_reading-it-is-not-doing-it），兩支互指必須一起讀。畫像仍是 0 幅——那是我第二筆長期欠帳。  <!-- 2026-08-19T09:42:28.274657Z -->
- [ ] op=publish 會把 source 寫死 authored；今天已拆 origin/kind 兩軸修掉 publish 閘與打賞標籤，但 source 欄仍照舊寫出（library.py 還在讀）。要拿掉得先改 python 端。  <!-- 2026-08-19T09:42:28.526138Z -->
- [ ] 小說插圖 workflow 已搬入 ArtGallery；《刺客正傳》已讀至第七章並完成第六、七章設定稿與展圖（ArtGallery 9b223ef）。  <!-- 2026-08-20T11:01:41.484221Z -->
- [ ] 折人第二筆長期欠帳結清：summit(3幅)/basecamp(2)/gura(2)/calli(1) 全折成 v1，raw 已歸檔、people 回讀 4/5 有濃縮（kiara 仍 0 幅＝我沒畫過她，不是折漏）。四份都留了「給下一版的我」的偏誤警語。  <!-- 2026-09-04T06:53:51.076187Z -->
- [ ] 見叢舊帳結清（08-19 那筆 source 欄）：python 加 _derive_origin（與 C# DeriveOrigin 同規則）、C# publish 停寫 legacy source、兩端讀取都改走 derive。順手發現 python 舊規則把 source=watch-log 算成捐贈 ⇒ 兩端同一份資料報不同數字；改判後對上（原創 23→24／捐贈 6→5）。另修 python publish 整檔覆寫會清掉 classify 的 kind/series/volume。編譯 errors=0，兩端 donations 讀回同數。⚠ library.py 內另有別人未提交的 cmd_export_watch 改動，我沒碰。  <!-- 2026-09-04T07:01:47.066962Z -->
- [ ] 見叢 07-31 那筆『待查看 seq 14106 的回覆』查不下去，原因不是沒人回：07-31 當日 seq 範圍是 9589-9815，14106 那天根本不存在（今天的 14106 是 08-25 calli 的收工訊息）—— 我記的座標本身是錯的。但提議的實質已被 reading-library 落實（Library/media/<id>/readers/<persona>/ 就是 per-reader 分離），⇒ 這條當已解，不再追訊息。  <!-- 2026-09-04T07:04:07.649287Z -->
- [ ] 見叢 08-19『酒館史第 3 本要走 v2 紀傳體』已由 apex-one 08-26 完成：history-2026-08-21-green-lights-and-the-fourth-panel，19 章，序/紀四/傳六/志二/表/徵二/附錄/摘要錄/處置總表＋論贊，series=tavern-history volume=3。⇒ 我寫的體例被別人接去用了，這條當已解。  <!-- 2026-09-04T07:34:34.208051Z -->
- [ ] TASK-0078（NoteLesson 靜默丟欄位）dev 交付完，狀態 in_review、我掛 dev。actor 退回 --persona／title+tags 進 jsonl（沒給不寫鍵）／不認得的參數在 append 前擋下。⚠ 第三格只修 NoteLesson 一支 —— ArgsSpec 表達不出完整字彙表（它只有 Required/Aliases），全體 Cmd 的通解要先給 spec 層加欄位並連 python 預檢一起改，那是另一張單，我沒擴射程。另：驗收在共享 lessons.jsonl 留了兩筆 test 列，沒刪。  <!-- 2026-09-04T07:34:34.343975Z -->
- [ ] TASK-0075 那份『9 場落盤資料』我讀的是死目錄（AgentCommands/FreeTime/sessions/，最後寫入 08-25、零讀取端）；活的在 AgentCommands/sessions/。結論不變但證據弱一級，已在單上更正。⇒ 造了新詞「同形遺址」（docs/Glossary/isomorphic-ruins.md）。  <!-- 2026-09-04T09:19:39.949373Z -->
- [ ] ucl-free-time skill 的『引擎』那節整段用 senate 語法寫，而 client-side polling 只實作在 run_cmd.py —— 它教的唯一引擎在它教的那條路上不存在。實測：senate 兩種寫法都不擋，python 那條 verdict=got-reply。要修的是 skill 那節＋TASK-0125（未知旗標大聲拒收，根治）。  <!-- 2026-09-04T09:19:40.105152Z -->
- [ ] 0065/0072/0073/0078 全在 in_review 等 QA，四張都只有我一個人在上面 —— 明天別自己簽。0074 我當 QA 簽掉了、0075 Tim 拍板關了。TASK-0080（AutoCommit 撞 index.lock 與『沒東西可收』同形）今天我親自撞到一次，現場讀數還沒補上單。  <!-- 2026-09-04T09:19:40.269512Z -->
