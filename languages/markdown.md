# 区块元素

## 标题
    ## 这是H2
    ### 这是H3
    ####### 这是H6
## 区块引用
    > 这是引用的部分
    > 另一部分
    > 结尾
可以在整个段落的第一行加上 **>**
    > 我是一整个段落的第一行
    第二行
    第三行
    > 其他引用段落的第一行
    第二行
    第三行
嵌套引用，根据层次加上不同数量的 **>**
    > This is first level of quoting
    >
    > > This is nested block quote.
    >
    > Back to the first level
引用区块内可以使用其他 Markdown 的语法，包括标题，列表，代码区块等：
    > ## This is a title
    >
    > 1.   这是第一行列表
    > 2.   这是第二行列表
    >
    > 代码区块例子
    >
    >    echo "Hello, world!";
## 列表
无序列表可以使用*, +, -
    *   Red
        something for red

        多个段落时，每个项目必须缩进4个空格或一个制表符
    *   Green
    *   Blue
有序列表
    1. First
    2. Second
    3. Three
ps: 需要注意的一些：
1.  列表项间用空行隔开，在输出HTML时将项目内容用<p>标签包起来
2.  列表中放引用，需要缩进
3.  列表中放代码区块，要缩进两次，也就是8个空格或2个制表符
4.  首行出现 **数字-句点-空白** 时，用 **\\.** 来取消列表

## 代码区块
只要简单的缩进4个空格或一个制表符

## 分割线
在一行使用三个以上的*, -, _ 来建立一个分隔线，行内不能有其他东西，星号或减号中间可以插入空格

    * * *
    ***
    *****
    - - -
    ____________

# 区段元素

## 链接
Markdown支持两种链接语法：行内式和参考式
行内式
    This is [an example](http://example.com "Title") inline link
参考式
    This is [an example][id] reference-style link.
    [id]: http://example.com "optional Title here"
链接内容格式：
*   方括号（前面可以选择性地加上至多三个空格来缩进），里面输入id
*   接着一个冒号
*   接着一个以上的空格或制表符
*   接着链接的网址
*   选择性地接着 title 内容，可以用单引号、双引号或是括弧包着
*   链接网址也可以用尖括号包起来
        [id]: <http://example.com/>  "Optional Title Here"
*   可以把 title 属性放到下一行，也可以加一些缩进，若网址太长的话
        [id]: http://example.com/longish/path/to/resource/here
            "Optional Title Here"
*   隐式链接标记
        [Google][]
        [Google]: http://www.google.com
## 强调
使用星号(\*)或底线(\_)

## 代码
Use the `printf()` function  
``There is a literal backtick (`) here.``

## 图片
雷同链接，前面多一个感叹号

## 自动链接
用尖括号包起来，网址的链接文字和链接地址一样  
<http://example.com>
