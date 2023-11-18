# iOS

iOS 平台下，有两个输入法应用可供选择，分别是[「仓」输入法](https://github.com/imfuxiao/Hamster) 和 [iRime 输入法](https://github.com/jimmy54/iRime)。在安装前，先要在电脑上完成一些准备工作。

1. 点击下方链接，下载输入方案文件。

    - [上海](https://codeload.github.com/NGLI/rime-wugniu_zaonhe/zip/master)（包含中派上海、老派上海和松江三种口音）
    - [苏州](https://codeload.github.com/NGLI/rime-wugniu_soutseu/zip/master)
    - [嘉兴](https://codeload.github.com/NGLI/rime-wugniu_kashin/zip/master)（包含桐乡、海宁、海盐、嘉兴、嘉善五种口音）
    - [宁波](https://codeload.github.com/NGLI/rime-wugniu_gninpou/zip/master)（包含宁波和鄞州两种口音）

2. 解压下载好的压缩包，找到以 `.yaml` 结尾的输入方案文件。

3. 点击 [此处](https://github.com/shinzoqchiuq/ngli-default.custom.yaml/archive/refs/heads/main.zip) 下载压缩包，解压后可得配置文件 `default.custom.yaml`。打开文件，应当显示为如下内容。

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

## 「仓」输入法

1. 在苹果应用商店下载安装「仓」输入法。

2. 确保电脑和 iOS 设备处在同一个 WiFi 下。在 iOS 设备上点击「仓」输入法的图标，选择「输入方案上传」>「启动服务」。按照说明在电脑浏览器上输入 iOS 设备上显示的网址。

3. 打开网址后，双击打开 `Rime` 文件夹，点击上传按钮或通过拖拽，将刚才解压得到的输入方案文件以及 `default.custom.yaml` 上传上去。

4. 关闭网页，并在 iOS 设备上点击「停止服务」。在 iOS 设备上选择「RIME」>「重新部署」，等部署完成后，再点击「输入方案设置」，根据自己的需要勾选输入方案。

5. 在 iOS 的「设置」中，选择「通用」>「键盘」，点击「添加新键盘」，将「仓输入法」添加到键盘中。

6. 到打字界面，点击键盘图标，在选单中选择输入法。


## iRime 输入法

1. 在苹果应用商店下载安装 iRime 输入法。

2. 确保电脑和 iOS 设备处在同一个 WiFi 下。在 iOS 设备上点击 iRime 的图标，选择“电脑快传”。按照说明在电脑浏览器上输入 iOS 设备上显示的网址。

3. 打开网址后，在列表内找到 `default.custom.yaml` 点击垃圾桶按钮将它删掉。再点击“上传文件”，将刚才解压得到的输入方案文件以及 `default.custom.yaml` 上传上去。

4. 退出 iOS 设备上“电脑快传”的页面，先点击“部署”，等部署完成后，再点击“选择方案”，根据自己的需要勾选输入方案。

5. 在 iOS 的「设置」中，选择「通用」>「键盘」，点击「添加新键盘」，将「iRime 输入法」添加到键盘中。

6. 到打字界面，点击键盘图标，在选单中选择输入法。
