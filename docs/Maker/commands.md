  # 编辑器命令
  
  :::danger[注意]
  本文档可能落后于插件版本
  如果你不知道或者有误,请使用/editor获取相应指令的帮助！
  :::
  
#### `help`
- **描述**: 显示帮助。
- **用法**: `/editor help [页数]`

#### `create`
- **描述**: 创建一个新的谱面 使用%20代替空格！
- **用法**: `/editor create <曲名> <曲师> <长度>`

#### `finish`
- **描述**: 完成编辑。
- **用法**: `/editor finish`

#### `judge`
- **描述**: 审核谱面。
- **用法**: `/editor judge <类型: pass/reject> [原因]`

#### `coauthors add`
- **描述**: 添加合作谱面作者。
- **用法**: `/editor coauthors add <玩家>`

#### `coauthors remove`
- **描述**: 移除合作谱面作者。
- **用法**: `/editor coauthors remove <玩家>`

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

#### `upload`
- **描述**: 上传谱面到云端以手动编辑。
- **用法**: `/editor upload`

#### `download`
- **描述**: 下载并覆盖当前谱面。
- **用法**: `/editor download <pasteURL>`

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
- **描述**: 设置一个全��图特效。
- **用法**: `/editor effects hologram <开始Tick> <持续Tick> <相对x> <相对y> <相对z> <内容>`

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
