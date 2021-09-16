## 出现We couldn't deploy your app because the source code violates the Salesforce Acceptable Use and External-Facing Services Policy.提示的就不要继续了。

* 使用[xray](https://github.com/XTLS/Xray-core)+caddy同时部署通过ws传输的vmess vless trojan shadowsocks socks等协议  
* 支持tor网络，且可通过自定义网络配置文件启动xray和caddy来按需配置各种功能  
* 支持存储自定义文件,目录及账号密码均为AUUID,客户端务必使用TLS连接 
* 请务必将本项目fork之后把部署地址后面的名字改成自己的，非常重要，切记！！！！
  
[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https://github.com/wwddf/xary-2)  
  
### 服务端
点击上面紫色`Deploy to Heroku`，会跳转到heroku app创建页面，填上app的名字、选择节点、按需修改部分参数和AUUID后点击下面deploy创建app即可开始部署  
如出现错误，可以多尝试几次，待部署完成后页面底部会显示Your app was successfully deployed  
  * 点击Manage App可在Settings下的Config Vars项**查看和重新设置参数**  
  * 点击Open app跳转[欢迎页面](/etc/CADDYIndexPage.md)域名即为heroku分配域名，格式为`appname.herokuapp.com`，用于客户端  
  * 默认协议密码为$UUID，WS路径为$UUID-[vmess|vless|trojan|ss|socks]格式
  
