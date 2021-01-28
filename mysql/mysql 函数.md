# 工作中遇到的一些函数

<hr>

## group_concat()

以某个值分组，**group_concat()** 中的字段同一行显示，默认用 **" , "** 分割

```sql
# 以id分组，把price字段的值在同一行打印出来，逗号分隔(默认)
select id , group_concat(price) from good group by id;
```

