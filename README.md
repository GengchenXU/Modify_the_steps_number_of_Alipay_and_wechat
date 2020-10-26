# Modify_the_steps_of_Alipay_and_wechat
修改支付宝&微信步数

实现方法
====

手机安装第三方软件乐心健康，注册账号登录，将运动数据同步到微信和支付宝。用 python 脚本远程修改乐心健康当前登录账号的步数即可。

第一步：在手机上安装乐心健康 app。  
![](https://github.com/GengchenXU/Modify_the_steps_of_Alipay_and_wechat/blob/main/picture/1.png)  
安卓版下载地址：[乐心健康安卓版](http://app.mi.com/details?id=gz.lifesense.weidong)  
苹果版下载地址：[乐心健康 iOS 版](https://apps.apple.com/cn/app/id1479525632)

第二步：注册账号登录，并设置登录密码。  
![](https://github.com/GengchenXU/Modify_the_steps_of_Alipay_and_wechat/blob/main/picture/2.png)  
第三步：完成第三方同步，将运动数据同步到微信和支付宝。![](https://github.com/GengchenXU/Modify_the_steps_of_Alipay_and_wechat/blob/main/picture/3.png)  
第四步：运行 python 脚本，修改乐心健康步数。  
![](https://github.com/GengchenXU/Modify_the_steps_of_Alipay_and_wechat/blob/main/picture/4.png)  



程序设定是每天 7 点自动修改步数，在下面脚本对应的位置替换填入乐心健康手机号、乐心健康密码、修改步数 (默认为 60000)，然后运行程序。修改步数推荐设置范围是 30000 至 90000，步数值太大会导致修改不成功。如果想改变第二天自动修改步数的时间，请修改图示位置的 25200，+25200 代表第二天 0 点后加上的秒数，也就是 7x60x60，即 7 小时，根据自己的需要修改即可。如果每天都要修改步数，那么让程序一直保持运行即可。  
注意：运行程序会立刻修改当天的步数，自动修改步数是从程序保持运行的第二天开始。  
![](https://github.com/GengchenXU/Modify_the_steps_of_Alipay_and_wechat/blob/main/picture/5.png)    
![](https://github.com/GengchenXU/Modify_the_steps_of_Alipay_and_wechat/blob/main/picture/6.png)  

