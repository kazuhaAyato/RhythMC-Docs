
# 手动修改谱面文件


## 命令说明
- `/editor upload`：获取谱面源文件
- `/editor download <url>`：导入修改后的谱面文件

## 操作流程
1. **获取谱面源文件**  
   输入 `/editor upload` 命令，获取一个 URL。用浏览器打开该 URL，即可查看谱面的所有内容。

2. **编辑谱面文件**  
   - 打开一个 JSON 编辑器（推荐使用 VSCode）。
   - 将谱面内容全选并复制到编辑器内。
   - 根据需求修改内容。

3. **上传修改后的谱面文件**  
   - 打开 [https://paste.frkovo.cn](https://paste.frkovo.cn)。
   - 将修改后的谱面文件内容复制粘贴到页面中。
   - 点击左上角的 **Upload** 按钮。

4. **导入修改后的谱面**  
   - 复制上传后获得的 URL。
   - 返回编辑器，输入 `/editor download <复制的URL>`，即可完成导入。

## 谱面示例
```json
{
// RhythMC Beatmap v1.2 / alias/comments update
    "meta":{ // 谱面的基本信息
		"name":"Intro", // 谱面名称
		"composer":"Frkovo", // 作曲家
		"charter":"a765dbe0-44eb-3cb1-961d-3967c00c6a77", // 制谱玩家的uuid
		"level":1.0, // 等级
		"offset":3, // 谱面整体偏移量
		"flow-speed":1.0, // 音符流速
		"uuid":"ad3dac5d-7af7-b63e-c57b-abbf4478e1b6", // 谱面唯一uuid
		"length":3320, // 歌曲长度
		"alias":"观星者", // 别名: aka.中文翻译 balabala
		"comments":[ // 谱面警告什么之类的
			"[FINE]这是一个测试",
			"[WARN]光敏性癫痫",
			"[SEVERE]IDK WHAT SEVERE STUFF IT CAN DO"
		] 
	},
	"frames":[ // 帧
		{ // 每个帧都由一个JSONObject代替。
			"judge-tick":540, // 判定tick,不是生成的tick!!!
			"notes":[ // 所有Notes列表
				{ 
					"type":"NOTE_LOOK",
					"pos":[
						-1,
						1
					]
				}
			]
		},
		{
			"judge-tick":541,
			"notes":[
				{
					"type":"NOTE_DO_NOT_CLICK",
					"pos":[
						0,
						0
					]
				},
				{
					"type":"NOTE_DO_NOT_CLICK",
					"pos":[
						0,
						1
					]
				},
				{
					"type":"NOTE_DO_NOT_CLICK",
					"pos":[
						1,
						0
					]
				},
				{
					"type":"NOTE_RIGHT_CLICK",
					"pos":[
						1,
						2
					]
				}
			]
		}
	],
	"effects":[ //谱面特效
		{
			"effect-type":"HOLOGRAM",
			"start-tick":0,
			"duration":36,
			"hologram-loc":[
				0,
				1
			],
			"hologram-contents":[
				"&b&lHi!"
			]
		},
		{
			"effect-type":"INVERT",
			"start-tick":10,
			"time":10
		},
		{
			"effect-type":"HOLOGRAM",
			"start-tick":36,
			"duration":36,
			"hologram-loc":[
				0,
				1
			],
			"hologram-contents":[
				"&b&l你好!"
			]
		},
		{
			"effect-type":"HOLOGRAM",
			"start-tick":72,
			"duration":36,
			"hologram-loc":[
				0,
				1
			],
			"hologram-contents":[
				"&b&l欢迎来到&a&lRhyth&2&lMC&b&l!"
			]
		},
		{
			"effect-type":"COLOR",
			"start-tick":100,
			"color":"GREEN"
		},
		{
			"effect-type":"HOLOGRAM",
			"start-tick":108,
			"duration":80,
			"hologram-loc":[
				0,
				1
			],
			"hologram-contents":[
				"&b&l一起熟悉一下游戏的玩法吧!"
			]
		}
	],
}
```