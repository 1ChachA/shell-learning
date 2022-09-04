shell note
1.shell查看编译器 sudo cat /etc/shells
2.#!/bin/bash 指定编译器
3.echo “your word” 相对于python的print
4.echo $HOME/PWD/SHELL/USER
5. A=1;echo $A; 定义变量并且输出
6.unset A;删除变量
7.readonly  A=1;静态只读变量
8.默认都是string，不能直接计算
9.有空格的内容需要用“或者 ‘引起来
10.export ”变量名字“ 让变量为全局变量
11.$n $1-$9 >10 需要用 ${10} 脚本参数
12.$# 输入变量的个数
13.$* 一次性获取全部变量
14.$@ 获取一个一个变量
15.$? 判断上一条命令有没有正常执行（为0时正常执行）
16.expr A + B 运算符之间有空格（+，-，\*，/，%），` `相当于()
17.$[运算表达式] 或者 $((运算表达式))  比如$[(3+2)*4]
18.判断符[ -e echo.sh ] -ge -le -lt -gt -ne -eq
19.多条件判断 [ 2-ge 3 ] && echo "OK" || echo "FAIL"，&&上一条成功时执行，||相反
20.if [ 条件判断 ];then
  程序
fi
