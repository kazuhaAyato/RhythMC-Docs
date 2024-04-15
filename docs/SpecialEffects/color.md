---
sidebar_position: 2
---

# 更改Note颜色

我没拍呢

更改除了Note_DO_Not_Click以外所有Note的发光颜色

## 谱面格式
```json
    {
        "effect-type":"COLOR",
        "start-tick":10,
        "color": "GREEN"
    }
```
start-tick : 开始时间(tick)  
color: 颜色名字(ChatColorz)

## 创建方式

### 命令

`/editor effects color <开始tick> <颜色id>`  
**参数&lt;开始tick>** : 整数，表示开始时间的绝对tick.  
**参数&lt;颜色id>** : 字符串，表示颜色的ChatColorID.(RGB(#AABBCC)支持)