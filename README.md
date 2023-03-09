# APISpace 介绍
**本 API 服务由 [APISpace（apispace.com）](https://www.apispace.com/?utm_source=github&utm_term=yangmaodun) 提供。**

APISpace 是 Eolink 旗下专业的 API 开放与交易平台，为广大企业以及个人开发者提供多维度、全方位的API接口，覆盖短信验证、天气查询、快递物流、OCR文字识别等海量 API 服务，帮助用户快速获取数据，降低获取数据的成本和难度，提升开发效率。

APISpace 提供15种开发语言的代码示例，分别是：
- Java(OK HTTP)
- HTTP
- cURL
- 微信小程序
- PHP(pecl_http)、PHP(cURL)
- Python(http.client)、Python(Requests)
- JavaScript(Jquery AJAX)、JavaScript(XHR)
- NodeJS(Native)、NodeJS(Request)
- Ruby(Net:Http)
- Shell(Httpie)、Shell(cUrl)

# 反欺诈（羊毛盾）
反机器欺诈，检测异常IP、异常手机号。帮助客户识别大量存在恶意的账号。在金融理财奖励、红包奖励、营销活动等场景下，帮助用户节约大量营销资源，将资源留给真正的用户。

**使用该产品前，您需要通过 [https://www.apispace.com/eolink/api/wool/introduction](https://www.apispace.com/eolink/api/wool/introduction?utm_source=github&utm_term=yangmaodun) 申请API服务**

本文档末尾提供了 Python(Requests) 的调用代码示例，可以前往文档末尾查看。

更多代码示例：[https://www.apispace.com/eolink/api/wool/guidence/](https://www.apispace.com/eolink/api/wool/guidence/?utm_source=github&utm_term=yangmaodun)

### 应用场景

1.  #### 互联网营销推广

在互联网企业推广过程中起到安全防护的作用，可以防止恶意注册、刷单、领用的行为。

2.  #### 数据真实性测评

针对虚假用户体量、虚假活动数量的困扰，帮助投资者做出正确的决策，规避风险，减少损失。

### 应对风险
![image](https://user-images.githubusercontent.com/36323798/223965831-4ea36e2b-d5a3-4db1-a414-10cb51ef0f73.png)


### 数据安全
![image](https://user-images.githubusercontent.com/36323798/223965848-dddb378d-786b-480f-b523-dd2a991e9724.png)


### 服务保障
![image](https://user-images.githubusercontent.com/36323798/223965869-2f6a7421-7f4a-46fe-9bad-7ce2a32d93c4.png)


### Python(Requests) 调用代码示例

```
import requests

url = "https://eolink.o.apispace.com/wool/wcheck"

payload = {"mobile":"","ip":""}

headers = {
    "X-APISpace-Token":"",
    "Authorization-Type":"apikey",
    "Content-Type":"application/x-www-form-urlencoded"
}

response=requests.request("POST", url, data=payload, headers=headers)

print(response.text)

```
