# ZNotify

English | [中文](https://github.com/ZNotify/.github/blob/master/profile/README.zh.md)

ZNotify is a project that allows you to send notifications to yourself across multiple platforms, including the Web, Android, and Windows.

ZNotify is currently in development.

## Messaging Services Supported

- Web Push
- Google Cloud Messaging
- Windows Push Notification Services
- Telegram
- WebSocket[^1]

[^1]: Only use as a fallback, as it consumes additional battery and data.

## Client

- [Web](https://github.com/ZNotify/frontend)[^2]
- [Android](https://github.com/ZNotify/android)
- [Windows](https://github.com/ZNotify/windows)
- [Cli](https://github.com/ZNotify/cli)[^3]
  
[^2]: The web push availability depends on the browser. See [Can I Use](https://caniuse.com/push-api) for more information.
[^3]: cli is available on most of the platforms, including Windows, Linux, and macOS. If you didn't find your platform, you can build it yourself.

## Basic Usage

```bash
curl -X POST -d "This is a message" https://{your-znotify-server}/{user-id}
```

For full documentation, see the [Web API Reference](https://push.learningman.top/docs/index.html).

ZNotify didn't provide a public server, but you can easily deploy your own server. See [Server](https://github.com/ZNotify/server) for more information.

## SDK

ZNotify has SDKs for the following languages:

- [Python](https://github.com/ZNotify/py-sdk)
- [C#](https://github.com/ZNotify/cs-sdk)
- [Kotlin](https://github.com/ZNotify/kt-sdk)
- [Rust](https://github.com/ZNotify/rs-sdk)

You can find generated openapi specification at [swagger.json](https://github.com/ZNotify/server/blob/master/docs/swagger.json). For unsupported languages, you can use the openapi specification to generate your own SDK.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue.


## License

Different parts of ZNotify are licensed under different licenses. See the `LICENSE` file in each repository for more information.



