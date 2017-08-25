# blog

vim简介

Vim 是一个具有很多命令的功能非常强大的编辑器。
vim的进入和退出

进入vim编辑器输入：vim文件名<回车>
退出vim 首先按 <ESC>键（这是为了确保您处于正常模式，防止有其他的错误操作）
然后输入： ：q！<回车>键（放弃所有改动）
或者输入： ：wq <回车>键（保存改动）
vim移动命令

h，l，k，j 分别代表左移，右移，上移，下移一个字符，还可配合数字使用，10j 代表下移十行。
vim的删除命令

当前光标删除至下一个单词，输入：dw
当前光标删除至当前行末尾，输入：d$
删除整行，输入：dd
重复一个动作，在他前面加一个数字：2w
移动光标到行首，按数字0键：0
撤销以前的操作，输入：u（小写的u）
撤销在一行中所做的改动，输入：U（大写的U）
撤销以前的撤销命令，恢复以前的操作结果，输入：CTRL-R
其他命令

置入命令：在正常模式下输入p将最后一次删除的内容置入光标之后。
替换命令？：输入r和一个字符替换光标所做位置的字符。
输入s/old/new/g 可以替换 old 为 new。
更改命令：要改变文本知道一个单纯的末尾，输入ce然后添加需要的内容。
打开类命令： 输入 o 将在光标的下方打开新的一行并进入插入模式。
输入大写的 O 可以在光标上方打开新的一行。
附加类命令： 输入 a 将可在光标之后插入文本。
输入大写的 A 可以在光标所在行的行末之后插入文本。
另外一个置换类命令的版本： 输入大写的 R 可连续替换多个字符。
复制粘贴文本：输入v进入可视模式，使用操作符 y 复制文本，使用 p 粘贴文本。
搜索

定位及文件状态：输入 CTRL-G 显示当前编辑文件中当前光标所在行位置以及文
件状态信息。
输入大写 G 则直接跳转到文件中的某一指定行。
搜索类命令： 输入 / 加上一个字符串可以用以在当前文件中查找该字符串。
配对括号的查找： 输入 % 可以查找配对的括号 )、]、}。
文件保存

:w FILENAME 可将当前 VIM 中正在编辑的文件保存到名为 FILENAME 的文
件中。
v motion :w FILENAME 可将当前编辑文件中可视模式下选中的内容保存到文件
FILENAME 中。
:r FILENAME 可提取磁盘文件 FILENAME 并将其插入到当前文件的光标位置
后面。
:r !dir 可以读取 dir 命令的输出并将其放置到当前文件的光标位置后面。

