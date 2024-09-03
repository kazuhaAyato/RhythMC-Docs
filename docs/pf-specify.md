---
sidebar_position: 2
---

# PF等级分

## 什么是Pf等级分？

Proficiency Score (Pf等级分)在RhythMC是用来衡量一名玩家的实力的重要参考目标。

相似机制：Arcaea ptt, Phigros rks, MaimaiDX rating。

## 计算方法

这里将会介绍Pf等级分是如何被计算的。

Pf = `(r10 * 30% + b15 * 70%)/13.5`

单曲Pf = `Difficulity * ((acc% - 55%)/45%)^2`

### r10 = 最近十次游玩的单曲pf的和。

但是有两种特殊情况:

- 当前玩家pf - 本次游玩pf > 2.5 时 本次游玩不计入r10.
- 当本次游玩的谱面难度 >= 16.0 时 以上规则无效，强制计入r10.

### b15 = 玩家单曲pf最高的十五张不同的谱面。

没有特殊情况.
