# EFZ_recite_word-in-Windows

## 练习方式

鼠标左键双击运行 `word_win.exe` 来启动。

根据给出的提示（包括首字母、词性与释义），直接完整写出该词然后换行。  
程序会对你的答案进行判定，若正确则绿字重复一遍，若错误则红字标出并绿字标示正确答案  
提示上一行白字为当前进度，判词状态后红字代表错误率，绿字代表正确率。

练习结束后，可查看得分（正确率）与用时。  
特别的，全对的正确率会显示为 `101.0000%` 而非 `100.0000%`。

### 防手误机制

键盘上打字容易出现各种意外。  
如果你的答案到标准答案的修改可以通过增加/删除/修改一个字符或交换相邻两个字符的修改来完成，
那么将会将单词标黄给第二次输入的机会。  
给机会时如果并非手误而确实是拼写错误，建议直接按换行来将此词计入订正。

### 中途退出存档机制

输入 `:wq`（请注意全半角）可退出并保存当前错题，并保存当前进度于 `savefile.txt`。进度可以多次中断。  
注意：新生成的错题本和进度都是保存内容的一部分，如果修改错题本的文件名或内容可能会导致未知错误。

## 词库相关

订正之前某次练习或订正直接输入其文件名（不含.txt 后缀）。  
之后可能会发布别的词库，加入文件夹即可类似地使用。

### 文件名格式

以下的 n,m 都代指数字：

- `BnUmWords`: Book n Unit m Words
- `GnME`: Grade n Midterm Exam
- `GnFE`: Grade n Final Exam
- `GnMmE`: Grade n Month m Exam

订正文件名格式：`correctionyyyyMMDDHHmm`。  
订正文件名的时间指“最开始一次输入文件名的时间”。

## 特性

### 默认 `yes`

任何需要输入 `yes/no` 的地方输入任何不是 `no` 的字符串都会被认为是输入 `yes`。

### 只计末次

中途退出会导致当前累计用时清零。

### 空格不敏感

你可以在输入单词时任意加入空格，它们在与答案比对时会被全部去除。

## 鸣谢

2608xyf：灵感来源&初版程序

2712zy：部分词库整理

作者：2711ltd
