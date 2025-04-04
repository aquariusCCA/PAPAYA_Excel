> `SUMIFS` 是 Excel 中非常實用的加總函數，它可以根據 **多個條件** 來加總資料，非常適合處理報表、統計或篩選性的數據。

---

### 🧠 **SUMIFS 語法說明：**

```excel
SUMIFS(sum_range, criteria_range1, criteria1, [criteria_range2, criteria2], ...)
```

| 參數 | 說明 |
|------|------|
| `sum_range` | 要加總的數值範圍 |
| `criteria_range1` | 條件1的範圍 |
| `criteria1` | 條件1 |
| `criteria_range2` | 條件2的範圍（可選） |
| `criteria2` | 條件2（可選） |
| ... | 可以有多組條件 |

---

### 📘 **實際應用範例**

假設你有一張銷售表格如下（在 A1:D6）：

| A      | B       | C          | D     |
|--------|---------|------------|-------|
| 日期   | 銷售員  | 商品類別   | 金額  |
| 3/1    | 小明    | 飲料       | 200   |
| 3/2    | 小華    | 零食       | 150   |
| 3/2    | 小明    | 零食       | 100   |
| 3/3    | 小明    | 飲料       | 300   |
| 3/3    | 小華    | 飲料       | 250   |

---

### 🎯 **問題：請問小明賣出飲料的總金額是多少？**

使用公式：

```excel
=SUMIFS(D2:D6, B2:B6, "小明", C2:C6, "飲料")
```

👉 解釋：
- `D2:D6` 是你要加總的「金額」欄。
- `B2:B6` 是「銷售員」欄，條件為「小明」。
- `C2:C6` 是「商品類別」欄，條件為「飲料」。

✅ 結果為：`200 + 300 = 500`

---

### 🔁 **更多進階用法：**

**加總 3 月 2 日 小明 的銷售金額：**

```excel
=SUMIFS(D2:D6, A2:A6, "3/2", B2:B6, "小明")
```

✅ 結果為：100（小明在 3/2 賣出零食）

---

如果你希望我幫你套用你自己的表格內容，也可以貼上資料，我可以幫你寫出對應的 `SUMIFS` 範例 👌  
需要我幫你練習幾題嗎？