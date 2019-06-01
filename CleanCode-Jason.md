# CleanCode - Jason

## What is clean code

1. 意圖明確
2. 容易維護
3. 功能不重複

## What is Legacy code

1. 遺留代碼
2. 沒有自動測試

## Check Code

### 註解 Code Example

- 說明註解：CleanCode不寫註解，因為註解不一定有人維護，Code會有
- 註解Todo：//Todo: -> 其實直接用Scrum中的Task就好
- 縮寫註解：變數不建議寫縮寫然後用註解再說明，如果有變數很長，想要寫縮寫的話，可以寫在README，說明整個專案的統一簡稱
- DeadCode：不該寫，因為別人會不知道該不該or可不可以刪除
- 註解跟Code邏輯相反：其實會以Code為主，所以註解其實不需要。

> 小結：不要寫註解，用Code表達

### 變數命名 Code Example

- if連續判斷int值，但==1 or ==2看不出來1跟2是什麼 -> 改成用enum對應int值比較好
- 不管是變數還是function，都避免簡寫
- iMaxRequest -> i代表INT -> 不需要額外在變數名稱標注型態
- MultiSelect() 變數，但出來是boolean型態
- incidentNameId -> 這變數到底是Name還是ID
- theCustomer -> 其實不需要the
- List\<Customer> ListOfApprovedCustomers -> 其實型態已經是List了，不需要變數名稱還寫List
- Naming規則：Function -> 開頭大寫，local變數 -> 駝峰，class自己成員變數 -> _開頭，Property 變數-> 全大寫

> 小結：別太長別太短、有意義、從問題來命名

### Duplicate Function / Duplicate Code

- 兩個function內容一樣

> Dry：Don't repeat youself

- ```var Customers``` vs. ```List\<Customer> Customers```

> 變數命名，左邊寫var即可

- long method example

> 一個function單一職責、function盡量<10行、一次只做一件事

### Data Clumn 資料泥沼

- function的參數過多

> 宣告集中多個參數物件，並且僅傳入一個
> Long Parameter：建議不要超過三個參數

### Poor Method Signatures

- ```Orange GetCustomer(int airPlane);```

- 鬼才知道上面Orage、GetCustomer、airPlane是啥

> to Be Continued...

> 作業：找三段Code，Refactor它。