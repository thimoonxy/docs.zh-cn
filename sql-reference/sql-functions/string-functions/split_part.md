# split_part

## description

### Syntax

`VARCHAR split_part(VARCHAR content, VARCHAR delimiter, INT field)`

根据分割符拆分字符串, 返回指定的分割部分(从一开始计数)。

## example

```Plain Text
MySQL > select split_part("hello world", " ", 1);
+----------------------------------+
|split_part('hello world', ' ', 1) |
+----------------------------------+
| hello                            |
+----------------------------------+

MySQL > select split_part("hello world", " ", 2);
+-----------------------------------+
| split_part('hello world', ' ', 2) |
+-----------------------------------+
| world                             |
+-----------------------------------+

MySQL > select split_part("2019年7月8号", "月", 1);
+-----------------------------------------+
| split_part('2019年7月8号', '月', 1)     |
+-----------------------------------------+
| 2019年7                                 |
+-----------------------------------------+

MySQL > select split_part("abca", "a", 1);
+----------------------------+
| split_part('abca', 'a', 1) |
+----------------------------+
|                            |
+----------------------------+
```

## keyword

SPLIT_PART,SPLIT,PART
