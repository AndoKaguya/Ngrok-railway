# Ngrok-Railway

利用Ngrok将Railway docker内网穿透做vps使用

## 一、注册 Railway 账号和 Ngrok 账号

1、点击 [Railway](https://railway.app/login?referralCode=JkdRr5) 进入网站注册 Railway 账号，直接使用  github 账号登录即可（需注册满30天）

2、点击 [Ngrok](https://dashboard.ngrok.com/auth) 进入网站，点击下方的 `Sign up for free!` 注册账号

3、再次进入 [Ngrok](https://dashboard.ngrok.com/auth) 复制保存你的 `Authtoken`

ps: Ngrok 的免费账号一个地区只能拥有一个隧道服务，所以想要部署多个项目请修改地区

## 二、部署

点击下方按钮部署

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template?template=https://github.com/buwang-w/Ngrok-railway&envs=NGROK_TOKEN,PORT,REGION&NGROK_TOKENDesc=在Ngrok注册得到的Authtoken&PORTDesc=你需要开放的端口，默认80&PORTDefault=80&REGIONDesc=Ngrok的地区，默认jp，可选us/eu/ap/au/sa/jp/in&REGIONDefault=jp&referralCode=JkdRr5)

默认密码 `akashi520`

`NGROK_TOKEN` 中填入在 `Ngrok` 注册得到的 `Authtoken`

`PORT` 中填入你搭建应用的端口，Railway 会自动将其转发到给你的域名上

`REGION` 中填入隧道所在的[地区代码](https://github.com/buwang-w/Railway-Ngrok/blob/master/README.md#region-地区参数)，距离越近越好（默认jp）

## 三、连接

在[status](https://dashboard.ngrok.com/endpoints/status)查看你的SSH连接 

Windows,macOS,Linux 推荐：[Termius](https://www.termius.com/download)（全平台）[Finalshell](http://www.hostbuf.com/t/988.html) 等

Andriod 推荐：[JuiceSSH](https://play.google.com/store/apps/details?id=com.sonelli.juicessh)（支持中文）termius 等

## 四、其他

### `REGION` 地区参数

- us - 美国（俄亥俄州）
- eu - 欧洲（法兰克福）
- ap - 亚太地区（新加坡）
- au - 澳大利亚（悉尼）
- sa - 南美洲（圣保罗）
- jp - 日本（东京）
- in - 印度（孟买）

