# Webhostmost部署 node-ws 项目教程： (https://banfeng.us.kg/archives/53.html)
仓库来源于https://github.com/banfeng-git/Webhostmost-ws-nodejs进行修改

1. 添加自定义域并申请证书，将项目中的 app.js 和 package.json 上传到public_html目录下即可

2. 下一步回到面板点击左栏 Website Management➡NodeJs APP➡Create application➡CREATE先看图

Node.js version➡22.13.0
Node.js 版本 22.13.0

Application root➡domains/xxx.xxxx.com/public_html (替换自己的完整域名)切记不要填写错误
应用程序根，例如domains/vmq.mqyzf.dedyn.io/public_html

Application startup file➡app.js
应用程序启动文件 app.js

点击Add variable添加环境变量
DOMAIN➡你的域名
PORT ➡端口（自己随便填写别人没用过的端口）
UUID➡生成的uuid

NEZHA_SERVER➡哪吒探针地址（没有可以不填）
NEZHA_PORT ➡哪吒探针端口（没有可以不填）
NEZHA_KEY➡哪吒探针密钥（没有可以不填）

3. 此时创建完成 Node.js 应用后往下翻点击Run NPM install等待执行完毕

等待完毕后点击 Run JS script弹出界面后点击start再点击Run JS script即可

这时输入你的域名 /sub 即可获取节点如xxxx.xom/sub 并访问得到类似于dmxlc3M6Ly9iMmU3ODcwYi1mZGE1LTQzMGQtYmNhMC00ZjNmYTdlZjIwM2NAdnAuemhpeXUudXMua2c6NDQzP2VuY3J5cHRpb249bm9uZSZzZWN1cml0eT10bHMmc这样的将他导入到v2中在设置一下跳过脸书认证就可以了
如果访问是503请更换端口或检查有无错误换端口请重新点击Run JS script

这个节点只支持v2ray使用，并跳过证书验证true才能直连，不支持优选ip
