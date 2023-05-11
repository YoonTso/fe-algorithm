# 前端算法学习笔记

## 20. 有效的括号

-   如果字符串 s 长度为奇数, 则括号一定不匹配直接返回 false
-   创建一个栈结构 stack
-   遍历字符串 s, 每次遍历得到的字符为 c
    -   如果 c 是左括号则 stack 执行入栈
    -   如果 c 是右括号
        -   匹配则 stack 执行出栈
        -   不匹配返回 false
-   遍历结束后返回值取决于 stack 的长度
    -   length 为 0 为返回 true
    -   否则返回 false;
