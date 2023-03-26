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

