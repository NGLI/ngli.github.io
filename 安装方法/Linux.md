# Linux下安装方法

### 方法一

1. 安装 Rime 输入法。安装和使用方法见 Rime 输入法的网站 https://rime.im/ 。

2. 在终端内运行以下命令，安装 [東風破](https://github.com/rime/plum)（需要先安装 [git](https://git-scm.com/)）。

    ```shell
    curl -fsSL https://git.io/rime-install | bash
    ```

3. 以安装宁波话输入法为例，运行以下命令，下载输入法码表。

    ```shell
    cd plum
    bash rime-install NGLI/rime-wugniu_gninpou
    ```

    要安装其他输入法，只需将 `NGLI/rime-wugniu_gninpou` 替换为仓库地址就可以了。注意是**仓库地址**不是输入法的方案名称。

4. 点击 [此处](https://github.com/shinzoqchiuq/ngli-default.custom.yaml/archive/refs/heads/main.zip) 下载压缩包，解压后可得配置文件 `default.custom.yaml`，将它放到 Rime 的用户文件夹（`~/.config/ibus/rime/`）内。打开文件，应当显示为如下内容。

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

    `-schema: ` 后面跟输入方案的名称。不需要某种输入法，就将那一行删去，只保留需要的。如果需要更多的输入法，也可以自行在列表中修改添加。具体可以参照Rime官方的 [教程](https://github.com/rime/home/wiki/CustomizationGuide#一例定製方案選單)。

5. 在输入法状态栏上点击“部署”。等待一段时间。

6. 按`F4`或`` Ctrl+` ``，从选单中选择想要的输入法。

### 方法二

1. 安装Rime输入法。安装和使用方法见 Rime 输入法的网站 https://rime.im/ 。

2. 点击下方链接，下载输入法文件。

    - [上海](https://codeload.github.com/NGLI/rime-wugniu_zaonhe/zip/master)（包含中派上海、老派上海和松江三种口音）
    - [苏州](https://codeload.github.com/NGLI/rime-wugniu_soutseu/zip/master)
    - [嘉兴](https://codeload.github.com/NGLI/rime-wugniu_kashin/zip/master)（包含桐乡、海宁、海盐、嘉兴、嘉善五种口音）
    - [宁波](https://codeload.github.com/NGLI/rime-wugniu_gninpou/zip/master)（包含宁波和鄞州两种口音）

3. 点击 [此处](https://github.com/shinzoqchiuq/ngli-default.custom.yaml/archive/refs/heads/main.zip) 下载压缩包，解压后可得配置文件 `default.custom.yaml`，将上一步下载的输入法文件和这一步下载的配置文件放到 Rime 的用户文件夹（`~/.config/ibus/rime/`）内。

4. 打开配置文件 `default.custom.yaml`，应当显示为如下内容。

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

    `-schema: ` 后面跟输入方案的名称。不需要某种输入法，就将那一行删去。如果需要更多的输入法，也可以自行在列表中修改添加。具体可以参照Rime官方的 [教程](https://github.com/rime/home/wiki/CustomizationGuide#一例定製方案選單)。

5. 在输入法状态栏上点击“部署”。等待一段时间。

6. 按`F4`或`` Ctrl+` ``，从选单中选择想要的输入法。

有需要的话，也可以参阅 Rime 输入法的 [文档](https://rime.im/docs/)。
