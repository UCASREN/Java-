### 什么是异步请求`AsyncContext`
>servlet2.5中，页面发送一次请求，是顺序执行，即使在servlet里的service中开启一个线程，线程处理后的结果是无法返回给页面的，因为servlet执行完毕后，response就关闭了，无法将后台更新数据即时更新到页面端。要实时推送，采用定时发送请求、Ajax 轮询、反向Ajax(Comnet)。在servlet3.0中提供了异步支持，当数据返回页面后，request并没有关闭，当服务器端有数据更新时，就可以推送了。
