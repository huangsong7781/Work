## 在微信浏览器中调起支付宝（国际）进行支付

How to use AliPay(International) in Wechat Browser ?

### 背景

目前我们的迷衣H5正在接入支付宝国际支付，实现收取国内用户人民币的同时，直接转为港币进入香港公司的账户，

我们的迷衣H5（微信浏览器版）已经接入了微信国际支付。

访问链接：https://me.xyh.io/

### 怎么做？

[业务流程图][https://tokyo.cdn.xiyanghui.com/%E6%94%AF%E4%BB%98%E5%AE%9D%E6%94%AF%E4%BB%98%E4%B8%83%E9%83%A8%E6%9B%B2.jpg]

### 现在遇到了什么问题？What's the problem in this project？

就是在微信内调起Safari，Safari再去调起Alipay App，支付完成后，是无法回到微信了。这个时候我参考其他家的H5，提出了如下解决方案：

* 如果跳回Safari，给一个新页面：支付成功，请您手动返回微信。
* 如果跳回微信，增加了一个按钮，可以让用户返回订单详情，去的是这个订单的订单详情。
* 因为用的人比较少，如果用原生浏览器打开之后是看不到微信登录的(负责H5的工程师完全不懂微信开放平台，他和我说怎么可能在Safari去调微信登录，哈哈哈)。
* 另外，因为微信国际支付原因，非微信浏览器支付时，直接调了支付宝支付，没得选。

### 紧张

最重要的用户用三星S10+老黑屏，然后老板让我把H5给她用，给完之后她的第一句话就是：确实比小程序快很多，然后又提了另一个问题，在微信聊天很容易退出呀(只能靠浮窗解决)，或者靠原生浏览器解决，她用了后者。

然后！我又发现了一些Bug！天，好刺激，最重要的用户真感尝鲜。