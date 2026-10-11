# Trie Homebrew tap

This repository contains the Homebrew cask for [Trie](https://trie.ai/), a local voice-input app for Apple Silicon Macs.

The first stable cask is being prepared. A cask will be added after the matching release is signed, notarized, and verified. Follow [Trie releases](https://github.com/TRIEAI/trie/releases) for availability.

Requirements: Apple Silicon, macOS 14 or later, at least 16 GB memory and 12 GB free disk space. The app's setup assistant prepares Python and downloads models with your confirmation.

After the stable cask is available:

```sh
brew install --cask TRIEAI/trie/trie
brew upgrade --cask TRIEAI/trie/trie
```

Quit Trie before upgrading. Regular uninstall removes the application while retaining user configuration and models:

```sh
brew uninstall --cask trie
```

`brew uninstall --zap --cask trie` also removes the configuration, application support directory and logs listed in the cask. Use it only if you intend to remove that data. Shared model caches are not removed.

Report app problems at [TRIEAI/trie](https://github.com/TRIEAI/trie/issues/new/choose). Reports are public; do not include private dictation, clipboard contents, recordings or credentials.

## 中文

这是 Trie 的 Homebrew 分发仓库。首个稳定 cask 正在准备，将在对应安装包完成签名、公证和验证后加入。安装要求与下载方式以 [官网](https://trie.ai/install.html) 和 [发布记录](https://github.com/TRIEAI/trie/releases) 为准。

升级前先退出 Trie。普通卸载保留配置和模型；只有你明确选择 `--zap` 时才移除 cask 中列出的配置、应用数据和日志，共享模型缓存不删除。
