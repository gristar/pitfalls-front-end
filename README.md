# pitfalls-front-end
那些年，我们一起踩过的前端的坑！

1. 使用了base标签，导致css、javascript等文件都会从服务器获取，给本地调试带来麻烦
2. 跨域登录，导致服务器设置登录成功session失效。
3. 微信不支持 background-size 百分比值，使用 contain 或 cover 或修改图片
4. 绑定了 touchend 事件的元素，在滑动页面时意外触发 touchend 事件，应该给 window 增加一个 touchmove 事件，在事件回调用阻止 touchend 事件触发