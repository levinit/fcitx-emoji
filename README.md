# 介绍

为fcitx提供常用的表情符号。

fcitx：

> fcitx(Flexible Input Method Framework) ──即小企鹅输入法，它是一个以 GPL 方式发布的[输入法](https://en.wikipedia.org/wiki/Input_method)平台(即原来的 G 五笔)，包括五笔、拼音(全拼和双拼)、二笔、区位等输入模块，支持简入繁出，是在 Linux 操作系统中常用的中文输入法。它的优点是，短小精悍、跟程序的兼容性比较好。

# 使用方法

- 安装方法--任选一种

  - 下载QuickPhrase.mb文件，将其放置到~/.config/fcitx/data目录下。

    如果~/.config/fcitx/data/QuickPhrase.mb中已有内容，可将下载的QuickPhrase.mb的内容与之合并。

  - 终端执行以下命令（不会覆盖已有内容）：

    ```shell
    curl -#C - -O https://raw.githubusercontent.com/levinit/fcitx-emoji/master/QuickPhrase.mb && cat ./QuickPhrase.mb >> ~/.config/fcitx/data/QuickPhrase.mb && rm ./QuickPhrase.mb
    ```

- 表情使用：fcitx激活状态下，按下分号`;`（默认的按键），然后输入表情的名字，例如😂名为xiaoku（笑哭），请看慢速演示：

  ![示例](./example.gif)

# 表情名字

查看/添加/编辑/删除表情名：可打开QuickPhrase.mb进行相关操作；或者打开fcitx设置-附加组件-快速输入-快速输入列表。

起名很麻烦……按照中文习惯命名酌情命名，参考了常用社交软件的表情名字。如果你有更为合适的命名方式，请提交issue。

# 相关

- unicode表情符号：https://apps.timwhitlock.info/emoji/tables/unicode#block-1-emoticons

- 一些颜文字：[rainlime/fcitx-quick-phrase-emoji](https://github.com/rainlime/fcitx-quick-phrase-emoji)

  可以将其内容后和本项目提供的表情合并到一起（放到QuickPhrase.mb文件中）使用