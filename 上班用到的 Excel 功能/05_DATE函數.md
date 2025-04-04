> `DATE` 函數是 Excel 裡非常重要的**日期處理工具**，可以用來**組合年、月、日，形成一個完整的日期**。

---

## 🧩 `DATE` 函數語法：

```excel
DATE(year, month, day)
```

- `year`：年份
- `month`：月份（可超過 12）
- `day`：日期（可超過 31）

👉 傳回值是**真正的日期格式**，可以用來做加減、排序、日期計算等操作。

---

## ✅ 常見應用範例

---

### 1. **組合年、月、日變成日期**
假設：
- A1 是年：`2025`
- B1 是月：`3`
- C1 是日：`27`

公式：

```excel
=DATE(A1, B1, C1)
```

📌 結果是 `2025/3/27`（依照你的日期格式設定顯示）

---

### 2. **用公式建立某年1月1日**
想要產生 2024 年的元旦：

```excel
=DATE(2024, 1, 1)
```

---

### 3. **月份超過 12 或天數超過 31 的自動調整**
Excel 會自動調整超過的部分，例如：

```excel
=DATE(2024, 13, 5)
```

📌 會變成：`2025/1/5`（13 月等於下一年的 1 月）

---

```excel
=DATE(2024, 1, 35)
```

📌 會變成：`2024/2/4`（1 月多出來的天數自動進位）

這很實用在做「月底加幾天」或「跨月」時的處理！

---

### 4. **結合其他函數使用**
如果你用 `YEAR`, `MONTH`, `DAY` 拆解某個日期，然後用 `DATE` 組回來也沒問題：

```excel
=DATE(YEAR(A1), MONTH(A1)+1, DAY(A1))
```

📌 這個例子是：把 A1 的日期往**下一個月**。

---

### 5. **找出某個月份的第一天**
A1 是任意日期，例如 `2025/03/27`：

```excel
=DATE(YEAR(A1), MONTH(A1), 1)
```

📌 結果是：`2025/3/1`

---

### 6. **找出某個月份的最後一天（配合 EOMONTH 函數）**

```excel
=EOMONTH(A1, 0)
```

📌 回傳 A1 所在月份的最後一天，例如 `2025/3/31`

---

如果你有特定想處理的日期情境（像是自動計算幾天後的日期、顯示某個年份的所有月底等等），也可以告訴我，我可以幫你設計公式 😄