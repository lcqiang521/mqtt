# mqtt
基于mqtt协议的即时聊天

代理服务器配置<br>
一、配置MQTT 服务器Mosquitto（以mac为例）<br>
    1.MQTT是IBM开发的一个即时通讯协议。MQTT是面向M2M和物联网的连接协议，采用轻量级发布和订阅消息传输机制。<br>
    2.Mosquitto是一款实现了 MQTT v3.1 协议的开源消息代理软件，提供轻量级的，支持发布/订阅的的消息推送模式，使设备对设备之间的短消息通信简单易用。<br>
二. Mosquitto 安装<br>
    安装命令：控制台直接输入 brew install mosquitto<br>
    你可能需要安装brew、如果brew不支持，请把/usr/local目录权限设置为当前用户<br>
三. mosquitto服务启动命令<br>
    停止服务  brew services stop mosquitto<br>
    启动服务  brew services start mosquitto<br>
    但是我是这样启动的，mosquitto -c /usr/local/etc/mosquitto/mosquitto.conf指定配置文件方便定位问题；<br>
四.配置服务器地址和端口号<br>
    mosquitto 服务器的配置环境文件路径 /usr/local/etc/mosquitto/mosquitto.conf<br>
    
都配置完成后，启动Mosquitto，并python get.py，即可看到结果
