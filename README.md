Welcome to your new dbt project!
# Doc 
https://github.com/dbt-labs/dbt-starter-project
https://medium.com/kkdaytech/dbt-data-build-tool-part1-introduction-b41cae4800bb

ithome
https://ithelp.ithome.com.tw/articles/10317471

dbt syntax
https://docs.getdbt.com/reference/node-selection/syntax

dbt test official doc
https://docs.getdbt.com/docs/build/data-tests

### Using the starter project

Try running the following commands:
- dbt run
- dbt test


### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [dbt community](https://getdbt.com/community) to learn from other analytics engineers
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices
- dbt_project.yml  https://ithelp.ithome.com.tw/m/articles/10317471

models: 存放 .sql 檔案，寫入需要用到的 SQL 語句，當使用 dbt run 可以在你的 Data Warehouse 建立此 model。
tests: 測試 dbt 中的 models 或其他資源做出 assert，當運行 dbt test 的時候則可以知道哪些是通過，哪些是失敗的。
marcos: 在 dbt 中可以使用 jinja 模板語言結合，而 marcos 則是可以多次重複使用的程式碼，類似於程式語言中的函數，若有重複的程式碼則可以好好的多加利用 marcos 。
snapshots: 有時候分析師需要 “look back” 也就是有些動態表的某些歷史資料。而 snapshots 紀錄了表隨時間的變化。
analysis: dbt 的 model 概念使資料團隊可以輕鬆地進行版本控制和協作進行資料轉換。 但有時，某個 SQL 語句並不完全適合 dbt model。 這些更具“分析性”的 SQL 可以使用 dbt 的分析功能在 dbt 項目中進行版本控制。
dbt_project.yml: 有這個設定檔案，dbt 才知道現在此專案是 dbt 的專案，裡面也可以設定一些重要資訊。



## dbt command 
dbt run 

dbt test 

dbt compile - check syntax error without modifying db

dbt build 
dbt docs generate - generate dbt doc
dbt docs serve - generate web browser at local



FAQ
Q1-dbt command not found?
A1-need to source .vent/bin/activate


Q2-How to add unit test?
-add schema.yml to tests/
-add sql to tests/
