# Golang key/Value store frame

because of k/v stord doesn't has table
没有表的概念，使用前缀实现，前缀分割符"`"。

key一般由

```
a`b
```

组成，a代表表名，b代表字段名，称为标准key。

当函数名包含Table时，必须为标准key。

当然key可以没有分割符，可以认为一个表为一个值；只能使用函数名不含Table的函数操作。

当key包含两个及以上的的分割符时，为不合法。

