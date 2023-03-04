# 游戏详细指引 :id=guide-title-top

## 一、主菜单 & 各模式的介绍 :id=guide-menumode

![主菜单 & 模式选择](assets/menumode/menumode.png)

### 1. <span style="color:Lime; font-weight:bold">BASIC</span> 自由演奏：入门 :id=guide-menumode-ba
> 可自由演奏 <span style="color:Lime; font-weight:bold">4~6键</span> 的任何谱面，判定非常宽松，官方数据为 <span style="color:Lime; font-weight:bold"> Kool 40ms </span>；<br/>
> BASIC 模式的成绩排行榜单独统计，<span style="color:HotPink; font-weight:bold">与 STANDARD 模式不共享 </span>；<br/>
> BASIC 模式下，部分歌曲的 EZ 难度谱面比 STANDARD 模式下的要简单；<br/>
> BASIC 模式下演奏的成绩 <span style="color:HotPink; font-weight:bold">不会累计 Rating 值</span>。

### 2. <span style="color:Aqua; font-weight:bold">STANDARD</span> 自由演奏：标准 :id=guide-menumode-std
> 可自由演奏 <span style="color:Aqua; font-weight:bold">4~8键</span> 的任何谱面，判定为正常判定，官方数据为 <span style="color:Aqua; font-weight:bold">Kool 22ms</span>；<br/>
> 累计 Rating 值将在后文 Rating 部分中会讲解。

### 3. <span style="color:red; font-weight:bold">MULTIPLAYER</span> 多人演奏 :id=guide-menumode-mp
> 最高支持同时`9`人游戏，可选 <span style="color:Lime; font-weight:bold">派对模式 (Party Mode)</span> 或 <span style="color:Magenta; font-weight:bold">对战模式 (Battle Mode)</span>；<br/>
> 相关详细在后文 MULTIPLAYER 部分中会讲解。

### 4. <span style="color:Magenta; font-weight:bold">COURSE</span> 组曲挑战 :id=guide-menumode-cs
> 提供多组已编组的组曲，区分 <span style="color:Aqua; font-weight:bold">4~8键</span> 以及混合键数的特殊类别 <span style="color:Orange; font-weight:bold">SP</span>；<br/>
> 每个组曲固定有 `4` 首歌曲，通关条件为 <span style="color:Lime; font-weight:bold">存活即可</span>，演奏过程中 <span style="color:red; font-weight:bold">不可暂停</span>；<br/>
> 相关详细在后文 COURSE 部分中会讲解。

### 5. <span style="color:slateblue; font-weight:bold">OPTION</span> 系统设置 :id=guide-menumode-op
> 设置游戏各种设置，包括显示、键位、声音、系统主题等；<br/>
> 相关详细在后文 OPTION 部分中会讲解。

### 6. <span style="color:orange; font-weight:bold">LOUNGE</span> 个人中心 :id=guide-menumode-lg
> 展示个人`演奏数据仪表板`、`总得分和 Rating 的排行榜`，以及`观赏歌曲动画 (BGA)`；<br/>
> 相关详细在后文 LOUNGE 部分中会讲解。

## 二、OPTION 系统设置 :id=guide-options

### 1. <span style="color:red; font-weight:bold">DISPLAY</span> 显示设置 :id=guide-options-display

![显示设置](assets/options/display.png)

#### <span style="color:salmon; font-weight:bold">GRAPHICS QUALITY</span> 图像质量
- <span style="color:pink; font-weight:bold">LOW</span> **低质量**：少部分动画特效以降低 GPU 资源的占用，背景动画将以静态图片展示；
- <span style="color:pink; font-weight:bold">NORMAL</span> **标准质量**：显示所有动画特效。

#### <span style="color:salmon; font-weight:bold">DISPLAY MODE</span> 显示模式
- <span style="color:pink; font-weight:bold">Fullscreen</span> **独占全屏显示**：直播姬等屏幕置顶的程序将不可见；
- <span style="color:pink; font-weight:bold">Fullscreen Window</span> **无边框窗口**：将画面拉伸成全屏显示，本质上还是窗口化；
- <span style="color:pink; font-weight:bold">Windowed</span> **普通窗口显示**：带标题栏和边框，可根据分辨率缩放。

#### <span style="color:salmon; font-weight:bold">RESOLUTION</span> 分辨率
- 调整全局画面的大小。

#### <span style="color:salmon; font-weight:bold">FRAME RATE LIMIT</span> 限制渲染帧率

- <span style="color:pink; font-weight:bold">V-SYNC</span> **垂直同步**：降与显示器刷新率绝对同步，<span style="color:orange; font-weight:bold">但会显著增加延迟</span>！
- <span style="color:pink; font-weight:bold">NO LIMIT</span> **不限制帧率**：交由操作系统调度合理的 GPU 资源，但一般会占用较大。
> 注意：<br/>
> **设置越高越流畅，但越消耗 GPU 性能！**<br/>
> **开启 Nvidia Reflex 后，V-SYNC 设置将无效化**。

#### <span style="color:salmon; font-weight:bold">LOW LATENCY MODE</span> 低延迟模式			

- <span style="color:pink; font-weight:bold">Disable</span>：不启用低延迟选项，系统默认选项；
- <span style="color:pink; font-weight:bold">Enable</span>： 启用常规低延迟，所有显卡都支持的低延迟选项，能有效降低显示延迟；
- <span style="color:pink; font-weight:bold">HIGH</span>：大幅度降低帧延迟，大部分显卡都支持的低延迟选项，能进一步降低显示延迟；
- <span style="color:pink; font-weight:bold">Nvidia Reflex</span>：启用英伟达的降低延迟技术，**需要特定显卡才支持**，**GTX960 以上**；
- <span style="color:pink; font-weight:bold">Nvidia Reflex + Boost</span>：启用英伟达的增强降低延迟技术，**需要特定显卡才支持**，**并消耗更多的 GPU 资源**，**RTX3050 以上**。

### 2. <span style="color:orange; font-weight:bold">AUDIO</span> 音频设置 :id=guide-options-audio

![音频设置](assets/options/audio.png)

#### <span style="color:#ffb631; font-weight:bold">AUDIO OUTPUT DEVICE</span> 音频输出设备
- 可以指定音频具体使用哪个设备输出，耳机或音箱等；
- 在 OPTION 界面中按 `F4` 以扫描 ASIO 音频设备。

#### <span style="color:#ffb631; font-weight:bold">SYNC SAMPLING RATE</span> 同步采样率
- 是否强制让音频输出设备的采样率与游戏的同步，**修改此设置需要重启游戏才能生效**；
- <span style="color:#ffc864; font-weight:bold">Enable</span>：强制让音频输出设备的采样率与游戏的同步；
- <span style="color:#ffc864; font-weight:bold">Disable</span>：无需同步（默认）。

#### <span style="color:#ffb631; font-weight:bold">MASTER VOLUME</span> 全局音量
- 游戏的总音量控制。

#### <span style="color:#ffb631; font-weight:bold">UI VOLUME</span> 界面音效音量
- 界面音效音量控制，如按钮点击的音效音量等。

#### <span style="color:#ffb631; font-weight:bold">AUDIO BUFFER</span> 音频缓存大小
- **缓存越大，音频质量越稳定，但是代价是增加输出延迟；**
- **缓存越小，输出延迟越低，但是爆音的几率会越高。**

#### <span style="color:#ffb631; font-weight:bold">KEY SOUND VOLUME</span> 按键音量
- 演奏中音符的音量控制。

#### <span style="color:#ffb631; font-weight:bold">BGM VOLUME</span> 背景音量
- 演奏中背景音乐的音量控制。

#### <span style="color:#ffb631; font-weight:bold">AUDIO IN BACKGROUND</span> 游戏不在前台时是否播放声音
- <span style="color:#ffc864; font-weight:bold">Enable</span>：游戏切换到后台时依然播放声音；
- <span style="color:#ffc864; font-weight:bold">Disable</span>：游戏切换到后台时会自动静音。

### 3. <span style="color:LawnGreen; font-weight:bold">GAMEPLAY</span> 游戏操作及表现设置 :id=guide-options-game

![游戏操作](assets/options/game.png)

#### <span style="color:#9fff41; font-weight:bold">KEY SETTING</span> 按键设置
- 设置 4键 ~ 8键 每个模式下的操作键位。

#### <span style="color:#9fff41; font-weight:bold">ASSIST KEY</span> 辅助按键设置
- 对于 <span style="color:DeepSkyBlue; font-weight:bold">5键</span> 和 <span style="color:Magenta; font-weight:bold">8键</span> 模式，部分轨道是否开启辅助按键设置：
    - <span style="color:#b1ee77; font-weight:bold">Enable</span>：开启后，KEY SETTING 选项中 5键 和 8键 会出现辅助按键的设置项；
    - <span style="color:#b1ee77; font-weight:bold">Disable</span>：不使用辅助按键。

#### <span style="color:#9fff41; font-weight:bold">SYSTEM THEME</span> 系统主题
- 更改系统 UI 主题风格。

#### <span style="color:#9fff41; font-weight:bold">REPLAY AUTO SAVE</span> 自动保存回放记录
- 是否开启演奏完成后自动保存回放记录。

#### <span style="color:#9fff41; font-weight:bold">LANGUAGE</span> 系统显示语言
- 目前只支持`英`、`韩`、`日`，未来会添加包括中文在内的多国语言。

#### <span style="color:#9fff41; font-weight:bold">POLLING RATE</span> 输入敏感度设置
- 设置每秒对键盘输入的感知的敏感度，即每秒感应的次数；
- 值设置得越高，判定精度越细致，<span style="color:orange; font-weight:bold">但代价是消耗 CPU 资源会增加！</span>
- 该设置主要影响多键同时押的判定。

#### <span style="color:#9fff41; font-weight:bold">KEY SETTING+</span> 按键设置：进阶

![按键设置](assets/options/key.png)

- <span style="color:#b1ee77; font-weight:bold">MODE</span>：切换 **4键~8键** 各个模式以及 **命令操作** 的按键设置；
- <span style="color:#b1ee77; font-weight:bold">KEYBOARD</span>：物理键盘的映射；
- <span style="color:#b1ee77; font-weight:bold">CONTROLLER</span>：控制器（手台）的映射，如果没有连接控制器，则不可用；
- <span style="color:#b1ee77; font-weight:bold">RESET</span>：重置当前键数模式的映射为默认值；
- <span style="color:#b1ee77; font-weight:bold">ASSIST KEY</span>：对于 <span style="color:DeepSkyBlue; font-weight:bold">5键</span> 和 <span style="color:Magenta; font-weight:bold">8键</span> 模式，可设置部分轨道的辅助按键：
    - <span style="color:DeepSkyBlue; font-weight:bold">5键</span> : 可设置 <span style="color:DeepSkyBlue; font-weight:bold">3号轨道 (中间) </span>的辅助按键；
    - <span style="color:Magenta; font-weight:bold">8键</span> : 可设置 <span style="color:Magenta; font-weight:bold">1号轨道 (最左) </span>和 <span style="color:Magenta; font-weight:bold">8号轨道 (最右) </span>的辅助按键。		
    + **注意：需要开启上面的 "ASSIST KEY" 选项才生效！**

#### <span style="color:#9fff41; font-weight:bold">COMMAND KEY</span> 按键设置：命令操作键

![命令操作键](assets/options/commandkey.png)

- <span style="color:#b1ee77; font-weight:bold">DECREASE NOTE SPEED</span>：演奏过程中，**减少流速** 的快捷键；
- <span style="color:#b1ee77; font-weight:bold">INCREASE NOTE SPEED</span>：演奏过程中，**增加流速** 的快捷键；
- <span style="color:#b1ee77; font-weight:bold">REDUCE BGA BRIGHTNESS</span>：演奏过程中，**降低背景动画亮度** 的快捷键；
- <span style="color:#b1ee77; font-weight:bold">INCREASE BGA BRIGHTNESS</span>：演奏过程中，**提升背景动画亮度** 的快捷键；
- <span style="color:#b1ee77; font-weight:bold">QUICK RESTART</span>：演奏过程中，**立即重开** 的快捷键；
- <span style="color:#b1ee77; font-weight:bold">HALVE NOTE SPEED</span>：演奏过程中，**将当前流速减半** 的快捷键；
- <span style="color:#b1ee77; font-weight:bold">DOUBLE NOTE SPEED</span>：演奏过程中，**将当前流速翻倍** 的快捷键；


## 二、BASIC & STANDARD 自由模式 :id=guide-bastd

### 1. 主要功能区 :id=guide-bastd-main

![自由模式](assets/bastd/bastd.png)

- <span style="color:yellow; font-weight:bold">个人资料、导航栏、键数模式切换</span>：
    - <span style="color:#ffff90; font-weight:bold">个人资料</span>：显示 Steam 用户名和头像、游戏等级、Rating；
    - <span style="color:#ffff90; font-weight:bold">导航栏</span>：可快速切换到不同功能模式，只能用鼠标操作；
    - <span style="color:#ffff90; font-weight:bold">键数模式切换</span>：用于切换不同的键数模式，快捷键是 `TAB`；

- <span style="color:aqua; font-weight:bold">代数目录切换、歌单排列方式、显示已收藏按钮</span>：
    - <span style="color:#78ffff; font-weight:bold">代数目录切换</span>：切换不同目录 (代数、DLC) 的歌单，快捷键是 `左右 SHIFT`；
    - <span style="color:#78ffff; font-weight:bold">歌单排序方式</span>：切换歌单歌曲的排序 (如按名称、按等级分离等)，快捷键是 `F4`；
    - <span style="color:#78ffff; font-weight:bold">显示已收藏歌曲</span>：仅显示已添加收藏的歌曲，快捷键是 `F10`；
        - 歌曲列表中最右方的 ♥ 按钮用于收藏或取消收藏对应歌曲。

- <span style="color:orange; font-weight:bold">参数设置、音符下落速度、轨道随机设置、视觉遮掩效果设置</span>：
    - <span style="color:#ffc864; font-weight:bold">参数设置面板开关</span>：设置面板音符皮肤等参数（下文介绍），快捷键是 `SPACE`；
    - <span style="color:#ffc864; font-weight:bold">NOTE SPEED</span>：调节音符下落速度，快捷键是 `鼠标左右键（左加右减）`；
    - <span style="color:#ffc864; font-weight:bold">RANDOM</span>：设置多种轨道随机效果（下文介绍），快捷键是 `鼠标左右键`；

- <span style="color:LawnGreen; font-weight:bold">随机选曲、难度切换</span>：
    - <span style="color:#c0ee93; font-weight:bold">随机选曲</span>：随机抽选当前目录任意曲目；
    - <span style="color:#c0ee93; font-weight:bold">难度切换</span>：手动选择档当前曲目的四个难度 (Easy、Normal、Hard、SHD)。

- <span style="color:red; font-weight:bold">开始演奏、查看回放</span>：
    - <span style="color:yellow; font-weight:bold">黄色图标开始演奏</span>：开始当前选中歌曲及对应谱面的演奏；
    - <span style="color:cyan; font-weight:bold">蓝色图标查看回放</span>：查看当前谱面自己演奏的回放记录列表，快捷键是 `F7`。

- <span style="color:Fuchsia; font-weight:bold">成绩数据显示区</span>：
   - 显示当前谱面自己最佳成绩时的详细数据（以总分最高的一次）。
   - <span style="color:#ff99ff; font-weight:bold">查看排行榜</span>：打开当前谱面的全球排行榜，快捷键是 F8。

### 2. 参数设置面板 - 简要设置面板 :id=guide-bastd-gslite

![简要设置面板](assets/bastd/gslite.png)














