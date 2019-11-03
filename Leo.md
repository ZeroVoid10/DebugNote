## guibulider运行无显示问题 
## FIXED

- Author: Leopold
- Data: 2019/11/04 Mon

### Bug描述

guibulider生成的.c文件调用CreateFramewin()函数，lcd不显示

### 解决方法

guibuilder中的函数调用不对，生成的.c文件中调用的是GUI_CreateDialogBox();
可goto defination，在其附近找到GUI_ExecDialogBox();

## 针对结构体typedef 
## FIXING

- Author: Leopold
- Data: 2019/11/04 Mon

### Bug描述

大多都遇见过的问题，结构体的typedef无效，必须使用struct xxx

### 解决方法

遇到后使用 struct xxx

## 关于滴答时钟立flag 
## FIXED
- Author: Leopold
- Data: 2019/11/04 Mon

### Bug描述

本人愚笨以及懒惰，在使用滴答当定时器使用时，没有立flag，只是对1ms_cnt对5求余表示5毫秒
例如
while(1)
{
    if(1ms_cnt%5==0)
    {
        //在5ms内会执行多次
    }
}

### 解决方法

老老实实立flag，并在每次flag使用后清零

## CAN有问题的时候一些可能需要检查的地方 
## FIXING

- Author: Leopold
- Data: 2019/11/04 Mon

### Bug描述

因为在使用 全场定位旧板子和新板子的时候，都遇到了can通信方面的问题
所以想整理一下can可能的问题，挺多的。明天问一下其他人汇总着一块写吧
### 解决方法




