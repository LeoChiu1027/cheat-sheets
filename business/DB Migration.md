
---
1.  DMS Full Load先轉移資料 (drop table) 
2.  admin 帳號執行permission SQL script 和 drop 沒在使用的table
3.  cicduser 設定 table sequences SQL script
4.  cicduser alter table SQL script
5.  cicduser create index
6.  執行migration確認資料庫是否需要調整

### 備註
---
- uat 沒有bcuser是用postgres
