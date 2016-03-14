###vimdiff

原文[连接]:[vimdiff]

####启动命令

    vimdiff FILE_LEFT FILE_RIGHT
or

    vim -d FILE_LEFT FILE_RIGHT
or

    vim FILE_LEFT
    :vertical diffsplit FILE_RIGHT

####差异点跳转

    ]c or [c
ps: 跳转到第二个差异点可以在命令前加上数字2

####文件合并

    dp (diff "put")     // 当前文件中差异内容复制到另一个文件中
    do (diff "get", 之所以不用dg,是因为dg已经被另一个命令占用了)    // 另一个文件中差异内容复制到当前文件中

####刷新比较结果

    :diffupdate



[vimdiff]: https://www.ibm.com/developerworks/cn/linux/l-vimdiff/   "vimdiff link"
