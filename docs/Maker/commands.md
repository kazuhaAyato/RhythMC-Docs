# 编辑器命令

:::danger[注意]
本文档可能落后于插件版本
如果你不知道或者有误,请使用/editor获取相应指令的帮助！
::

#### `calc`
- **描述**: 切换计算器状态。
- **用法**: `/editor calc`

#### `help`
- **描述**: 显示帮助信息。
- **用法**: `/editor help [页数]`

#### `create`
- **描述**: 创建一个新的谱面。使用 `%20` 代替空格。
- **用法**: `/editor create <曲名> <曲师> <长度>`

#### `finish`
- **描述**: 完成编辑。
- **用法**: `/editor finish`

#### `judge`
- **描述**: 审核谱面。
- **用法**: `/editor judge <类型: pass/reject> [原因]`

#### `eval`
- **描述**: 计算一个表达式。
- **用法**: `/editor eval <表达式>`

#### `setmeta`
- **描述**: 设置谱面元数据。
- **用法**: `/editor setmeta <meta> <value>`

#### `comments add`
- **描述**: 添加作者声明 / 警告信息。
- **用法**: `/editor comments add <等级> <value>`

#### `comments remove`
- **描述**: 移除作者声明 / 警告信息。
- **用法**: `/editor comments remove <id>`

#### `comments list`
- **描述**: 列出作者声明 / 警告信息。
- **用法**: `/editor comments list`

#### `shift`
- **描述**: 偏移当前Block。
- **用法**: `/editor shift <偏移量>`

#### `read`
- **描述**: 读取一个谱面。
- **用法**: `/editor read <谱名>`

#### `partshift`
- **描述**: 偏移一段tick。
- **用法**: `/editor partshift <开始tick> <结束tick> <偏移量>`

#### `listmeta`
- **描述**: 列出谱面元数据。
- **用法**: `/editor listmeta`

#### `gm`
- **描述**: 设置游戏模式。
- **用法**: `/editor gm`

#### `forcereload`
- **描述**: 强制重新从磁盘加载谱面。
- **用法**: `/editor forcereload`

#### `play`
- **描述**: 播放当前编辑器中的谱面。
- **用法**: `/editor play`

#### `save`
- **描述**: 保存当前编辑器中的谱面。
- **用法**: `/editor save`

#### `quit`
- **描述**: 退出编辑器。
- **用法**: `/editor quit`

#### `edit`
- **描述**: 设置chunk。
- **用法**: `/editor edit <chunk>`

#### `effects hologram`
- **描述**: 设置一个全息图特效。
- **用法**: `/editor effects hologram <开始Tick> <持续Tick> <相对x> <相对y> <相对z> <内容>`

#### `effects textDisplay`
- **描述**: 设置一个高级全息特效。
- **用法**: `/editor effects textDisplay <开始Tick> <相对x> <相对y> <相对z> <内容>`

#### `effects textTrans Transformations`
- **描述**: 全息特效-变换。
- **用法**: `/editor effects textTrans Transformations <目标ID> <起始Tick> <目标位置x> <目标位置y> <目标位置z> <旋转角度> <大小变化> <持续时间>`

#### `effects textTrans Opacity`
- **描述**: 全息特效-透明度。
- **用法**: `/editor effects textTrans Opacity <目标ID> <起始Tick> <透明度:0-255>`

#### `effects textTrans BackgroundColor`
- **描述**: 全息特效-背景颜色。
- **用法**: `/editor effects textTrans BackgroundColor <目标ID> <起始Tick> <颜色>`

#### `effects textTrans Shadow`
- **描述**: 全息特效-是否阴影。
- **用法**: `/editor effects textTrans Shadow <目标ID> <起始Tick> <是/不是>`

#### `effects textTrans Glowing`
- **描述**: 全息特效-发光颜色。
- **用法**: `/editor effects textTrans Glowing <目标ID> <起始Tick> <颜色>`

#### `effects textTrans Text`
- **描述**: 全息特效-换字。
- **用法**: `/editor effects textTrans Text <目标ID> <起始Tick> <内容>`

#### `effects textTrans Remove`
- **描述**: 全息特效-移除。
- **用法**: `/editor effects textTrans Remove <目标ID> <Tick>`

#### `effects invert`
- **描述**: 设置一个反转特效。
- **用法**: `/editor effects invert <开始Tick> <持续Tick>`

#### `effects judgedot`
- **描述**: 设置/重置一个扩判特效。
- **用法**: `/editor effects judgedot <开始Tick> <百分比>`

#### `effects message`
- **描述**: 设置一个消息特效。
- **用法**: `/editor effects message <开始Tick> <信息>`

#### `effects effect`
- **描述**: 设置一个药水特效。
- **用法**: `/editor effects effect <开始Tick> <持续Tick> <药水等级> <药水类型>`

#### `effects time`
- **描述**: 设置一个时间特效。
- **用法**: `/editor effects time <开始Tick> <时间>`

#### `effects color`
- **描述**: 设置一个颜色特效。
- **用法**: `/editor effects color <开始Tick> <颜色ID>`

#### `effects speed`
- **描述**: 设置一个速度特效。
- **用法**: `/editor effects speed <开始Tick> <速度>`

#### `effects list`
- **描述**: 列出当前Tick的特效列表。
- **用法**: `/editor effects list <Tick>`

#### `effects remove`
- **描述**: 移除一个特效。
- **用法**: `/editor effects remove <tick> <ID>`