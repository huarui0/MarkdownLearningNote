<head>
<link rel="stylesheet" type="text/css" href="github.css">
<link rel="stylesheet" type="text/css" href="colors.css">
</head>

# 基础知识
## 参考 - 有用得链接(GitHub)<br>
   * [Basic writing and formatting syntax](https://help.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax)<br>
   * [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)<br>
   * [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)<br>
   * [emoji-cheat-sheet](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md) - 很好的图标，值得用用<br>
   * [Note/GithubEmoji/emoji.md](https://github.com/jingyuexing/Note/blob/master/GithubEmoji/emoji.md) :heavy_check_mark:另一个很好的图标，值得参考<br>
   * [Basic Syntax](https://www.markdownguide.org/basic-syntax/) - The Markdown elements outlined in John Gruber's design document.<br>

## Markdown 语法介绍：
备注：起的文件名扩展名必须是md，就可以用到md的语法组织文档：） <br>  
- 官网参考：  
    ⋅⋅1. [MarkDown - 语法说明](http://www.markdown.cn/)  
    ⋅⋅2. [Markdown Guide](https://www.markdownguide.org/)  
    ⋅⋅3. ![#f03c15](https://placehold.it/15/f03c15/000000?text=+)[GitHub Flavored Markdown Spec](https://github.github.com/gfm/)  
    ⋅⋅4. ![#f03c15](https://placehold.it/15/f03c15/000000?text=+)[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)  
    ⋅⋅5. [Markdown Example - Markdown例子](https://en.wikipedia.org/wiki/Markdown#Example)<br>
    ⋅⋅6. [一个很好的Git做笔记的例子](https://github.com/imhuay)<br>
- 其他参考：  
    ⋅⋅1. [Markdown 语法介绍](https://coding.net/help/doc/project/markdown.html)  
    ⋅⋅2. [Markdown基本语法](https://www.jianshu.com/p/191d1e21f7ed)  
    ⋅⋅3. [掌握这几种 Markdown 语法你就够了](https://learnku.com/laravel/t/621/you-will-be-able-to-master-these-markdown-grammars)
    
   - 标题
   - 列表
   - 强调
       - 斜体：
       - 加粗：
   - 表格
      * 语法说明
         + |、-、:之间的多余空格会被忽略，不影响布局。
         + 默认标题栏居中对齐，内容居左对齐。
         + -:表示内容和标题栏居右对齐，:-表示内容和标题栏居左对齐，:-:表示内容和标题栏居中对齐。
         + 内容和|之间的多余空格会被忽略，每行第一个|和最后一个|可以省略，-的数量至少有一个。
   - 代码的语法说明
      * C 语言代码的语法
       ```c
          // 这里加入代码语句。
       ```
      * 参考：
        - [Markdown code block syntax highlightning is broken for C and C++ #34525](https://github.com/Microsoft/vscode/issues/34525)
   - 链接
       + 参考：
          - [如何实现Github markdown 目录/页内跳转？](https://www.zhihu.com/question/58630229)<br>
          - [该文件用来测试和展示书写README的各种markdown语法。](https://github.com/guodongxiaren/README#%E9%93%BE%E6%8E%A5)<br>
       + 链接外部URL 
          - 
       + 链接内部的URL
       + 文档内的链接和跳转（两种方式实现页内跳转）
          - 1.MarkDown实现
             - a. [使用Markdown语法增加的跳转到“文档开头”的链接](#CPractice) 注：因为标题就是锚点id，这里直接用标题名称了。
          - 2.html标签实现
             - a. 定义一个锚(id)：<span id="jump">跳转到的地方（id设置为jump）</span>
             - b. 使用markdown语法：[点击跳转到:用Html的标签设置的锚点](#beginpoint)  

## 基本的使用
   * 锚点 与 链接
      + 内部链接
         - <span id="beginpoint">这是用Html的标签设置的锚点</span>  
         - [点击跳转到id为jump的锚点](#jump)
* 备注：这个是用html标签做表格的例子。<br>
    <table>
        <tr>
            <th>设备</th>
            <th>设备文件名</th>
            <th>文件描述符</th>
            <th>类型</th>
        </tr>
        <tr>
            <th>键盘</th>
            <th>/dev/stdin</th>
            <th>0</th>
            <th>标准输入</th>
        </tr>
        <tr>
            <th>显示器</th>
            <th>/dev/stdout</th>
            <th>1</th>
            <th>标准输出</th>
        </tr>
        <tr>
            <th>显示器</th>
            <th>/dev/stderr</th>
            <th>2</th>
            <th>标准错误输出</th>
        </tr>
    </table>
# 颜色的使用<br>
   * 方法 1<br>
      + ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `#f03c15`
      + ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) `#c5f015`
      + ![#1589F0](https://placehold.it/15/1589F0/000000?text=+) `#1589F0`
   * approach 2<br>
      + ![](https://placehold.it/60x18/ff0000/000000?text=IMPORTANT!)

      + ![](https://placehold.it/60x18/ff6600/000?text=WARNING!)

      + ![](https://placehold.it/60x18/009955/fff?text=SUCCESS!)

```diff
+ this will be highlighted in green
- this will be highlighted in red
```

In case this may be helpful for someone who just needs to show colors rather than output, as a hackish workaround (and FYI), since Github supports Unicode numeric character references (and HTML entities), you could try colored Unicode symbols, though it depends on the font rendering them in color (as it happens to be appearing for me on Windows 10 and Mac 10.12.5, at least, though on the Mac at least, the up/down-pointing small red triangles don't show in red):

RED APPLE (&#x1F34E;): 🍎  
GREEN APPLE (&#x1F34F;): 🍏  
BLUE HEART (&#x1F499;): 💙  
GREEN HEART (&#x1F49A;): 💚  
YELLOW HEART (&#x1F49B;): 💛  
PURPLE HEART (&#x1F49C;): 💜  
GREEN BOOK (&#x1F4D7;): 📗  
BLUE BOOK (&#x1F4D8;): 📘  
ORANGE BOOK (&#x1F4D9;): 📙  
LARGE RED CIRCLE (&#x1F534;): 🔴  
LARGE BLUE CIRCLE (&#x1F535;): 🔵  
LARGE ORANGE DIAMOND (&#x1F536;): 🔶  
LARGE BLUE DIAMOND (&#x1F537;): 🔷  
SMALL ORANGE DIAMOND (&#x1F538;): 🔸  
SMALL BLUE DIAMOND (&#x1F539;): 🔹  
UP-POINTING RED TRIANGLE (&#x1F53A;): 🔺  
DOWN-POINTING RED TRIANGLE (&#x1F53B;): 🔻  
UP-POINTING SMALL RED TRIANGLE (&#x1F53C;): 🔼  
DOWN-POINTING SMALL RED TRIANGLE (&#x1F53D;): 🔽  

In his beard lived three <span style="color:red">cardinals</span>.

<h6 class="bg-navy">Hello World</h6>

<p class="bg-navy">This paragraph refers to two classes.</p>


<p style="color:DodgerBlue;">Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>

<p style="color:MediumSeaGreen;">Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>


<table cellspacing="5">
<caption>Comparing weather and time zones</caption>
<tr>
<th>Location</th>
<th>Tucson, Arizona</th>
<th>Las Vegas, Nevada</th>
</tr>
<tr>
<th>Weather</th>
<td>Warm to Hot</td>
<td>Warm to Hot</td>
</tr>
<tr>
<th>Time Zone</th>
<td>No Daylight Savings</td>
<td  class="highlight">Mountain Standard Time</td>
</tr>
</table>


```mermaid
graph LR
A[Hard edge] -->B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
```

```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
```


```flow
st=>start: Start
op=>operation: Your Operation
cond=>condition: Yes or No?
e=>end

st->op->cond
cond(yes)->e
cond(no)->op
```


## 文件转换工具 - PanDoc
  * 说明：这个工具可以将文本文件 转换成 PDF 等等，功能似乎很强大。说不定哪天会用得到，收藏先。<br>
  * 参考：[Pandoc   a universal document converter](http://pandoc.org/MANUAL.html#divs-and-spans)

