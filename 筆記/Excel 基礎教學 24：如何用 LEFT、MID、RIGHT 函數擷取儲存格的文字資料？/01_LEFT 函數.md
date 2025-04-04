> Excel 中的 `LEFT` 函數用來從**文字的左邊**開始，擷取指定數量的字元。

---

### 📘 函數語法：
```excel
LEFT(text, [num_chars])
```

- `text`：你要擷取字元的原始文字。
- `num_chars`（可選）：你想從左邊開始擷取幾個字元。  
  ➤ 如果省略，預設是 1 個字元。

---

### ✅ 範例說明：

假設 A1 儲存格中有內容：

```
A1 = "Excel教學"
```

#### 範例 1：取左邊前 2 個字元
```excel
=LEFT(A1, 2)
```
🔹 結果為：「Ex」

---

#### 範例 2：只取最左邊的 1 個字元（省略 num_chars）
```excel
=LEFT(A1)
```
🔹 結果為：「E」

---

#### 範例 3：搭配其他函數（例如取姓名中的姓）
假設 A2 儲存格中有姓名：
```
A2 = "王小明"
```

```excel
=LEFT(A2, 1)
```
🔹 結果為：「王」

---

如果你也想學 `RIGHT` 或 `MID` 等相關文字函數，我也可以幫你補上喔！需要嗎？😄