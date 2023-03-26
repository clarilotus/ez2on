## OPTION 系统设置

### 1. <span style="color:red; font-weight:bold">DISPLAY</span> 显示设置

![显示设置](./assets/display.png)

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

### 2. <span style="color:orange; font-weight:bold">AUDIO</span> 音频设置


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

### 3. <span style="color:LawnGreen; font-weight:bold">GAMEPLAY</span> 游戏操作及表现设置

![游戏操作](./assets/game.png)

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

![按键设置](./assets/key.png)

- <span style="color:#b1ee77; font-weight:bold">MODE</span>：切换 **4键~8键** 各个模式以及 **命令操作** 的按键设置；
- <span style="color:#b1ee77; font-weight:bold">KEYBOARD</span>：物理键盘的映射；
- <span style="color:#b1ee77; font-weight:bold">CONTROLLER</span>：控制器（手台）的映射，如果没有连接控制器，则不可用；
- <span style="color:#b1ee77; font-weight:bold">RESET</span>：重置当前键数模式的映射为默认值；
- <span style="color:#b1ee77; font-weight:bold">ASSIST KEY</span>：对于 <span style="color:DeepSkyBlue; font-weight:bold">5键</span> 和 <span style="color:Magenta; font-weight:bold">8键</span> 模式，可设置部分轨道的辅助按键：
    - <span style="color:DeepSkyBlue; font-weight:bold">5键</span> : 可设置 <span style="color:DeepSkyBlue; font-weight:bold">3号轨道 (中间) </span>的辅助按键；
    - <span style="color:Magenta; font-weight:bold">8键</span> : 可设置 <span style="color:Magenta; font-weight:bold">1号轨道 (最左) </span>和 <span style="color:Magenta; font-weight:bold">8号轨道 (最右) </span>的辅助按键。		
    + **注意：需要开启上面的 "ASSIST KEY" 选项才生效！**

#### <span style="color:#9fff41; font-weight:bold">COMMAND KEY</span> 按键设置：命令操作键

![命令操作键](./assets/commandkey.png)

- <span style="color:#b1ee77; font-weight:bold">DECREASE NOTE SPEED</span>：演奏过程中，**减少流速** 的快捷键；
- <span style="color:#b1ee77; font-weight:bold">INCREASE NOTE SPEED</span>：演奏过程中，**增加流速** 的快捷键；
- <span style="color:#b1ee77; font-weight:bold">REDUCE BGA BRIGHTNESS</span>：演奏过程中，**降低背景动画亮度** 的快捷键；
- <span style="color:#b1ee77; font-weight:bold">INCREASE BGA BRIGHTNESS</span>：演奏过程中，**提升背景动画亮度** 的快捷键；
- <span style="color:#b1ee77; font-weight:bold">QUICK RESTART</span>：演奏过程中，**立即重开** 的快捷键；
- <span style="color:#b1ee77; font-weight:bold">HALVE NOTE SPEED</span>：演奏过程中，**将当前流速减半** 的快捷键；
- <span style="color:#b1ee77; font-weight:bold">DOUBLE NOTE SPEED</span>：演奏过程中，**将当前流速翻倍** 的快捷键；
