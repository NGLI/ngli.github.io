# 吳語學堂拼音輸入方案合集

## 方案列表

- [上海吳語拼音輸入方案](https://github.com/NGLI/rime-wugniu_zaonhe)
    - 上海 `wugniu_zaonhe`
    - 松江 `wugniu_sonkaon`
- [蘇州吳語拼音輸入方案](https://github.com/NGLI/rime-wugniu_soutseu)
    - 蘇州 `wugniu_sutseu`
- [嘉興（五縣兩區）吳語拼音輸入方案](https://github.com/NGLI/rime-wugniu_kashin)
    - 桐鄉 `wugniu_donshian`
    - 海寧 `wugniu_haegnin`
    - 海鹽 `wugniu_haeye`
    - 嘉興 `wugniu_kashin`
    - 嘉善 `wugniu_kazoe`
- [寧波話吳語拼音輸入方案](https://github.com/NGLI/rime-wugniu_gninpou)
    - 寧波城區 `wugniu_gninpou`
    - 鄞縣（鍾公廟） `wugniu_gninyu_tsonkonmiau`

## 安裝方法

### Windows

方法一：

1. 安装Rime输入法。安装和使用方法见Rime输入法的[网站](https://rime.im/)。

2. 右键任务栏上的Rime图标，打开菜单。在菜单中选择“輸入法設定”，打开设定界面。

3. 在设定界面点击左下角的“獲取更多輸入法方案...”，会弹出一个命令行界面。在这个命令行中输入仓库的地址。比如要安装宁波话输入法，就可以输入
    ```shell
    NGLI/rime-wugniu_gninpou
    ```
    输入完按下回车，等待一段时间。

    要安装其他输入法，只需将`NGLI/rime-wugniu_gninpou`替换为仓库地址就可以了。注意是**仓库地址**不是输入法的方案名称。

4. 等到命令行界面不再变化，就可以关掉命令行界面。再回到“輸入法設定”的界面，就可以发现输入法选单已经有了你需要的那种输入法。现在可以根据需要勾选。勾选完毕后，点击“中”，等待一段时间。

5. 按`F4`或`` Ctrl+` ``，从选单中选择想要的输入法。

方法二：

1. 安装Rime输入法。安装和使用方法见Rime输入法的[网站](https://rime.im/)。

2. 到以上各个输入法的主页面，点击“Download”，选择“Download Zip”下载文件。

3. 解压下载好的压缩包，找到以`.yaml`结尾的文件，将它们放到rime输入法的用户文件夹。

    Windows下的用户文件夹是 `%APPDATA%\Rime`。可以通过右键任务栏上的Rime图标来找到用户文件夹。

4. 放好之后右键任务栏上的Rime图标，打开菜单。在菜单中选择“輸入法設定”，打开界面。根据自己的需要勾选输入方案。点击“中”，等待一段时间。

5. 按`F4`或`` Ctrl+` ``，从选单中选择想要的输入法。

视频教程：https://www.bilibili.com/video/av43252366

### Linux、macOS

1. 安装Rime输入法。安装和使用方法见Rime输入法的[网站](https://rime.im/)。

2. 在终端内运行以下命令，安装[東風破](https://github.com/rime/plum)。

    ```shell
    curl -fsSL https://git.io/rime-install | bash
    ```

3. 以安装宁波话输入法为例，运行以下命令，下载输入法码表。

    ```shell
    cd plum
    bash rime-install NGLI/rime-wugniu_gninpou
    ```

    要安装其他输入法，只需将`NGLI/rime-wugniu_gninpou`替换为仓库地址就可以了。注意是**仓库地址**不是输入法的方案名称。

4. 在用户文件夹（Linux下为`~/.config/ibus/rime/`，macOS下为`~/Library/Rime/`）内新建文件`default.custom.yaml`，在新建的文件中写入类似下面的语句。

    ```yaml
    patch:
      schema_list:
        - schema: wugniu_gninpou
        - schema: wugniu_gninyu_tsonkonmiau
    ```

    `-schema: `后面跟输入方案的名称。如果需要其他输入法，可以自行在列表中修改添加。具体可以参照Rime官方的[教程](https://github.com/rime/home/wiki/CustomizationGuide#一例定製方案選單)。

5. 在输入法状态栏上点击“部署”（macOS下为“重新部署”）。等待一段时间。

6. 按`F4`或`` Ctrl+` ``，从选单中选择想要的输入法。

### Android

1. 安装同文输入法。具体可以参照Trime的[网站](https://github.com/osfans/trime)。

2. 到以上各个输入法的主页面，点击“Download”，选择“Download Zip”下载文件。

3. 解压下载好的压缩包，找到以`.yaml`结尾的文件，将它们放到`/sdcard/rime`文件夹。

4. 放好后，点击输入法图标。选择“输入”>“方案”，根据自己的需要勾选输入方案。选完点“确定”，等待一段时间。

5. 长按输入法左下角“選單”，在选单中选择输入法。

有需要的话，也可以参阅Rime输入法的[文档](https://rime.im/docs/)。

