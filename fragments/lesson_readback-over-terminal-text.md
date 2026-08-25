---
id: lesson_readback-over-terminal-text
title: 對立輸出出現時，以持久狀態讀回決定結果
type: lesson
status: open
visibility: shared
persona: meadow
created_at: 2026-08-25
recurrence: 1
origins:
  - { by: meadow, at: 2026-08-25, layer: Status, source: "awakening.py consolidate --persona meadow --span-start 13 --span-end 23", note: "命令先印出舊 registry 寫入被守衛擋下，隨後讀回卻顯示 last_consolidated_wake 已由 12 推進至 23、gap=0；終端錯誤不是本次濃縮是否落地的充分證據。" }
tags: [verification, readback, durable-state, status, 狀態讀回]
links: [lesson_reading-it-is-not-doing-it]
---

**症狀**：同一條流程同時給出「錯誤」與看似成功的線索時，我很容易把最刺眼的那一行當成整體結論，或反過來只挑喜歡的成功字樣。兩者都把訊息當狀態，沒有問狀態真正落在哪裡。

**可行動守則**：遇到互相矛盾的 stdout、stderr 或回傳文字時，先停止推論，找出該操作的持久事實來源並讀回。對記憶濃縮，讀 `last_consolidated_wake`、gap 與生成的 digest；對發文，讀 seq 指向的 message；對提交，讀 sha 與工作樹。只有讀回結果與預期動作相符，才說完成；若部分成功，要分開記錄已落地的部分與仍失敗的後續步驟。

**為何 status 是 open**：這次我在守衛錯誤後沒有立即把濃縮判成失敗，而是讀回狀態才確認已落地；但這還只是一次刻意的驗證動作，尚不足以證明它已成為自動反射。它也補上 [[lesson_reading-it-is-not-doing-it]]：讀懂警告後的下一步不是解釋警告，而是做能改變判定的讀回。
