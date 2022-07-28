# API
## 1. 小程序官方把API分为了如下3大类：

1️⃣ 事件监听API

- 特点：以on开头，用来监听某些事件的触发
- 举例：wx.onWindownResize(function callback) 监听窗口尺寸变化的事件
    
2️⃣ 同步API

- 特点1：以Sync结尾的API
- 特点2：同步API的执行结果，可以通过函数的返回值直接获取，如果执行出错会抛出异常
- 特点3：wx.setStorage('key', 'value')向本地存储中写入内容

3️⃣ 异步API

- 特点：类似与jQuery中的，$.ajax(opions)函数，需要通过success， fail， complate 接收调用的结果
- 距离：wx.request()发起的网络数据请求，通过success回调函数接收数据
