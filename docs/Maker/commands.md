# 编辑器命令手册

本手册详细介绍了 RhythMC 的编辑器命令用法及指令分类。通过本手册，您可以快速了解如何使用编辑器进行谱面编辑、特效添加、元数据设置等操作。

---

## 目录
1. [基础命令](#基础命令)
2. [谱面编辑](#谱面编辑)
3. [元数据管理](#元数据管理)
4. [特效管理](#特效管理)
   - [全息特效 (Hologram)](#全息特效-hologram)
   - [高级全息特效 (TextDisplay)](#高级全息特效-textdisplay)
   - [TextDisplay 变换特效 (TextTrans)](#textdisplay-变换特效-texttrans)
   - [其他特效](#其他特效)
5. [审核与发布](#审核与发布)
6. [其他命令](#其他命令)

---

## 基础命令

### 帮助命令
- **命令**: `/editor help`
- **描述**: 显示帮助信息。
- **用法**: `/editor help [页数]`

### 创建新谱面
- **命令**: `/editor create`
- **描述**: 创建一个新的谱面。
- **用法**: `/editor create <曲名> <曲师> <长度>`
- **示例**: `/editor create MySong ComposerName 120`

### 退出编辑器
- **命令**: `/editor quit`
- **描述**: 退出当前编辑器。
- **用法**: `/editor quit`

---

## 谱面编辑

### 读取谱面
- **命令**: `/editor read`
- **描述**: 读取一个已存在的谱面。
- **用法**: `/editor read <谱名>`
- **示例**: `/editor read MySong`

### 保存谱面
- **命令**: `/editor save`
- **描述**: 保存当前编辑器中的谱面。
- **用法**: `/editor save`

### 播放谱面
- **命令**: `/editor play`
- **描述**: 播放当前编辑器中的谱面。
- **用法**: `/editor play`

### 偏移当前 Block
- **命令**: `/editor shift`
- **描述**: 偏移当前 Block。
- **用法**: `/editor shift <偏移量>`
- **示例**: `/editor shift 10`

### 部分偏移
- **命令**: `/editor partshift`
- **描述**: 偏移一段 tick。
- **用法**: `/editor partshift <开始tick> <结束tick> <偏移量>`
- **示例**: `/editor partshift 100 200 10`

---

## 元数据管理

### 设置元数据
- **命令**: `/editor setmeta`
- **描述**: 设置谱面元数据。
- **用法**: `/editor setmeta <meta> <value>`
- **示例**: `/editor setmeta name MySong`

### 列出元数据
- **命令**: `/editor listmeta`
- **描述**: 列出谱面元数据。
- **用法**: `/editor listmeta`

### 强制重新加载
- **命令**: `/editor forcereload`
- **描述**: 强制重新从磁盘加载谱面。
- **用法**: `/editor forcereload`

---

## 特效管理

### 全息特效 (Hologram)

#### 添加全息图特效
- **命令**: `/editor effects hologram`
- **描述**: 设置一个全息图特效。
- **用法**: `/editor effects hologram <开始Tick> <持续Tick> <相对x> <相对y> <相对z> <内容>`
- **示例**: `/editor effects hologram 100 50 0 2 0 HelloWorld`

---

### 高级全息特效 (TextDisplay)

#### 添加高级全息特效
- **命令**: `/editor effects textDisplay`
- **描述**: 设置一个高级全息特效。
- **用法**: `/editor effects textDisplay <开始Tick> <相对x> <相对y> <相对z> <内容> [可选:名称]`
- **示例**: `/editor effects textDisplay 100 0 2 0 HelloWorld MyDisplay`

---

### TextDisplay 变换特效 (TextTrans)

#### 变换特效 (Transformation)
- **命令**: `/editor effects textTrans Transformations`
- **描述**: 设置全息特效的变换效果。
- **用法**: `/editor effects textTrans Transformations <目标ID> <起始Tick> <目标位置x> <目标位置y> <目标位置z> <旋转角度> <大小变化> <持续时间>`
- **示例**: `/editor effects textTrans Transformations MyDisplay 100 0 2 0 45 1.5 50`

#### 背景颜色特效 (BackgroundColor)
- **命令**: `/editor effects textTrans BackgroundColor`
- **描述**: 设置全息特效的背景颜色。
- **用法**: `/editor effects textTrans BackgroundColor <目标ID> <起始Tick> <Alpha> <Red> <Green> <Blue> <持续时间>`
- **示例**: `/editor effects textTrans BackgroundColor MyDisplay 100 255 0 0 255 50`

#### 阴影特效 (Shadow)
- **命令**: `/editor effects textTrans Shadow`
- **描述**: 设置全息特效的阴影效果。
- **用法**: `/editor effects textTrans Shadow <目标ID> <起始Tick> <是/不是> <持续时间>`
- **示例**: `/editor effects textTrans Shadow MyDisplay 100 true 50`

#### 背景透明特效 (Transparent)
- **命令**: `/editor effects textTrans Transparent`
- **描述**: 设置全息特效的背景透明效果。
- **用法**: `/editor effects textTrans Transparent <目标ID> <起始Tick> <持续时间>`
- **示例**: `/editor effects textTrans Transparent MyDisplay 100 50`

#### 文字特效 (Text)
- **命令**: `/editor effects textTrans Text`
- **描述**: 设置全息特效的文字内容。
- **用法**: `/editor effects textTrans Text <目标ID> <起始Tick> <内容>`
- **示例**: `/editor effects textTrans Text MyDisplay 100 NewText`

#### 移除特效 (Remove)
- **命令**: `/editor effects textTrans Remove`
- **描述**: 移除全息特效。
- **用法**: `/editor effects textTrans Remove <目标ID> <Tick>`
- **示例**: `/editor effects textTrans Remove MyDisplay 100`

---

### 其他特效

#### 添加反转特效
- **命令**: `/editor effects invert`
- **描述**: 设置一个反转特效。
- **用法**: `/editor effects invert <开始Tick> <持续Tick>`
- **示例**: `/editor effects invert 100 50`

#### 添加消息特效
- **命令**: `/editor effects message`
- **描述**: 设置一个消息特效。
- **用法**: `/editor effects message <开始Tick> <信息>`
- **示例**: `/editor effects message 100 HelloWorld`

#### 添加药水特效
- **命令**: `/editor effects effect`
- **描述**: 设置一个药水特效。
- **用法**: `/editor effects effect <开始Tick> <持续Tick> <药水等级> <药水类型>`
- **示例**: `/editor effects effect 100 50 1 SPEED`

#### 添加时间特效
- **命令**: `/editor effects time`
- **描述**: 设置一个时间特效。
- **用法**: `/editor effects time <开始Tick> <时间>`
- **示例**: `/editor effects time 100 6000`

#### 添加颜色特效
- **命令**: `/editor effects color`
- **描述**: 设置一个颜色特效。
- **用法**: `/editor effects color <开始Tick> <颜色ID>`
- **示例**: `/editor effects color 100 RED`

#### 添加速度特效
- **命令**: `/editor effects speed`
- **描述**: 设置一个速度特效。
- **用法**: `/editor effects speed <开始Tick> <速度>`
- **示例**: `/editor effects speed 100 1.5`

#### 列出特效
- **命令**: `/editor effects list`
- **描述**: 列出当前 Tick 的特效列表。
- **用法**: `/editor effects list <Tick>`
- **示例**: `/editor effects list 100`

#### 移除特效
- **命令**: `/editor effects remove`
- **描述**: 移除一个特效。
- **用法**: `/editor effects remove <tick> <ID>`
- **示例**: `/editor effects remove 100 1`

---

## 审核与发布

### 完成编辑
- **命令**: `/editor finish`
- **描述**: 完成编辑并提交审核。
- **用法**: `/editor finish`

### 添加合作作者
- **命令**: `/editor coauthors add`
- **描述**: 添加合作谱面作者。
- **用法**: `/editor coauthors add <玩家名>`
- **示例**: `/editor coauthors add Player2`

### 移除合作作者
- **命令**: `/editor coauthors remove`
- **描述**: 移除合作谱面作者。
- **用法**: `/editor coauthors remove <玩家名>`
- **示例**: `/editor coauthors remove Player2`

---

## 其他命令

### 设置游戏模式
- **命令**: `/editor gm`
- **描述**: 设置游戏模式为创造模式。
- **用法**: `/editor gm`

### 计算表达式
- **命令**: `/editor eval`
- **描述**: 计算一个表达式。
- **用法**: `/editor eval <表达式>`
- **示例**: `/editor eval 1+1`

### 上传谱面
- **命令**: `/editor upload`
- **描述**: 上传谱面到云端以手动编辑。
- **用法**: `/editor upload`

### 下载谱面
- **命令**: `/editor download`
- **描述**: 下载并覆盖当前谱面。
- **用法**: `/editor download <pasteURL>`
- **示例**: `/editor download https://paste.frkovo.cn/xxxxxx`

---

通过本手册，您可以轻松掌握 RhythMC 编辑器的各项命令，快速进行谱面编辑与特效添加。如有任何疑问，请参考帮助命令或联系管理员。