# Android

安卓平台下，有两个输入法应用可供选择，分别是 [同文输入法（Trime）](https://github.com/osfans/trime) 和 [小企鹅输入法（fcitx5-android）](https://github.com/fcitx5-android/fcitx5-android)。在安装前，先要下载一些文件。

1. 点击下方链接，下载输入方案文件。

    - [上海](https://codeload.github.com/NGLI/rime-wugniu_zaonhe/zip/master)（包含中派上海、老派上海和松江三种口音）
    - [苏州](https://codeload.github.com/NGLI/rime-wugniu_soutseu/zip/master)
    - [嘉兴](https://codeload.github.com/NGLI/rime-wugniu_kashin/zip/master)（包含桐乡、海宁、海盐、嘉兴、嘉善五种口音）
    - [宁波](https://codeload.github.com/NGLI/rime-wugniu_gninpou/zip/master)（包含宁波和鄞州两种口音）

2. 解压下载好的压缩包，找到以 `.yaml` 结尾的输入方案文件。

## 同文输入法

1. 安装同文输入法。具体可以参照 Trime 的 [网站](https://github.com/osfans/trime#同文安卓輸入法平臺trime-rime-ime-for-android)。

2. 安装好之后，打开同文输入法，按界面指引启用输入法。

3. 输入法需要基础配置文件和基础词表，同时也依赖朙月拼音和五筆畫实现反查。点击下方链接下载。

    - [Rime 輸入法基礎配置](https://codeload.github.com/rime/rime-prelude/zip/master)
    - [essay](https://codeload.github.com/rime/rime-essay/zip/master)
    - [朙月拼音](https://codeload.github.com/rime/rime-luna-pinyin/zip/master)
    - [五筆畫](https://codeload.github.com/rime/rime-stroke/zip/master)

4. 解压前面下载好的几个压缩包，找到所有以 `.yaml` 和 `.txt` 结尾的文件，将它们放到安卓设备的 `/sdcard/rime` 文件夹（主目录下的 `rime` 文件夹）。

5. 放好后，再次打开同文输入法。选择“部署”，等待一段时间后，再选择“输入”>“方案”，根据自己的需要勾选输入方案。选完点“确定”。

6. 到打字界面，长按输入法左下角“選單”，在选单中选择输入法。

有需要的话，也可以参阅 Trime 输入法的 [文档](https://github.com/osfans/trime/wiki/UserGuide)。

## 小企鹅输入法

1. 安装 [小企鹅输入法](https://f-droid.org/packages/org.fcitx.fcitx5.android)，并安装 [Rime 插件](https://f-droid.org/zh_Hans/packages/org.fcitx.fcitx5.android.plugin.rime/)。

2. 安装好之后，打开小企鹅输入法，按界面指引启用输入法。

3. 在输入法界面，点“输入法”，再点按右下角的加号，添加“中州韵”。

4. 点击 [此处](https://github.com/shinzoqchiuq/ngli-default.custom.yaml/archive/refs/heads/main.zip) 下载压缩包，解压后可得配置文件 `default.custom.yaml`。打开文件，应当显示为如下内容。

    ```yaml
    patch:
    schema_list:
        - schema: wugniu_zaonhe        # 上海
        - schema: wugniu_zaonhe_laupha # 上海（老派）
        - schema: wugniu_sonkaon       # 松江
        - schema: wugniu_soutseu       # 苏州
        - schema: wugniu_donshian      # 桐乡
        - schema: wugniu_haegnin       # 海宁
        - schema: wugniu_haeye         # 海盐
        - schema: wugniu_kashin        # 嘉兴
        - schema: wugniu_kazoe         # 嘉善
        - schema: wugniu_gninpou       # 宁波
        - schema: wugniu_gnincieu      # 鄞州
    ```

    `-schema: ` 后面跟输入方案的名称。不需要某种输入法，就将那一行删去，只保留需要的。如果需要更多的输入法，也可以自行在列表中修改添加。具体可以参照 Rime 官方的 [教程](https://github.com/rime/home/wiki/CustomizationGuide#一例定製方案選單)。

5. 将之前下载的所有以 `.yaml` 结尾的文件，将它们放到安卓设备的 `/sdcard/Android/data/org.fcitx.fcitx5.android/files/data/rime` 文件夹（主目录下的 `Android/data/org.fcitx.fcitx5.android/files/data/rime` 文件夹）。

6. 到打字界面，按键盘下方地球图标，切换到中州韵。点按左上角“>”号，展开选单，点击“…”，点按“<>”图标切换输入方案。

有需要的话，也可以查看小企鹅输入法的 [网站](https://fcitx5-android.github.io/)。

