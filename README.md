# 王硕 2018310734
# 实验目的
掌握字符串String及其方法的使用

掌握异常处理结构
# 任务
利用已学的字符串处理知识编程完成《长恨歌》古诗的整理对齐工作，达到如下功能：

  每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”

  允许提供输入参数，统计古诗中某个字或词出现的次数

  考虑操作中可能出现的异常，在程序中设计异常处理程序

# 实验核心方法

利用*字符串String*及其方法对古诗做对齐处理

利用*io输出流*将文件输出到txt文件

利用异常处理结构将可能发生的意外排除

### 将诗插入逗号和句号
        StringBuffer poetResult = new StringBuffer();
        for(int i=0; i< poet.length() ; i++)
        {
            poetResult.append(poet.charAt(i));
            if (i%14 == 6){
                poetResult.append("，");
            }else if(i%14 == 13 ){
                poetResult.append("。\n");
            }
        }
#### 代码解释
这部分代码是整段代码中最重要的一部分，他利用七言诗的特点，将七言诗分成两个部分，在模14余6的位置插入逗号，在模14余13的位置插入句号。

# 实验结果
![avatar](https://raw.githubusercontent.com/ws1226395769/wangshuo123/master/%E7%BB%93%E6%9E%9C.png)
![avatar](https://raw.githubusercontent.com/ws1226395769/wangshuo123/master/%E7%BB%93%E6%9E%9C1.png)
![avatar]()
