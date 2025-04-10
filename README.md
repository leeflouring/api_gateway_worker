<h1 align="center">API Hub</h1>

<p align="center">
一个强大的 API 代理服务集合
</p>

## 功能特性

- 支持多种主流 AI API 服务代理:
  - OpenAI 
  - Google Gemini  
  - Claude 
  - Grok 
- 支持其他常用服务:
  - Docker Registry 服务
  - GitHub 
  - Telegram Bot 
- 优雅的 Web UI 界面
- 简单易用的配置方式


## API 端点

各服务的访问端点如下:

- OpenAI API: `/openai/*`
- Gemini API: `/gemini/*`
- Claude API: `/claude/*`
- Grok API: `/grok/*`
- Docker Registry: `/docker/*`
- GitHub API: `/github/*`
- Telegram Bot API: `/telegram/*`

## 开发

### 项目结构

```
.
├── src/
│   ├── worker.js      # 主要业务逻辑
├── package.json
└── README.md
```

### 添加新的 API 服务

在 `API_CONFIGS` 中添加新的配置即可:

```js
{
  "service-name": {
    host: "api.example.com",
    paths: ["/v1/"],
    description: "服务描述",
    logo: "📦"
  }
}
```



## 贡献指南

欢迎提交 Issue 和 Pull Request 来帮助改进项目。

## 联系方式

如有问题，请提交 Issue 或通过以下方式联系:

- GitHub Issues