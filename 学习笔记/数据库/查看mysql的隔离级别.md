# 查看mysql的隔离级别


## 查看当前会话的隔离级别
```
select @@tx_isolation;
```
![会话隔离级别](_v_images/20200301101245850_1489883113.png)
</br>
## 查看系统的隔离级别
```
select @@global.tx_isolation;
```
![系统隔离级别](_v_images/20200301101321922_806156171.png)