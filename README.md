# 创新实践之WAF
## 项目解读：
WAF（Web Application Firewall）中文名为： Web应用防护系统
* WAF和传统防火墙的区别：  
网络防火墙作为访问控制设备，主要工作在OSI模型三、四层，基于IP报文进行检测。只是对端口做限制，对TCP协议做封堵。不能对HTTP通讯进行输入验证或攻击规则分析。  

  Web应用防火墙是通过执行一系列针对HTTP/HTTPS的安全策略来专门为Web应用提供保护的一款产品。其工作原理：解析HTTP请求（协议解析模块），规则检测（规则模块），做不同的防御动作（动作模块），并将防御过程（日志模块）记录下来。

* WAF的分类：  
硬件WAF、**软件WAF**、代码级WAF(脚本语言实现过滤器模式)
## 实践方向：
利用已有的开源WAF进行源码分析以及二次开发
* 初步资源选择：  
Ubuntu 18  
Nginx（HTTP和反向代理web服务器）  
ModSecurity 3  
Lua
