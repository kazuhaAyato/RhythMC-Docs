# 编辑器命令

:::danger[注意]
本文档可能落后于插件版本
如果你不知道或者有误,请使用/editor获取相应指令的帮助！
::


## 创建谱面

- `/editor create <曲名> <曲师> <长度>`: 创建一个新的谱面。

## 完成编辑

- `/editor finish`: 完成当前的谱面的编辑，完成后谱面将锁定，审核通过后即可上线。

## 设置谱面元数据

- `/editor setmeta <meta> <value>`: 设置谱面元数据。

## 读取谱面

- `/editor read <谱名>`: 读取一个谱面。

## 播放谱面

- `/editor play`: 播放当前编辑器中的谱面(15s)
- 如果正在播放，则取消当前播放

## 保存谱面

- `/editor save`: 保存当前编辑器中的谱面。

## 退出编辑器

- `/editor quit`: 退出编辑器。

## 设置chunk

- `/editor edit <chunk编号>`: 设置当前的chunk id。

## 偏移Chunk

- `/editor shift <tick>`: 将本Chunk整体偏移几个tick

## 设置特效

- `/editor effects hologram <开始Tick> <持续Tick> <相对x> <相对y> <相对z> <内容>`: 设置一个全息图特效。

- `/editor effects invert <开始Tick> <持续Tick>`: 设置一个反转特效。

- `/editor effects message <开始Tick> <信息>`: 设置一个消息特效。

- `/editor effects speed <开始tick> <速度>`: 设置一个速度特效

- `/editor effects effect <开始Tick> <持续Tick> <药水等级> <药水类型>`: 设置一个药水特效。

- `/editor effects time <开始Tick> <持续Tick> <时间>`: 设置一个时间特效。

- `/editor effects color <开始Tick> <颜色ID>`: 设置一个颜色特效。

- `/editor effects remove <tick>`: 移除一个特效。

