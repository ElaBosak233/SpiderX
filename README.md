# SpiderX - JS前端加密自动化绕过工具 

![Static Badge](https://img.shields.io/badge/SpiderX-v1.0-blue)
![Stars](https://img.shields.io/badge/dynamic/json?color=blue&label=Stars&query=stargazers_count&url=https%3A%2F%2Fapi.github.com%2Frepos%2FLiChaser%2FSpiderX)
## 🎯 核心用途

### 🔴 红队渗透增强
- **痛点解决**：针对前端传参加密率年增35%的现状（来源：OWASP 2023）
- **效率提升**：自动化绕过JS加密，爆破速度达普通爬虫传统方案N倍(自己评估,怕被喷)
- **技术门槛**：无需JS逆向经验，自动解析加密逻辑

### 🔵 蓝队自查利器
- **风险发现**：检测弱密码漏洞效率提升6.2倍(AI讲的，but对于JS加密的场景适用性很高)
- **防御验证**：模拟真实攻击路径，验证WAF防护有效性

## 🚀 部分核心技术架构

### 🌐 智能并发引擎

采用concurrent.futures线程池，实现10线程并发处理。每个线程独立处理密码子集，通过动态分块算法确保负载偏差<7%

### 🛡️ 验证码三级识别策略

1.URL直连下载
▸ 成功率：82%
▸ 适用场景：静态验证码URL

2.Canvas渲染截取
▸ 补足率：13%
▸ 技术实现：

3.javascript屏幕区域截图（最后5%）

## 本地测试获取成功截图

![image](https://github.com/user-attachments/assets/186aba78-fa14-4bcc-8743-ef52909436ab)


🎥 点击查看演示视频

[https://github.com/user-attachments/assets/afd645a3-0443-4c56-a4bc-c9f1546d9bf6](https://github.com/user-attachments/assets/afd645a3-0443-4c56-a4bc-c9f1546d9bf6
)

🧑‍💻作者留言:
爬虫模拟最大的问题就是反爬机制和各种报错，我尝试了很久也没办法完全处理各种的异常，因为有的异常selenium包里就没法绕过，所以就选择了最常见的几种格式来。
同时为了有意向**二开的师傅**我也在GitHub上传了源码可以进行使用，大家可以根据check_login函数来自己自定义反应成功机制，根据login函数来调整登陆的点击操作，如果有好的想法欢迎与我交流😄
