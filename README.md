一步到位的方式，切换DNS配置。
仅支持Mac。



一、使用情景：

部分工作场景需要使用自定义DNS配置，然而自定义DNS针对部分网络、网站会造成加载缓慢甚至无法加载的情况。



二、使用目的：

简化手动打开设置，手动输入DNS、手动保存等的操作，通过shell命令，一步搞定～



三、使用方法：

打开，选择“恢复默认”，或选择“自定义”即可；

仅支持Mac。



四、核心命令：

networksetup -setdnsservers



五、配置说明：

通过“自动操作”打开该app，更改如下代码：

1、确认网络连接方式（Wi-Fi / iPhone USB / Bluetooth PAN / Thunderbolt Bridge / ...）

以Wi-Fi方式连接为例：

networksetup -setdnsservers Wi-Fi 8.8.8.8 1.1.1.1 8.8.4.4 1.0.0.1

修改Wi-Fi后面的DNS配置即可，注意如有多个请用空格符号分割；


2、保存app；



六、功能说明：

1、恢复默认：清空DNS配置，默认使用系统自配DNS；

2、自定义：设置为用户DNS配置；


感谢使用！
