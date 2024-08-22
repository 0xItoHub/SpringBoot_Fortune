
# 占いアプリケーション



このプロジェクトは、Spring Bootを使用して作成された簡単な占いアプリケーションです。アプリケーションはランダムに大吉、中吉、小吉、凶の結果を返し、それぞれに対応するHTMLページを表示します。

## 特徴

- ランダムに運勢を決定します
- 4種類の運勢（大吉、中吉、小吉、凶）を表示します

## 使用技術

- Java 21.0.2
- Spring Boot 3.2.8
- Thymeleaf

## インストールと実行

1. **リポジトリをクローン**

   ```
   git clone https://github.com/yourusername/fortune-app.git
   cd fortune-app
   ```

2. **依存関係をインストール**

   プロジェクトのルートディレクトリで以下のコマンドを実行して、必要な依存関係をインストールします。

   ```
   mvn clean install
   ```

3. **アプリケーションの実行**

   以下のコマンドでアプリケーションを起動します。

   ```
   mvn spring-boot:run
   ```

4. **アプリケーションにアクセス**

   ブラウザを開き、`http://localhost:8080/fortune`にアクセスすると、ランダムに選ばれた運勢が表示されます。

## ファイル構成

- `src/main/java/com/example/demo/Fortune.java`: アプリケーションのコントローラ。ランダムに運勢を決定します。
- `src/main/resources/templates/`
  - `greatFortune.html`: 大吉の結果を表示するテンプレート
  - `middleFortune.html`: 中吉の結果を表示するテンプレート
  - `smallFortune.html`: 小吉の結果を表示するテンプレート
  - `misFortune.html`: 凶の結果を表示するテンプレート

## サンプルHTML

各テンプレートは以下のような内容を持ちます：

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>占い</title>
</head>
<body>
<h1>あなたの運勢は。。。大吉です！</h1>
</body>
</html>
```

上記は大吉のテンプレートの例です。中吉、小吉、凶のテンプレートも同様に、`<h1>`タグの内容を変えることで対応しています。

## ライセンス

このプロジェクトはMITライセンスの下で公開されています。詳細はLICENSEファイルを参照してください。

## 貢献

バグ報告や新機能の提案は、GitHubの[Issues](https://github.com/yourusername/fortune-app/issues)ページで受け付けています。プルリクエストも歓迎します。
