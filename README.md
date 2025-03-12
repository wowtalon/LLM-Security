# LLM-Security

## Overview

**LLM** (Large Language Model) application is an application built with LLM behind. It has different forms including Website, mobile app, Web API, desktop app, etc. This repository is to introduce basic concepts about LLM and basic approach to enhance LLM security.

## Infrastructure Security

### [NVIDIA NIM](https://docs.nvidia.com/nim/large-language-models/latest/introduction.html)

## LLM Application Security

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

## Model Security

### Content Security

#### Prompt Security

- Prompt Injection
- Data Leakage
- TBD

### Tools

- [AI Infra Guard](https://github.com/Tencent/AI-Infra-Guard)
- [Garak](https://github.com/NVIDIA/garak)

### Compliance

#### Output Compliance

- TBD

#### LLM Regulation

- [Safe and Secure Innovation for Frontier Artificial Intelligence Models Act](https://en.wikipedia.org/wiki/Safe_and_Secure_Innovation_for_Frontier_Artificial_Intelligence_Models_Act)
- [Artificial Intelligence Act](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32024R1689)

### [Owasp Top 10 for LLM](https://owasp.org/www-project-top-10-for-large-language-model-applications/)

## Usage Security

If you are not going deploy or develop your own LLM application, there are also some risks during apdopting LLM service to your daily business. For example, it's very common for user to upload files and ask LLM to do some analysis. Users may upload a file contains confidential information to a public SaaS LLM service, which leads to data leakage.

### Access Control

To prevent your business data from leaking to third party service provider. The easiest way is to block employee from using third party LLM application. Usually, *Access Control* bases on domain/signature. Take *DeepSeek* as an example, you could add `deepseek.com` to blocklist on the firewall to prevent your employee from access *DeepSeek*.

Here are some commonly used LLM application list:

|Application Name|Provider|Domain|
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

### Data Security

### Compliance
