# Crawling Ｇas Fee On TzKT  

# 準備 csv 檔案  
### 1. 進入 [Fxhash GraphQL](https://api.fxhash.xyz/graphql)   

### 2. 在 Operation 欄位填寫   
```
query GenerativeToken($generativeTokenId: Float) {
  generativeToken(id: $generativeTokenId) {
    entireCollection {
      generationHash
    }
  }
}
```

### 3. 在 Variables 欄位填寫   
```
{
  "generativeTokenId": 作品 ID
}
```

![image](https://user-images.githubusercontent.com/87169493/227763089-d8440d27-1c03-400f-8a36-6a1393924f49.png)

### 4. 在 Response 欄位點擊下載 csv 檔案

![image](https://user-images.githubusercontent.com/87169493/227763151-272a7d9a-c347-4310-b36f-fd7ced0a0e14.png)

# 使用 selenium 爬取資料  
### 1. 修改程式碼開頭的檔案名稱（不需要加副檔名）
### 2. 將檔案新增至左側 content 資料夾
### 3. 等待程式執行，完成後會在右側追加 gas fee 欄位
### 4. 儲存新檔案（新檔案會覆蓋原始檔案）
### 5. 若要再次爬取，請重新執行全部的程式碼
