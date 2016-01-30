#w3m浏览器

w3m是一个基于文本的网页浏览器，支持多种操作系统，在命令行终端可以很好的支持中文。即使在没有鼠标支持的情况下也可以检查网页的输出。本文列出常用的快捷键。

##安装
在大多数的linux发行版本中并不默认包含w3m浏览器，需要我们手动安装，我们需要2个包，w3m和w3m-img，w3m-img包支持在w3m浏览器中显示图片，在ubuntu下使用apt-get install 安装。
```
sudo apt-get install w3m w3m-img
```

##使用
```
w3m www.plusdo.com
```

##常用快捷键

```
H    显示帮助 （大写使用shift+字母）
q    退出，会有提示的  
j,k,l,h  移动光标，就像vim中一样
J/K   向下/向上滚屏  
</>   左右滚屏  
Enter 输入，将光标移动到输入框后，按下Enter会提示TEXT:然后就可以输入了。  
T     打开一个新标签页  
Esc-t 打开所有标签页，供你选择，使用jk来上下移动  
{/}   在标签页中切换  
U     输入新的网址  
B     后退  
Ctrl+q 关闭当前标签页  
/     向后查找当前页  
?     向前查找当前页
```

##详细的操作说明

###页面操作
```
 SPC,C-v 向下翻页
 b,ESC v 向上翻页
 l,C-f 焦点向右
 h,C-b 焦点向左
 j,C-n 焦点向下
 k,C-p 焦点向上
 J 向下滚动一行
 K 向上滚动一行
 ^,C-a 到行首
 $,C-e 到行尾
 w 到下一个单词
 W 到上一个单词
 &gt; 右移一屏
 &lt; 左移一屏
 . 屏幕右移一列
 , 屏幕左移一列
 g,M-&lt; 到首行
 G,M-&gt; 到末行
 ESC g 到指定行
 Z 当前行居中
 z 当前列居中
 TAB 转到下个超链接
 C-u,ESC TAB 到上个超链接
 [ 到第一个超链接
 ] 到最後一个超链接
```

###超链接操作
```
 RET 打开超链接
 a, ESC RET 链接另存为
 u 查看链接url
 i 查看图片url
 I 查看图片
 ESC I 图片另存为
 : 标记rul字符串为锚点
 ESC&nbsp;: 标记ID串为锚点
 c 查看当前页面的URL
 = 显示当前页面属性
 C-g 查看当前行号
 C-h 查看历史记录
 F 提交表单
 M 用外部浏览器打开当前页面 (use 2M and 3M to invoke second and third browser)
 ESC M 用外部浏览器打开链接 (use 2ESC M and 3ESC M to invoke second and third browser
```

###文件/流 操作
```
 U 打开URL
 V 打开文件
 @ 执行外部命令并导入
 # 执行外部命令并浏览
```

###缓存操作
```
 B 返回
 v 查看源代码
 s 选择缓存
 E 编辑缓存代码
 C-l 重画屏幕
 R 刷新
 S 页面另存为
 ESC s 源码另存为
 ESC e 编辑图片
```
###缓存选择模式（也就是按了s以后）
```
 k, C-p 上一缓存
 j, C-n 下一缓存
 D 删除当前缓存
 RET 转至选择的缓存
```

###书签操作
```
 ESC b 打开书签
 ESC a 添加当前页到书签
```

###搜索
```
 /,C-s 向前搜索
 ?,C-r 向後搜索
 n 下一个
 N 上一个
 C-w 打开/关闭 循环搜索
```

###标记
```
 C-SPC 设定/取消 标记（好像这个键一般被输入法占用了）
 ESC p 转至上一标记
 ESC n 转至下一标记
 " 使用正则表达式标记
```

###杂项
```
 ! 执行外部命令
 H 帮助
 o 设置选项
 C-k 显示接受到的cookie
 C-c 终止
 C-z 挂起（输入jobs命令可以列出被停止运行的进程及编号， 运行命令bg %进程编号可将进程转为后台运行， fg %进程号将进程转向前台进行）
 q 退出（需确认）
 Q 退出而不确认
```

###行编辑模式
```
 C-f 光标向後
 C-b 光标向前
 C-h 删除前一字符
 C-d 删除当前字符
 C-k 删除光标後所有内容
 C-u 删除光标前所有内容
 C-a 光标到行首
 C-e 光标到行尾
 C-p 取得历史记录中的前一个词
 C-n 取得历史记录中的後一个词
 TAB,SPC 自动完成文件名
 RETURN 确定
```

转载至http://wiki.ubuntu.org.cn/W3