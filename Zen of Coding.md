## Simple is the first discipline of Coding

保持每次代码逻辑简单，一旦单个逻辑发生超过一次的更改，就会叠加风险。

eg
在亚马逊期间，通过更改AddrType和删除部分代码来实现线上效果一致。结果证明AddrType的更改是欠考虑的，而事后向其他人解释为何更改AddrType也变得很复杂。

## Direct. Tricky should not be encouraged.

保持代码逻辑直接，采用Tricky的方法可能简化代码量，长期埋下隐患。

eg
通过允许输入空字符串“”来覆盖原值。一旦其他人将`null!=val` 改成 `StringUtils.isNotBlank(val)`，将引发问题。
