# 这里是哪里

这里是[Phigros HTML5](https://github.com/Yuameshi/PhiCommunity)的谱面仓库，用于储存谱面文件

# 提交谱面

在一切的之前，您需要PhiEditor创建的JSON格式谱面或者PEC格式谱面，没有就别说了（

首先`Fork`这个仓库到你的账号，这一步需要一个GitHub账号。如果您没有，只需注册一个，然后 Fork。

首先创建一个具有正确名称的新文件夹，例如 `rrhar` 或 `rrharil` 指的是 `Rrhar'il`。（不要包含特殊字符，如 `' / \ ` 等，不能以.开头）

首先创建一个具有正确名称的新文件夹，例如 `rrhar` 或 `rrharil` 指的是 `Rrhar'il`。（不要包含特殊字符，如 `' / \ ` 等，不能以.开头）

在其中创建或粘贴以下文件
```
meta.json			必须-元数据		(名称不可变更)
base.mp3			必选-音乐		(名称可变更)
chart.json			必须-铺面		(名称可变更)
line.json			可选-判定线贴图	 (名称可变更)
illustration.jpg 	必须-曲绘		 (名称可变更)
```
> 音乐要求：MP3/OGG/WAV等常见格式，大小小于5MB

> 曲绘要求：JPG/PNG等常见格式(WebP没测试过)，大小小于1MB

在`meta.json`内填入歌曲元信息（见下），注意要删除注释，使用英文字符，且双引号需要添加`\`转译。
```javascript
{
	"name":"Rrhar'il",								//曲名
	"codename":"rrharil",							//代号(你的文件夹名称)
	"artist": "Team Grimoire",						//曲师
	"musicFile":"music.ogg",						//音乐文件名
	"ezRanking":7,									//EZ定数（可带小数）
	"hdRanking":12,									//HD定数（可带小数,可与上一个相同）
	"inRanking":15,									//IN定数（可带小数,可与上一个相同）
	"atRanking":16,									//AT定数（可带小数,可与上一个相同）
	"lineTexture":"line.json",						//可选-判定线贴图文件名
	"chartEZ":"Chart_EZ.json",						//EZ谱面（可与上一个相同）
	"chartHD":"Chart_HD.json",						//HD谱面（可与上一个相同）
	"chartIN":"Chart_IN.json",						//IN谱面（可与上一个相同）
	"chartAT":"Chart_AT.json",						//AT谱面（可与上一个相同）
	"chartLegacy":"Chart_AT.json",					//Legacy谱面（可与上一个相同）
	"illustration":"illustration.jpg",				//曲绘文件名
	"ezChartDesigner":"RDRT -p 19:08:31",			//谱师(当此属性存在时将忽略所有其他谱师设定)
	"ezChartDesigner":"RDRT -p 19:08:31",			//EZ谱师
	"hdChartDesigner":"RDRT -p 20:02:21",			//HD谱师
	"inChartDesigner":"RDRT -p 20:08:31",			//IN谱师
	"atChartDesigner":"RWND -p 16493:62786:92551",	//AT谱师
	"illustrator":"犀牛沱动画工坊",					//曲绘画师
	"sliceAudioStart":"84.5"						//预览音频切片开始时间（秒），预览音频持续时间为15秒
}
```

完成后，将谱面文件夹（您之前创建的）上传到 *你的Git仓库*（您之前复刻的那个），然后打开一个新的 `Pull Request` 然后等待合并。

# 请最好一次Commit搞定
