# From ZohyCao

受他人启发，记录一些队内相关的学习笔记，先分享一份别人的学习笔记吧，内容来源于知乎
> [ STM32学习笔记 ](https://zhuanlan.zhihu.com/p/64348776)


## vscode下markdown的snippets配置 FIXED

- Author: ZohyCao
- Data: 2019/10/22 周二

### Bug描述
vscode配置了markdown的snippets后无法使用

### 解决方法

在用户配置中添加如下配置：
> "[markdown]": {
    "editor.formatOnSave": true,
    "editor.renderWhitespace": "all",
    "editor.quickSuggestions": {
        "other": true,
        "comments": true,
        "strings": true
    },
    "editor.acceptSuggestionOnEnter": "on"
}

