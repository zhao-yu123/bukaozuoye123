# bukaozuoye123
# 赵雨 2018310766
# 实验目的
掌握字符串String及其方法的使用
掌握异常处理结构
任务
利用已学的字符串处理知识编程完成《长恨歌》古诗的整理对齐工作，达到如下功能：
每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”
允许提供输入参数，统计古诗中某个字或词出现的次数
考虑操作中可能出现的异常，在程序中设计异常处理程序
# 实验核心方法
利用字符串String及其方法对古诗做对齐处理
利用io输出流将文件输出到txt文件
利用异常处理结构将可能发生的意外排除
## 将诗插入逗号和句号
StringBuffer poetBuffer = new StringBuffer("");
        List<String> list = new ArrayList();

        for (int i = 0; i < (poet.length()); i= i+7) {
            list.add(poet.substring(i, i+ 7));
        }
        for(int i=0 ; i < list.size(); i++){
            System.out.println(list.get(i));
            poetBuffer.append(list.get(i));
            if(i %2 == 0){
                poetBuffer.append("，");
            }else{
                poetBuffer.append("。\n");
            }
        }
## 代码解释
这部分代码是整段代码中最重要的一部分，我利用七言诗的特点，将七言诗
先按照7个字符截取出来存到列表里，然后再拼接出结果，奇数句加逗号，偶数句加句号。
# 异常处理
有时候我们处理的字符串包含多余的逗号句号，所以我加入了异常处理，如果含有句号逗号将报错。
# 实验收获
我不会将结果输入txt文件中的实现，于是我在网上看了很多代码，还是有一些问题，无奈的我最终在java书里寻找到了结果，这个代码是通用的，所以我记住了，以后可以照搬，通过此次实验，我进一步熟悉了java以及string的用法还有列表对于字符串的一些应用。
# 实验结果
