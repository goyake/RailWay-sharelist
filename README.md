# 一键部署 [ShareList](https://github.com/reruin/sharelist) 到 railway 

> 首先你得有一个注册时间已经满30天的 github 账户，才能登陆 railway 并白嫖每月 5 美刀的额度，可以先注册一个 github 账户等着，等不及就用其他方式部署 ShareList 。

> railway并不会像其他云服务托管平台那样：部署好的项目一段时间不活跃就休眠，而是持续运行。

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new?template=https%3A%2F%2Fgithub.com%2FChirmyRam%2FRailWay-sharelist)

# 步骤：

* 1. 点击以上按钮进入 railway ，使用 github 账户授权登录，一键部署；


* 2. 在部署好的项目 app 面板左侧，点击 **Variables** ，添加环境变量 **33001** 端口：PORT 33001


![image](https://user-images.githubusercontent.com/34760505/136553624-a19d9556-f4a9-41d9-b251-4ef27fa177c3.png)


* 3. 在 **Deployments** → **Deploys** 里面访问默认域名进行挂载 OneDrive ，在 **Domains** 里面使用CNAME解析自定义域名，在 **Triggers** 里面解绑或换绑 github 仓库，否则仓库内容变动会导致 railway 对应 app 自动重新部署，丢失数据。


![image](https://user-images.githubusercontent.com/34760505/136554404-ebcfa3f4-333d-4e05-b3ad-46fe63b47da6.png)


* 4. 访问 https://railway.app/account/billing 查看账户预估计费，以免超出免费额度。当然挖矿、刷PT等行为会被封号。

