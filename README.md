# javabook-maven-example

『Java本格入門』Chapter 12「ビルドと静的解析で品質を上げる」で使うMavenのサンプルプロジェクトです。

## 版とタグの対応

| 版 | タグ | 前提環境 |
| --- | --- | --- |
| 第1版 | `java8` | Java 8 / Maven 3 / JUnit 4 |
| 第2版（Java 25対応） | `java25` | Java 25 / Maven 3.9 / JUnit 6 |

お読みの版に対応するタグをチェックアウトしてください。

```
git clone https://github.com/acroquest/javabook-maven-example.git
cd javabook-maven-example
git checkout java25
```

## 使い方（第2版）

| コマンド | 内容 |
| --- | --- |
| `mvn package` | コンパイル・テスト・JAR作成（target/javabook-maven-example-1.0.0.jar） |
| `mvn checkstyle:check` | Checkstyleの結果をログに出力する（規約違反があるとビルドは失敗する） |
| `mvn compile spotbugs:check` | SpotBugsの結果をログに出力する |
| `mvn site` | Checkstyle・SpotBugs・テスト結果のHTMLレポートをtarget/siteに出力する |
