# 介绍

fcitx中使用的的**常用**表情符号中文拼音版。

(常用常用常用！个人喜好……如果你有相关想法可发起讨论或推送请求（比如增加符号，增加或变更命名）。)

---

缘何？

有时候需要输入符号，但是：

fcitx输入法自带的表情名都是英文的，而且以两个`:`包含住的，例如🌹（玫瑰rose），按下`;`后，输入`:rose:`即可打出玫瑰的图标（更多内置图标名字见**fcitx设置-附加组件-快速输入-快速输入列表-快速输入编辑器**）。

一方面，这种输入较麻烦，要输入一个`:`开头；另一方面，这显然这不太符合天朝人士的~~脑回路~~需求，难道你看到这个表情的快速反应不是“笑哭”😂？至少和笑或哭相关吧。（~~`joy`什么的还得切换一下大脑中的中英文翻译插件~~ ）

所以本项目中表情符号对应的名字均不使用前的引号，略微提升输入的便捷性；把常用表情符号名字**本土化**（参看[命名](#命名)），以符合先进文化的前进方向。（不过这个按音命名的方法也许还是恐怕应该不会太适合形码用户的习惯吧？）



一点微小的工作，谢谢大家。🐸

# 安装

- 任选一种

  - 终端执行以下命令（不会覆盖已有内容）：

    ```shell
    curl -#C - -O https://raw.githubusercontent.com/levinit/fcitx-emoji/master/QuickPhrase.mb && cat ./QuickPhrase.mb >> ~/.config/fcitx/data/QuickPhrase.mb && rm ./QuickPhrase.mb
    ```

- 将项目中的**QuickPhrase.mb**文件放置到`~/.config/fcitx/data`目录下。

  如果`~/.config/fcitx/data/QuickPhrase.mb`中已有内容，可将下载的**QuickPhrase.mb**的内容与之合并。

# 使用

fcitx的输入法激活状态下（即非区域“键盘”模式下，就是能打汉字的那个状态）

1. **按下分号**`;`（默认的按键是分号，也可在fcitx设置-附加组件-快速输入中修改）

2. **输入表情的名字**即可看到提示，按需选用即可（和普通打字一样）

   例如😂名为xiaoku（笑哭）演示：

![示例](./example.gif)

# 命名

- 参考天朝网络社交工具及中文交流习惯酌情命名。

- 为了方便使用的时候较为容易找到相关的符号，同一个表情符号（也可能是几个看起来很类似的表情）会给出多个命名。

  比如😅命名了`daxiao`（大笑）、`gaoxing`（高兴）、`haha`（哈哈）等等

  - 某些在使用上比较专业化的符号，可能还增加有英文命名。

    如©（版权），命名有`banquan`和`copyright`。

  - 某些符号可能只有英文名称（谁让英文如此强势）

    如🆚命名为`vs`

- 查看/添加/编辑/删除符号：

  - 打开QuickPhrase.mb进行相关操作。
  - 打开**fcitx设置-附加组件-快速输入-快速输入列表-快速输入编辑器**中进行相关操作。

# 相关

- unicode表情符号：https://apps.timwhitlock.info/emoji/tables/unicode#block-1-emoticons

- 一些颜文字：[rainlime/fcitx-quick-phrase-emoji](https://github.com/rainlime/fcitx-quick-phrase-emoji)

  可以将其内容后和本项目提供的表情合并到一起（放到QuickPhrase.mb文件中）使用
