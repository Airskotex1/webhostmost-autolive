# 安装  
文件来源于https://github.com/frankiejun/node-ws 和 https://github.com/eooce/node-ws ，做个人使用  

> **注意：** 记得把命令中的 `yourdomain` 改为你真实的域名,也可以不带参数会自动检测路径/home/$username/domains/下的文件名的第一个，一般情况就是你的域名
```bash 
curl -Ls https://raw.githubusercontent.com/Airskotex1/webhostmost-autolive/main/node-ws/setup.sh > setup.sh && chmod +x setup.sh && ./setup.sh yourdimain
```



# Node-ws说明
用于node环境的玩具和容器，基于node三方ws库，集成哪吒探针服务，可自行添加环境变量
* PaaS 平台设置的环境变量
  | 变量名        | 是否必须 | 默认值 | 备注 |
  | ------------ | ------ | ------ | ------ |
  | UUID         | 否 |0196d2a9-b1c0-708e-b48b-6d7634c7fba9| 开启了哪吒v1,请修改UUID|
  | PORT         | 否 |  3000  |  监听端口                    |
  | NEZHA_SERVER | 否 |        |哪吒v1填写形式：nz.abc.com:8008   哪吒v0填写形式：nz.abc.com|
  | NEZHA_PORT   | 否 |        | 哪吒v1没有此变量，v0的agent端口| 
  | NEZHA_KEY    | 否 |        | 哪吒v1的NZ_CLIENT_SECRET或v0的agent端口 |
  | NAME         | 否 |        | 节点名称前缀，例如：Glitch |
  | DOMAIN       | 是 |        | 项目分配的域名或已反代的域名，不包括https://前缀  |
  | SUB_PATH     | 否 |  webhostmost   | 订阅路径   |
  | AUTO_ACCESS  | 否 |  false | 是否开启自动访问保活,false为关闭,true为开启,需同时填写DOMAIN变量 |

* 域名/webhostmost查看节点信息，也是订阅地址，包含 https:// 或 http:// 前缀，非标端口，域名:端口/webhostmost

    
* 温馨提示：READAME.md为说明文件，请不要上传。
* js混肴地址：https://obfuscator.io

