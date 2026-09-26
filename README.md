# IceBridge

IceBridge is an Android LSPosed module supporting IceBox SDK mode and Root (su) mode.

## Features

- Observes supported HTTPS links from system_server.
- Identifies Xiaohongshu, Weibo, Zhihu, Alipay, X/Twitter, YouTube, Instagram, and Telegram targets.
- Restores a frozen target app, then opens the original link.
- Supports custom domain.example=com.example.app mappings.

The default scope only needs system. WeChat, QQ, browsers, and target apps are not required. The optional WebView observer runs only in a host process explicitly added by the user.

## Usage

1. Download and install the APK from the Releases page.
2. Enable Ice Bridge in LSPosed and select system as its scope.
3. Reboot the device or relevant system process.
4. Select IceBox SDK or Root mode in the app and grant the requested permissions.

The runtime requires a rooted Android device, LSPosed (libxposed API 102), and Android 8.0 or newer. ROM, Android version, and work profile behavior require separate validation.

## Package migration

From 0.0.78 to 0.0.79, the application ID changed from com.huanchengfly.icebridge to io.github.yudigaga.icebridge, so the new version installs as a separate app. Export custom link rules from the old app before uninstalling it, import them into the new app, and configure other settings again. Disable the old module, enable the new module, and reboot.

## Source and license

- Source repository: https://github.com/yudigaga/IceBridge
- v0.0.79 release: https://github.com/yudigaga/IceBridge/releases/tag/v0.0.79
- License: GPL-3.0-only.
