# CQXQ
让先驱QQ机器人支持酷Q插件

## 使用方法:
1. 将CQXQ.XQ.dll放入Plugin文件夹
2. 创建CQPlugins文件夹，将CQ插件的dll和json放入
3. 启动机器人，在插件管理启动CQXQ，在CQXQ管理页面配置插件
4. 开始使用

## 如何获取酷Q插件
**联系作者提供DLL和JSON文件**
（或者你可以提供通过CPK解包后的DLL文件让溯洄恢复……（纯粹看溯洄心情））

## 为什么酷Q插件不在XQ插件列表中显示
因为就是不会显示，管理CQ插件请右键CQXQ点设置插件

## 联系开发者:
你可以选择加入开发群 610272090 获取最新资讯（这是开发群，不是你什么都不会然后进去问来问去的群）

## 开发进度：
事件
- [x] 加载
- [x] 退出
- [x] 启用
- [x] 禁用
- [x] 群消息（传入了一个假的消息ID（实际上是一个到某结构体的指针）来实现撤回）
- [x] 私聊消息（好友, 群临时会话, 讨论组临时会话）
- [x] 讨论组消息
- [x] 邀请机器人加入群/其他人被邀请进群/其他人申请进群
- [x] 群成员增加
- [x] 群成员减少
- [x] 群管理变动
- [ ] 群文件上传（XQ似乎未实现）
- [x] 好友已添加
- [x] 禁言/全局禁言

API
- [x] 获取应用目录
- [x] 发送群消息（不支持获取发出消息的消息ID，固定返回1）
- [x] 发送私聊消息（好友, 群临时会话, 讨论组临时会话）（不支持获取发出消息的消息ID，固定返回1）
- [x] 发送讨论组消息（不支持获取发出消息的消息ID，固定返回1）
- [x] 退出群
- [ ] 退出讨论组（XQAPI未找到对应函数）
- [x] 设置好友添加处理
- [x] 设置群邀请处理/有人加群处理
- [x] 设置群名片
- [ ] 设置群管理员（XQAPI未找到对应函数，但是理论上可以用qinfo.clt.qq.com的接口实现）
- [x] 设置群匿名
- [x] 获取陌生人信息（只支持昵称）
- [x] 获取群成员信息（待优化）（只支持昵称，群名片，最后发言时间，入群时间，群等级名称，权限）
- [x] 获取群信息（待优化）
- [x] 获取好友列表（待优化）
- [x] 获取群列表
- [x] 获取群成员列表（只支持每个群成员的昵称，群名片，最后发言时间，入群时间，群等级名称，权限）
- [x] 获取Cookie
- [x] 获取CsrfToken
- [x] 获取图片下载路径
- [x] 获取录音下载路径
- [ ] 设置群成员头衔（XQAPI未找到对应函数）
- [x] 禁言
- [x] 全局禁言
- [ ] 禁言匿名用户（XQAPI未找到对应函数，但是理论上可以用qqweb.qq.com的接口实现）
- [x] 撤回消息（只支持撤回群消息，只支持在群消息事件内部进行撤回）

CQ码
- [x] at
- [x] image(file或者URL)
- [x] record(只支持amr和silk文件)
- [x] face
- [x] emoji(只支持单向从cq码到emoji的转换)
- [ ] 其他

GUI及管理
- [x] 启用/禁用插件
- [ ] 重载插件
- [x] 插件优先级
- [x] 插件菜单
- [ ] 插件权限管理
- [ ] 悬浮窗
- [ ] cpk解析
