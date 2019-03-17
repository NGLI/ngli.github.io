# macOS下安装方法

1. 安装Rime输入法。安装和使用方法见Rime输入法的网站https://rime.im/ 。

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

4. 在用户文件夹（`~/Library/Rime/`）内新建文件`default.custom.yaml`，在新建的文件中写入类似下面的语句。

    ```yaml
    patch:
      schema_list:
        - schema: luna_pinyin
        - schema: stroke
        - schema: wugniu_gninpou
        - schema: wugniu_gninyu_tsonkonmiau
    ```

    `-schema: `后面跟输入方案的名称。如果需要其他输入法，可以自行在列表中修改添加。具体可以参照Rime官方的[教程](https://github.com/rime/home/wiki/CustomizationGuide#一例定製方案選單)。

5. 在输入法状态栏上点击“重新部署”。等待一段时间。

6. 按`F4`或`` Ctrl+` ``，从选单中选择想要的输入法。

有需要的话，也可以参阅Rime输入法的[文档](https://rime.im/docs/)。