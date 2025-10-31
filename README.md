# ohos-sdk-dailybuild

本组织下的许多项目都依赖最新版的 ohos-sdk 的能力，如二进制签名工具（为二进制文件加代码签名以支持它运行在商用发行版 HarmonyOS 上）、原生编译器（允许用户在 ohos 系统上编 ohos 的产物）等。

这部分能力在 [6.0 正式版的 ohos-sdk](https://gitcode.com/openharmony/docs/blob/master/zh-cn/release-notes/OpenHarmony-v6.0-release.md#%E4%BB%8E%E9%95%9C%E5%83%8F%E7%AB%99%E7%82%B9%E8%8E%B7%E5%8F%96) 上还尚未提供，因此我们只能从 [OpenHarmony 官方社区的流水线](https://ci.openharmony.cn/) 下载每日构建版本的 ohos-sdk 来使用。

由于每日构建版本的下载链接是有时效的，每个 ohos-sdk 压缩包的下载链接都会在一段时间后过期（一个月左右），因此我们无法拿到一个固定链接、固定内容的 ohos-sdk 来进行我们的构建工作，这会导致我们组织内的项目无法做到“可重复构建”。

为了解决这个问题，使组织内的其他项目能做到“可重复构建”，我们会不定期把每日构建的 ohos-sdk 下载一份存档起来，放到这个仓库的 Releases 页面中。这样做之后，组织内的其他项目要用 ohos-sdk 的时候就可以来这里取，它们就可以获取到固定链接、固定内容的 ohos-sdk，以实现“可重复构建”。

在满足自身需求的同时，我们也期望这个项目能为更多人提供便利。其他开发者若也有相同需求，也可从这里下载最新 ohos-sdk，不需要再自己进行存档。

如果你关心产物可信，我们也提供了完整性校验的手段：我们发布压缩包时候会标注它的构建时间，你可以前往 [OpenHarmony 官方社区的流水线](https://ci.openharmony.cn/) 根据构建时间进行检索，获取它们的哈希值和签名文件，对我们的压缩包进行校验。哈希值、签名文件与 ohos-sdk 压缩包不同，它不会过期。
