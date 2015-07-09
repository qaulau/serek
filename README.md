
使用示例
```python
>>> import serek
>>> x = serek.dumps({1: "foo", "bar": [2, 4, 8]})
>>> x
'a:2:{i:1;s:3:"foo";s:3:"bar";a:3:{i:0;i:2;i:1;i:4;i:2;i:8;}}'
>>> x == serek.serialize({1: "foo", "bar": [2, 4, 8]})
True
>>> serek.loads(x)
{1: 'foo', 'bar': {0: 2, 1: 4, 2: 8}}

```
