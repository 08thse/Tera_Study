# TERASOLUNA 勉強用
TERASOLUNA の勉強用にリポジトリを作ってみました

## やりたいこと
* とりあえず簡単なコメント Web アプリ
* 単体テスト自動化
* 結合テスト自動化
* CI/CD

## 環境
### 開発用
* Windows 10
* Eclipse neon.1
* Tomcat 8.5
* Postgres 9.5
* Oracle JDK 8u151
* [chocolatey](https://chocolatey.org/)

### 動作用 (まだ)
* CentOS 7.x
* Postgres
* OpenJDK

### リポジトリ
https://github.com/08thse/Tera_Study

### 参考情報
* http://terasolunaorg.github.io/guideline/

## 1. とりあえず動かしてみる
###テンプレートからひな形を作成
* chocolatey から maven をインストールした
* コマンドプロンプトにて下記の通りコマンドを実行
```
mvn archetype:generate -B^
 -DarchetypeGroupId=org.terasoluna.gfw.blank^
 -DarchetypeArtifactId=terasoluna-gfw-multi-web-blank-mybatis3-archetype^
 -DarchetypeVersion=5.3.1.RELEASE^
 -DgroupId=local.08thse.comment^
 -DartifactId=comment^
 -Dversion=1.0.0-SNAPSHOT
```
