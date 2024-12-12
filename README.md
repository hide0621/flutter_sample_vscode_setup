# Flutter Android: could not create task ' generatelockfiles'の解消法

### 手順1

以下のコマンドでローカルのjavaのバージョンを調べる

`java --version`

### 手順2

java versionと一致するgradle varsionを確認する。

[対応表](https://docs.gradle.org/current/userguide/compatibility.html)

この時、たとえばjavaのバージョンが`19.0.2`なら、

`distributionUrl=https\://services.gradle.org/distributions/gradle-7.6-all.zip`

上記のように、`distributionUrl`を書き換える！

ポイントは`-all`とすること！

### 手順3

`flutter pub get`をして、新しいgradleを入れる。

この時、上手く同期ができないこともあるので、その際は**少し時間が経ってから再度プロジェクトを開く！**

参考：
- https://qiita.com/yoshiki132/items/e1f7ae9bf842818b069a

- https://marcelobarce.wordpress.com/2024/08/24/fixing-generatelockfiles-error-on-flutter/

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
