# react-chat
a web chat tool with react 

这次为了更完美，不断推翻之前的写法(vue-chat的代码用react实现一遍还是挺快)，几个地方暂时没想到更优的实现方式(特别是聊天模块的前后端部分有没有性能更佳的实现方式)，感觉写了也是不满意，先停更一段时间，好好沉淀一番&&研究公司的东西去。

![image](https://user-images.githubusercontent.com/24861316/42560354-0d569eb0-8529-11e8-924f-948bdc786426.png)

![image](https://user-images.githubusercontent.com/24861316/42560447-414e6676-8529-11e8-99c5-97ecf12b3d77.png)

![image](https://user-images.githubusercontent.com/24861316/42560766-09b51858-852a-11e8-9eb0-0a6d78857a5a.png)


目前进度

- [x] 登录
- [x] 注册
- [x] 弹窗，提示等组件
- [x] 响应式布局。以前的实现只是移动端的布局。
- [x] 机器人智能聊天回复
- [x] 聊天页表
- [x] 私聊（外加重要的重构）：始化时请求聊天列表所有聊天对象的聊天记录（后期将请求聊天记录的限制为20条聊天内容，避免初始化时间过长），接着根据点击列表导致chatId(取自url params)的改变，重新渲染新的聊天内容。以前的实现方式是单页面的，点击进入每个聊天页面都会发1至多次请求然后渲染页面，性能较差。。。终于想出自己较为满意的方案，开森~ 不过现在看以前vue-chat的代码真是烂成💩了，搞完react-chat有空了回去重构一波
- [ ] 把后端接口封装成sdk