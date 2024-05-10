---
sidebar_position: 3
---

# 变速
  
修改Note的速度。

## 谱面格式
```json
    {
        "effect-type":"SPEED",
        "start-tick":0,
        "duration": 10,
        "speed": 1.0
    }
```
start-tick : 开始时间(tick)  
duration : 持续时间(tick)  
speed: 速度(block/tick)

## 创建方式

### 命令

`/editor effects speed <开始tick> <持续tick> <速度>`  
**参数&lt;开始tick>** : 整数，表示开始时间的绝对tick.  

**参数&lt;速度>** : 浮点数，表示更改成的速度(单位为 格/t )