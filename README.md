【[繁體](https://github.com/NGLI/rime-wugniu#吳語學堂拼音輸入方案合集)】 【[简体](吴语学堂拼音输入方案合集)】

# 吳語學堂拼音輸入方案合集

## 方案列表

- 代碼倉庫：[上海吳語拼音輸入方案](https://github.com/NGLI/rime-wugniu_zaonhe) `wugniu_zaonhe`
    - 上海 `wugniu_zaonhe`
    - 松江 `wugniu_sonkaon`
- 代碼倉庫：[蘇州吳語拼音輸入方案](https://github.com/NGLI/rime-wugniu_soutseu) `wugniu_soutseu`
    - 蘇州 `wugniu_soutseu`
- 代碼倉庫：[嘉興（五縣兩區）吳語拼音輸入方案](https://github.com/NGLI/rime-wugniu_kashin) `wugniu_kashin`
    - 桐鄉 `wugniu_donshian`
    - 海寧 `wugniu_haegnin`
    - 海鹽 `wugniu_haeye`
    - 嘉興 `wugniu_kashin`
    - 嘉善 `wugniu_kazoe`
- 代碼倉庫：[寧波話吳語拼音輸入方案](https://github.com/NGLI/rime-wugniu_gninpou) `wugniu_gninpou`
    - 寧波城區 `wugniu_gninpou`
    - 鄞縣（鍾公廟） `wugniu_gninyu_tsonkonmiau`


## 安裝方法

### Windows

方法一：

1. 安裝Rime輸入法。安裝和使用方法見Rime輸入法的[網站](https://rime.im/)。

2. 右鍵任務欄上的Rime圖標，打開菜單。在菜單中選擇“輸入法設定”，打開設定界面。

3. 在設定界面點擊左下角的“獲取更多輸入法方案...”，會彈出一個命令行界面。在這個命令行中輸入倉庫的地址。比如要安裝寧波話輸入法，就可以輸入
    ```shell
    NGLI/rime-wugniu_gninpou
    ```
    輸入完按下回車，等待一段時間。

    要安裝其他輸入法，只需將`NGLI/rime-wugniu_gninpou`替換爲倉庫地址就可以了。注意是**倉庫地址**不是輸入法的方案名稱。

4. 等到命令行界面不再變化，就可以關掉命令行界面。再回到“輸入法設定”的界面，就可以發現輸入法選單已經有了你需要的那種輸入法。現在可以根據需要勾選。勾選完畢後，點擊“中”，等待一段時間。

5. 按`F4`或`` Ctrl+` ``，從選單中選擇想要的輸入法。

方法二：

1. 安裝Rime輸入法。安裝和使用方法見Rime輸入法的[網站](https://rime.im/)。

2. 到以上各個輸入法的主頁面，點擊“Download”，選擇“Download Zip”下載文件。

3. 解壓下載好的壓縮包，找到以`.yaml`結尾的文件，將它們放到rime輸入法的用戶文件夾。

    Windows下的用戶文件夾是 `%APPDATA%\Rime`。可以通過右鍵任務欄上的Rime圖標來找到用戶文件夾。

4. 放好之後右鍵任務欄上的Rime圖標，打開菜單。在菜單中選擇“輸入法設定”，打開界面。根據自己的需要勾選輸入方案。點擊“中”，等待一段時間。

5. 按`F4`或`` Ctrl+` ``，從選單中選擇想要的輸入法。

視頻教程：https://www.bilibili.com/video/av43252366

### Linux、macOS

1. 安裝Rime輸入法。安裝和使用方法見Rime輸入法的[網站](https://rime.im/)。

2. 在終端內運行以下命令，安裝[東風破](https://github.com/rime/plum)。

    ```shell
    curl -fsSL https://git.io/rime-install | bash
    ```

3. 以安裝寧波話輸入法爲例，運行以下命令，下載輸入法碼錶。

    ```shell
    cd plum
    bash rime-install NGLI/rime-wugniu_gninpou
    ```

    要安裝其他輸入法，只需將`NGLI/rime-wugniu_gninpou`替換爲倉庫地址就可以了。注意是**倉庫地址**不是輸入法的方案名稱。

4. 在用戶文件夾（Linux下爲`~/.config/ibus/rime/`，macOS下爲`~/Library/Rime/`）內新建文件`default.custom.yaml`，在新建的文件中寫入類似下面的語句。

    ```yaml
    patch:
      schema_list:
        - schema: wugniu_gninpou
        - schema: wugniu_gninyu_tsonkonmiau
    ```

    `-schema: `後面跟輸入方案的名稱。如果需要其他輸入法，可以自行在列表中修改添加。具體可以參照Rime官方的[教程](https://github.com/rime/home/wiki/CustomizationGuide#一例定製方案選單)。

5. 在輸入法狀態欄上點擊“部署”（macOS下爲“重新部署”）。等待一段時間。

6. 按`F4`或`` Ctrl+` ``，從選單中選擇想要的輸入法。

### Android

1. 安裝同文輸入法。具體可以參照Trime的[網站](https://github.com/osfans/trime)。

2. 到以上各個輸入法的主頁面，點擊“Download”，選擇“Download Zip”下載文件。

3. 解壓下載好的壓縮包，找到以`.yaml`結尾的文件，將它們放到`/sdcard/rime`文件夾。

4. 放好後，點擊輸入法圖標。選擇“輸入”>“方案”，根據自己的需要勾選輸入方案。選完點“確定”，等待一段時間。

5. 長按輸入法左下角“選單”，在選單中選擇輸入法。

有需要的話，也可以參閱Rime輸入法的[文檔](https://rime.im/docs/)。




# 吴语学堂拼音输入方案合集

## 方案列表

- 代码仓库：[上海吴语拼音输入方案](https://github.com/NGLI/rime-wugniu_zaonhe) `wugniu_zaonhe`
    - 上海 `wugniu_zaonhe`
    - 松江 `wugniu_sonkaon`
- 代码仓库：[苏州吴语拼音输入方案](https://github.com/NGLI/rime-wugniu_soutseu) `wugniu_soutseu`
    - 苏州 `wugniu_soutseu`
- 代码仓库：[嘉兴（五县两区）吴语拼音输入方案](https://github.com/NGLI/rime-wugniu_kashin) `wugniu_kashin`
    - 桐乡 `wugniu_donshian`
    - 海宁 `wugniu_haegnin`
    - 海盐 `wugniu_haeye`
    - 嘉兴 `wugniu_kashin`
    - 嘉善 `wugniu_kazoe`
- 代码仓库：[宁波话吴语拼音输入方案](https://github.com/NGLI/rime-wugniu_gninpou) `wugniu_gninpou`
    - 宁波城区 `wugniu_gninpou`
    - 鄞县（钟公庙） `wugniu_gninyu_tsonkonmiau`

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

