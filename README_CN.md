# 大语言模型安全

[English](https://github.com/wowtalon/LLM-Security/blob/main/README.md) | [中文版](https://github.com/wowtalon/LLM-Security/blob/main/README_CN.md)


## 总览

**LLM** (大语言模型)应用是指集成了大语言模型的应用，LLM应用存在多种形式，如网页、手机APP、Web API和桌面应用等。本项目旨在介绍大语言模型安全的一些基本概念和防护手段。

## 基础设施安全

### [NVIDIA NIM](https://docs.nvidia.com/nim/large-language-models/latest/introduction.html)

## LLM应用安全

### [Ollama](https://github.com/ollama/ollama)

- CVE-2024-45436
- CVE-2024-39722
- CVE-2024-39721
- CVE-2024-39720
- CVE-2024-39719
- CVE-2024-37032
- CVE-2024-28224
- [More](https://cve.mitre.org/cgi-bin/cvekey.cgi?keyword=ollama)

### [Dify](https://github.com/langgenius/dify)

- [More](https://cve.mitre.org/cgi-bin/cvekey.cgi?keyword=dify)

### [LangChain](https://github.com/langchain-ai/langchain)

- [More](https://cve.mitre.org/cgi-bin/cvekey.cgi?keyword=langchain)

## 模型安全

### 内容安全

#### 提示词安全

- 提示词注入
- 数据泄露
- 更多

### 相关工具

- [AI Infra Guard](https://github.com/Tencent/AI-Infra-Guard)
- [Garak](https://github.com/NVIDIA/garak)

### 合规

#### 输出合规性

- 更多

#### LLM法律法规

- [Safe and Secure Innovation for Frontier Artificial Intelligence Models Act](https://en.wikipedia.org/wiki/Safe_and_Secure_Innovation_for_Frontier_Artificial_Intelligence_Models_Act)
- [Artificial Intelligence Act](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32024R1689)

### [Owasp Top 10 for LLM](https://owasp.org/www-project-top-10-for-large-language-model-applications/)

## 大模型使用安全

即使你不打算开发或部署自己的大模型应用，你也需要注意在日常工作中使用大模型服务时可能产生的风险。打个比方，在使用大模型时上传文件并让大模型对文件进行分析是非常常见的场景，但如果不对员工上传的文件加以限制，就可能导致员工随意上传包含敏感数据的文件到公共大模型服务，进而导致数据泄露。

### 访问控制

防止数据泄露到第三方大模型应用的最有效方法，就是禁止员工使用第三方大模型应用。通常来说*访问控制*是基于域名或应用签名来实现的，比如要禁止员工访问*DeepSeek*，就在防火墙上把*deepseek.com*这个域名封禁掉即可。

以下是一些常见的公共大模型应用：

|应用名称|应用提供商|域名|
|-|-|-|
|DeepSeek|DeepSeek|www.deepseek.com|
|OpenAI|OpenAI|openai.com|
|Kimi|Moonshot AI|kimi.moonshot.cn|
|Doubao|ByteDance|www.doubao.com|
|文心一言|百度|yiyan.baidu.com|
|通义千问|阿里巴巴|tongyi.aliyun.com|
|混元|腾讯|yuanbao.tencent.com|
|盘古|华为|pangu.huaweicloud.com|
|星火|科大讯飞|xinghuo.xfyun.cn|
|商量SenseChat|商汤科技|platform.sensenova.cn|
|百小应|百川智能|ying.baichuan-ai.com|
|智谱清言|智谱华章|chatglm.cn|
|天工AI|昆仑万维|www.tiangong.cn|
|Coze（扣子）|字节跳动|www.coze.cn|

### 数据安全

### 合规
