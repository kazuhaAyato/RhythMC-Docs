
# 手动修改谱面文件
这个功能正在开发中。但是谱面文件的格式已经在这里了。  

```json
{
// RhythMC Beatmap v1.0
    "meta":{ // 谱面的基本信息
		"name":"Intro", // 谱面名称
		"composer":"Frkovo", // 作曲家
		"charter":"a765dbe0-44eb-3cb1-961d-3967c00c6a77", // 制谱玩家的uuid
		"level":1.0, // 等级
		"offset":3, // 谱面整体偏移量
		"flow-speed":1.0, // 音符流速
		"uuid":"ad3dac5d-7af7-b63e-c57b-abbf4478e1b6", // 谱面唯一uuid
		"length":3320 // 歌曲长度
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