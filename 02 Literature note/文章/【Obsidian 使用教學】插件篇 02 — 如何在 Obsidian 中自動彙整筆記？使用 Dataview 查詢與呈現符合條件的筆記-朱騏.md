
# Dataview語法
用 ```dataview 當作開頭，最後用 ``` 將指令包住。
> dataview  
> [TABLE|LIST|TASK] field1, field2, ..., fieldN FROM # tag or "folder" or [[link]]  
> WHERE somefield = somevalue  
> COMMAND argument  

**中文翻譯版**
> dataview  
> 輸出格式(Table/List/Task) 欄位名稱  
> from [#tag 或 資料夾 或 [[筆記]] ]  
> where 條件  
> sort 欄位 [排序]  

---

**範例**
>LIST
FROM ""
WHERE contains(file.inlinks, [[110 蘭博大陸]])
SORT file.name DESC

# Dataview `WHERE` 可用條件速查表

| 屬性 | 類型 | 說明 | 範例用法 |
|------|------|------|----------|
| `file.name` | string | 檔案標題（不含副檔名） | `WHERE file.name = "110 蘭博大陸"` |
| `file.folder` | string | 所在資料夾路徑 | `WHERE file.folder = "110 蘭博大陸"` |
| `file.path` | string | 檔案完整路徑（含副檔名） | `WHERE contains(file.path, "蘭博")` |
| `file.link` | link | 指向該檔案的連結 | `WHERE file.link = [[110 蘭博大陸]]` |
| `file.size` | number | 檔案大小（bytes） | `WHERE file.size > 1000` |
| `file.ctime` | datetime | 建立時間（日期＋時間） | `WHERE file.ctime > date(2025-01-01)` |
| `file.cday` | date | 建立日期（只有日期） | `WHERE file.cday = date(2025-08-18)` |
| `file.mtime` | datetime | 最後修改時間（日期＋時間） | `WHERE file.mtime > date(2025-08-01)` |
| `file.mday` | date | 最後修改日期（只有日期） | `WHERE file.mday = date(today)` |
| `file.tags` | array | 所有標籤（含階層拆解） | `WHERE contains(file.tags, "#TRPG")` |
| `file.etags` | array | 顯式標籤（不含拆解） | `WHERE contains(file.etags, "#TRPG/模組")` |
| `file.inlinks` | array | 指向該檔案的連結來源 | `WHERE contains(file.inlinks, [[110 蘭博大陸]])` |
| `file.outlinks` | array | 該檔案連出去的連結 | `WHERE contains(file.outlinks, [[迷霧之罐]])` |
| `file.aliases` | array | 檔案的所有別名 | `WHERE contains(file.aliases, "蘭博世界")` |
| `file.day` | date | 檔案內 YAML/行內日期 | `WHERE file.day = date(2025-08-18)` |


---
來源：[朱騏部落格](https://medium.com/pm%E7%9A%84%E7%94%9F%E7%94%A2%E5%8A%9B%E5%B7%A5%E5%85%B7%E7%AE%B1/obsidian-%E4%BD%BF%E7%94%A8%E6%95%99%E5%AD%B8-%E6%8F%92%E4%BB%B6%E7%AF%87-02-%E5%A6%82%E4%BD%95%E5%9C%A8-obsidian-%E4%B8%AD%E8%87%AA%E5%8B%95-%E5%BD%99%E6%95%B4%E7%AD%86%E8%A8%98-8d90b5e44f6a)
#Refrence #檔案管理 