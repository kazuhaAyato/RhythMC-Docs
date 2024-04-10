---
sidebar_position: 2
---

# NoteHold
踩

![imgsrc](img/Hold.png)

默认材质: `Material.DIAMOND_BLOK`

本Note以长条形式出现在-1层。  
你需要站在和本Note相同的x坐标方块上获得判定。  

长条中的每个Note单独判定。

## 谱面格式
```json
    {
        "type":"NOTE_DO_NOT_CLICK",
        "pos": 0,
        "length":40
    }
```
type : 类型
pos : x坐标
length : Hold的长度 in ticks。

## 创建方式

编辑器放置方块。
:::danger[注意!]
本Note只能在-1轴放置!!
:::
