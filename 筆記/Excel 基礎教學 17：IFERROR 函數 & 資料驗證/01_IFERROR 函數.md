# ✅ **什麼是 IFERROR 函數？**

`IFERROR` 是 Excel 的一個函數，用來**處理可能發生錯誤的公式**，並**顯示一個你自訂的訊息或結果**，取代預設的錯誤訊息（例如 `#N/A`、`#DIV/0!` 等）。

---

# 📌 **IFERROR 函數語法**：
```excel
IFERROR(要檢查的公式, 錯誤時顯示的內容)
```

- `要檢查的公式`：你原本會寫的公式，例如 `VLOOKUP()`。
- `錯誤時顯示的內容`：當公式出現錯誤時，要顯示什麼訊息或數值（可以是文字、數字或空白）。

---

# 🎯 **範例說明**

當然可以！以下是 **範例 1** 和 **範例 2** 中會用到的資料結構（Excel 資料表格樣式），你可以照這個格式建立來練習使用 `IFERROR` 函數👇

---

## 📘【成績表】（命名為範圍：成績表）

| 學號 | 分數 |
|------|------|
| A001 | 90   |
| A002 | 85   |
| A003 | 78   |
| A004 | 92   |

這個表可以放在工作表的 A1:B5 範圍，然後選取這個範圍並命名為 `成績表`（使用 Excel 的「名稱管理員」或直接在左上方名稱框設定）。

---

## 🧪【查詢區】（給使用者輸入學號並查詢分數）

| 輸入學號 | 查詢分數 |
|----------|----------|
| C3       | D3       |

- 使用者在 C3 輸入學號（例如：A001、A005）
- D3 則用公式來查詢分數

---

### ✅ 範例 1：處理查無資料

D3 輸入以下公式：
```excel
=IFERROR(VLOOKUP(C3, 成績表, 2, FALSE), "查無此人")
```

### ✅ 範例 2：處理「未輸入學號」時顯示空白

D3 改用以下公式：
```excel
=IF(C3="", "", IFERROR(VLOOKUP(C3, 成績表, 2, FALSE), "查無此人"))
```

---

這樣的設計就可以讓你清楚體會 `IFERROR` 的用途，也能避免出現難懂的錯誤訊息 👌  
如果你想，我也可以幫你設計一份 Excel 範例檔（附公式）給你練習～需要嗎？

# 🧠 小提醒：
- `IFERROR` 會處理**所有錯誤類型**，不只 `#N/A`，像 `#DIV/0!` 也能攔截。
- 若只想處理特定錯誤（如只處理 `#N/A`），可以考慮使用 `IFNA()` 函數（只在 Excel 2013 以上可用）。

---

需要我幫你做個練習題或範例檔案嗎？還是你想要用 IFERROR 搭配其他函數的實戰應用？