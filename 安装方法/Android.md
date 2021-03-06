# Android

1. 安装同文输入法。具体可以参照 Trime 的 [网站](https://github.com/osfans/trime#同文安卓輸入法平臺trime-rime-ime-for-android)。

2. 安装好之后，打开同文输入法，点击“启用”，再点击“选取”选择同文输入法平台。

3. 点击下方链接，下载输入法文件。

    - [上海](https://codeload.github.com/NGLI/rime-wugniu_zaonhe/zip/master)（包含中派上海、老派上海和松江三种口音）
    - [苏州](https://codeload.github.com/NGLI/rime-wugniu_soutseu/zip/master)
    - [嘉兴](https://codeload.github.com/NGLI/rime-wugniu_kashin/zip/master)（包含桐乡、海宁、海盐、嘉兴、嘉善五种口音）
    - [宁波](https://codeload.github.com/NGLI/rime-wugniu_gninpou/zip/master)（包含宁波和鄞州两种口音）

4. 输入法需要基础配置文件和基础词表，同时也依赖朙月拼音和五筆畫实现反查。点击下方链接下载。

    - [Rime 輸入法基礎配置](https://codeload.github.com/rime/rime-prelude/zip/master)
    - [essay](https://codeload.github.com/rime/rime-essay/zip/master)
    - [朙月拼音](https://codeload.github.com/rime/rime-luna-pinyin/zip/master)
    - [五筆畫](https://codeload.github.com/rime/rime-stroke/zip/master)

5. 解压第 3 步和第 4 步下载好的几个压缩包，找到所有以 `.yaml` 和 `.txt` 结尾的文件，将它们放到安卓设备的 `/sdcard/rime` 文件夹（主目录下的 `rime` 文件夹）。

6. 放好后，再次打开同文输入法。选择“部署”，等待一段时间后，再选择“输入”>“方案”，根据自己的需要勾选输入方案。选完点“确定”。

7. 到打字界面，长按输入法左下角“選單”，在选单中选择输入法。

有需要的话，也可以参阅 Trime 输入法的 [文档](https://github.com/osfans/trime/wiki/UserGuide)。
