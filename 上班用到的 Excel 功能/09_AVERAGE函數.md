## ✅ `AVERAGE` 函數的基本語法：

```excel
=AVERAGE(number1, [number2], ...)
```

- **number1, number2...**：你要計算平均值的數字、儲存格或範圍。
- Excel 會自動忽略空白儲存格或非數字的內容（像是文字）。

---

## 🧠 功能簡介：

`AVERAGE` 函數會計算選定數值的**算術平均值**，也就是「總和 ÷ 筆數」。

---

## 📘 實際應用範例：

### 🧾 範例情境：學生分數平均

你有一個表格如下：

| A     | B         |
|-------|-----------|
| 姓名  | 成績       |
| 小明  | 80        |
| 小華  | 90        |
| 小美  | 70        |
| 小強  | 85        |

你希望計算這 4 位學生的平均分數。

### ✏️ 步驟：

1. 在 Excel 中選擇一個儲存格（例如 `B6`）
2. 輸入以下公式：
   ```excel
   =AVERAGE(B2:B5)
   ```
3. 按下 Enter，你會看到結果是 `81.25`，這就是平均分數。

---

## 🔁 延伸應用：

### 1. **跳過空白儲存格：**
如果某些成績尚未填寫，例如小美的成績是空白：
| 小明 | 80 |
| 小華 | 90 |
| 小美 | （空白） |
| 小強 | 85 |

`=AVERAGE(B2:B5)` 的結果會是 `(80+90+85)/3 = 85`  
👉 Excel 自動忽略空白儲存格。

---

### 2. **搭配條件使用（進階，可用 AVERAGEIF）：**
假設你只想計算「成績 ≥ 80」的平均分數，可以用：

```excel
=AVERAGEIF(B2:B5, ">=80")
```

---

需要我幫你做一份練習檔案或有其他想算的場景嗎？😊