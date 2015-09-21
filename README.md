我稍微修改的 telegram 版本（Fork from [DrKLO/Telegram](https://github.com/DrKLO/Telegram)）：

* 增加 类似微信的习惯，打开表情栏的时候，如果点击上面的聊天区域，能够自动回缩关闭表情栏。
* 修改 当超过1条的未读消息时候，通知（包括浮动通知）的消息预览不再是显示「x new messages」，而是直接在 content 中显示消息内容。（No "x new messages" in notification, show all the preview messages  content / summary in notification including head up.）

telegram 需要翻墙，初次启动它会同步下来所有聊天记录，所以这时候有可能比较卡，之后就好了。

Release：https://github.com/drakeet/Telegram/releases/tag/d1.1

因为官方限制，所以我们开发的 telegram 不能叫做 telegram（「*Please don't use the word Telegram in the title of your app.*」），所以我改名叫 `Teleet`，我自己的是 `Tel4Drakeet`，哈哈哈！

--------------
## Telegram messenger for Android

[Telegram](http://telegram.org) is a messaging app with a focus on speed and security. It’s superfast, simple and free.
This repo contains the official source code for [Telegram App for Android](https://play.google.com/store/apps/details?id=org.telegram.messenger).

##Creating your Telegram Application

We welcome all developers to use our API and source code to create applications on our platform.
There are several things we require from **all developers** for the moment.

1. [**Obtain your own api_id**](https://core.telegram.org/api/obtaining_api_id) for your application.
2. Please **do not** use the name Telegram for your app — or make sure your users understand that it is unofficial.
3. Kindly **do not** use our standard logo (white paper plane in a blue circle) as your app's logo.
3. Please study our [**security guidelines**](https://core.telegram.org/mtproto/security_guidelines) and take good care of your users' data and privacy.
4. Please remember to publish **your** code too in order to comply with the licences.

### API, Protocol documentation

Telegram API manuals: http://core.telegram.org/api

MTproto protocol manuals: http://core.telegram.org/mtproto

### Usage

**Beware of using the dev branch and uploading it to any markets, in many cases it not will work as expected**.

First of all, take a look at **src/main/java/org/telegram/messenger/BuildVars.java** and fill it with correct values.
Import the root folder into your IDE (tested on Android Studio), then run project.

### Localization

We moved all translations to https://www.transifex.com/projects/p/telegram/. Please use it.
