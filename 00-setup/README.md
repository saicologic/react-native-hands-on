
- [React Native](https://facebook.github.io/react-native/)の開発をサポートする[Expo](https://expo.io/)を利用して、プロジェクトファイルを作成します。
- プロジェクトファイルを作成するためには、[expo-cli](https://docs.expo.io/versions/latest/workflow/expo-cli)というコマンドラインツールをインストールする必要があります。
- expo-cliを動作させるためには、[Node.js](https://nodejs.org/en/)が必要なため、先にNode.jsをインストールします、

# やること
- nodeをインストールする(すでにインストール済みであれはスキップ)
- expo-cliをインストールする

# 手順
## nodeをインストールする
Node.jsのバージョンは、10以上のバージョンが推奨されています。=> [expo-cli installation](https://docs.expo.io/versions/latest/introduction/installation)

下記から、`10.15.0`(2019/1/12最新) ダウンロードしてください。
https://nodejs.org/en/

### nvmを利用する場合（オプション）

もし、Node.jsのバージョン管理ツールの[nvm](https://github.com/creationix/nvm)を利用している場合は、下記のコマンドでインストールします。

#### node v10.15.0をインストールする

```
nvm install v10.15.0
```

#### v10.15.0を使う

```
nvm use v10.15.0
```

### node.jsのバージョンを確認する

```
node -v
```

出力結果

```
v10.15.0
```

## expo-cliをインストールする

```
npm install -g expo-cli
```

### expo-cliのバージョンを確認する

```
expo-cli --version
```

出力結果

```
2.6.14
```
