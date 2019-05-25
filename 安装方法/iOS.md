# iOS

1. 至苹果应用商店下载安装iRime输入法。

2. 在电脑上点击下方链接，下载输入法文件。

    - [上海](https://codeload.github.com/NGLI/rime-wugniu_zaonhe/zip/master)（包含上海和松江两种口音）
    - [苏州](https://codeload.github.com/NGLI/rime-wugniu_soutseu/zip/master)
    - [嘉兴](https://codeload.github.com/NGLI/rime-wugniu_kashin/zip/master)（包含桐乡、海宁、海盐、嘉兴、嘉善五种口音）
    - [宁波](https://codeload.github.com/NGLI/rime-wugniu_gninpou/zip/master)（包含宁波城区和鄞县（钟公庙）两种口音）

3. 解压下载好的压缩包，找到以`.yaml`结尾的输入法文件。

4. 点击[此处](https://gist.github.com/shinzoqchiuq/ddeb5014026fce768f7c9ec7d4e01655/archive/ab0d24e10f6ceb1f0797b516cbcbe17f73425d1e.zip)下载压缩包，解压后可得配置文件`default.custom.yaml`。打开文件，应当显示为如下内容。

    ```yaml
    patch:
      schema_list:
        - schema: wugniu_zaonhe             # 上海
        - schema: wugniu_sonkaon            # 松江
        - schema: wugniu_soutseu            # 苏州
        - schema: wugniu_donshian           # 桐乡
        - schema: wugniu_haegnin            # 海宁
        - schema: wugniu_haeye              # 海盐
        - schema: wugniu_kashin             # 嘉兴
        - schema: wugniu_kazoe              # 嘉善
        - schema: wugniu_gninpou            # 宁波
        - schema: wugniu_gninyu_tsonkonmiau # 鄞县（钟公庙）
    ```

    `-schema: `后面跟输入方案的名称。不需要某种输入法，就将那一行删去，只保留需要的。如果需要更多的输入法，也可以自行在列表中修改添加。具体可以参照Rime官方的[教程](https://github.com/rime/home/wiki/CustomizationGuide#一例定製方案選單)。

5. 确保电脑和iOS处在同一个WiFi下。在iOS设备上点击iRime的图标，选择“电脑快传”。按照说明在电脑浏览器上输入iOS设备上显示的网址。

6. 打开网址后，在列表内找到`default.custom.yaml`点击垃圾桶按钮将它删掉。再点击“上传文件”，将刚才解压得到的输入法文件以及第4步新建的`default.custom.yaml`上传上去。

7. 退出iOS设备上“电脑快传”的页面，先点击“部署”，等部署完成后，再点击“选择方案”，根据自己的需要勾选输入方案。

8. 到打字界面，点击键盘图标，在选单中选择输入法。
