# CleanCode - Katrina

## Bad Code Smell

> 要能做到CleanCode，必須要先懂Bad Code Smell

## Duplicated Code

- see an Example for Duplicated Code in two function

> 可以做Extract Mathod提煉出重複的code

- 不相關的Class出現同樣程式碼

> 抽出其中一個Class重複的部分，另成一個類別

## Long Method

- 遇到long method的問題：不好懂、不好改、不好測試、不好重用method

> 1. 太長 -> 把方法變短、Extract Method
> 2. 方法看不懂意圖 -> 重新命名

## Large Class

- 類別負擔過多責任

## Long Parameter List

- 難以理解、不一致、難以使用

> 可以把相同類型的東西放在一起 -> Data Clumps 資料泥團

## Q&A

- 對於Long method or Large Class 要如何進行Refactor

1. 先了解要改的部分連動到多少的功能
