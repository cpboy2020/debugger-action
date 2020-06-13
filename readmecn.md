动作调试器
GitHub Actions的交互式调试器

用法
steps:
- name: Setup Debug Session
  uses: csexton/debugger-action@master
在操作日志中，您将看到：

Running tmate...

To connect to this session copy-n-paste the following into a terminal:

ssh redactedMxoJ0pXmjredacted@nyc1.tmate.io
只需按照说明进行操作，然后将ssh命令复制到您的终端即可在正在运行的实例之间建立ssh连接。在关闭与正在运行的实例的ssh连接后，该会话将立即关闭。

15分钟后会出现全局超时。这将关闭所有打开的ssh会话。为防止会话终止，请运行：

touch /tmp/keepalive
致谢
tmate.io
马克斯·施密特（Max Schmitt）的动作伴侣
执照
该项目中的操作以及相关的脚本和文档是根据MIT许可证发布的。
