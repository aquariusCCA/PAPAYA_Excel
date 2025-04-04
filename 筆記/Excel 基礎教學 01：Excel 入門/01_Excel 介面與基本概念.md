### 📌 **儲存格 (Cell)**

> Excel 的文件是由「儲存格」組成，每個儲存格都有一個特定的「參照位置」（如 D5、F7）。

- 每個儲存格由欄位（A, B, C, …）與列（1, 2, 3, …）組合而成，例如：  
  - `A1`：表示 A 欄與第 1 列的交叉儲存格。
  - `D5`：表示 D 欄與第 5 列交叉的儲存格。

- 儲存格可以：
  - 輸入**文字**、**數字**、**日期**。
  - 輸入**公式**，例如：
    ```excel
    =A1+B1
    ```
    表示將 A1 和 B1 的數值加總。

---

### 📌 **輸入資料與移動方式**

| 動作 | 鍵盤操作 | 說明 |
|------|----------|------|
| 向下移動 | `Enter` | 完成輸入後跳到下一列 |
| 向右移動 | `Tab` | 完成輸入後跳到下一欄 |
| 向左移動 | `Shift + Tab` | 返回左邊儲存格 |
| 任意移動 | `方向鍵 ↑ ↓ ← →` | 上下左右自由移動 |
| 多儲存格移動 | `Ctrl + 方向鍵` | 一次跳到資料區的邊緣 |
| 移動至最左上 | `Ctrl + Home` | 移至 A1 |
| 移動至最右下資料格 | `Ctrl + End` | 移至最後一格資料 |

---

### 📌 **範例說明**

#### 範例 1：輸入基本資料
在下列位置輸入資料：
| A | B |
|---|---|
| 姓名 | 分數 |
| 小明 | 80 |
| 小美 | 90 |

你可在 A1 輸入 `姓名`，按 `Tab` 鍵跳到 B1 輸入 `分數`，再按 `Enter` 鍵跳到 A2 繼續輸入下一列。

---

#### 範例 2：加總分數

假設 B2 和 B3 有學生分數，想計算總和，選擇 B4 並輸入：

```excel
=SUM(B2:B3)
```

輸入完按 `Enter`，B4 就會顯示 170（80+90）。

---

#### 範例 3：加總指定儲存格

```excel
=B2+B3
```

這是另一種加總方式，直接指定兩個儲存格。

---

> 若你想了解更多像是儲存格格式、資料對齊、欄列調整等，也可以再告訴我，我可以幫你整理更詳細的學習筆記喔！要不要我也幫你製作一份「Excel 快速鍵與操作大全」？👨‍🏫📄