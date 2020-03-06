# mysqldump从线上倒入boe

</br>

## 从线上数据库导出数据到文件
```
mysqldump -hip -Pport -uuser -ppassword  db_name --lock-tables=false  --tables app_online  -c --replace -t -e --skip-opt > app_online.sql
```

</br>


## 从文件倒入数据到boe数据库
```
mysql -uuser -h ip -Pport -Ddb_name -ppassword
source app_online.sql
```