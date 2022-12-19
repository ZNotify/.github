# ZNotify

[English](https://github.com/ZNotify/.github/blob/master/profile/README.md) | 中文

ZNotify 是一个允许你在多个平台上向自己发送通知的项目，包括 Web、Android 和 Windows。

ZNotify 目前仍然在开发中。

## 支持的消息服务

- Web Push
- Google Cloud Messaging
- Windows Push Notification Services
- Telegram
- WebSocket[^1]

[^1]: 仅作为后备方案使用，因为它会消耗额外的电池和数据。

## 客户端

- [Web](https://github.com/ZNotify/frontend)[^2]
- [Android](https://github.com/ZNotify/android)
- [Windows](https://github.com/ZNotify/windows)
- [Cli](https://github.com/ZNotify/cli)[^3]
  
[^2]: 网络推送的可用性取决于浏览器。更多信息请参见[Can I Use](https://caniuse.com/push-api)。
[^3]: cli 在大多数平台上都可用，包括 Windows、Linux 和 macOS。如果你没有找到你的平台，你可以自己构建它。

## 基本用法

```bash
curl -X POST -d "This is a message" https://{your-znotify-server}/{user-id}
```

完整的文档请参见[Web API Reference](https://push.learningman.top/docs/index.html)。

ZNotify 没有提供一个公共服务器，但你可以很容易地部署你自己的服务器。更多信息请参见[服务器](https://github.com/ZNotify/server)。

## SDK

ZNotify有针对以下语言的SDK。

- [Python](https://github.com/ZNotify/py-sdk)
- [C#](https://github.com/ZNotify/cs-sdk)
- [Kotlin](https://github.com/ZNotify/kt-sdk)
- [Rust](https://github.com/ZNotify/rs-sdk)

你可以在[swagger.json](https://github.com/ZNotify/server/blob/master/docs/swagger.json)找到生成的 openapi 规范。对于不支持的语言，你可以使用 openapi 规范来生成你自己的SDK。

## 贡献

欢迎贡献! 请提交一个 pull request 或打开一个 issue。


## 许可证

ZNotify 的不同部分在不同的许可下被授权。更多信息请参见每个仓库中的 "LICENSE "文件。