
# 1. install & Quick Start
以下のURLを参考にインストール。

## 1.1 install jdk  
http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

## 1.2 install sbt  
https://www.scala-sbt.org/1.x/docs/ja/Setup.html


## 1.3 Hello Scala
コマンドラインから以下を実行する
$sbt new scala/hello-world.g8

![sbt new scala/hello-world.g8](vs_code07.png "VS Codeダウンロード")

名前を入力するように求められるので、入力します。  
![VS Code インストール](vs_code08.png "VS Codeダウンロード")


- [giter8](http://www.foundweekends.org/giter8/)

- [giter8 templates wiki](https://github.com/foundweekends/giter8/wiki/giter8-templates)


# 2. VS Codeで編集

## 2.1 インストール

お好きな環境の対象をダウンロードします。  
[VS Code ダウンロードサイト](https://code.visualstudio.com/Download)

![VS Code インストール](vs_code01.png "VS Codeダウンロード")

以下は Macでのインストールの様子です。  
![VS Code インストール](vs_code02.png "VS Codeダウンロード")

![VS Code インストール](vs_code03_2.png "VS Codeダウンロード")

![VS Code インストール](vs_code03_3.png "VS Codeダウンロード")

![VS Code インストール](vs_code04.png "VS Codeダウンロード")

![VS Code起動直後](vs_code05.png "VS Code起動直後")

## 2.2 フォルダを開く

![VS Code フォルダ1](vs_code09.png "VS Codeダウンロード")

![VS Code フォルダ2](vs_code10.png "VS Codeダウンロード")

![VS Code フォルダ3](vs_code11.png "VS Codeダウンロード")

--------

## 2.3 デバックコンソール  

![VS Code コンソール1](vs_code12.png "VS Codeダウンロード")

![VS Code コンソール2](vs_code13.png "VS Codeダウンロード")

![VS Code コンソール3](vs_code14.png "VS Codeダウンロード")

## 2.4 プラグインのインストール
![VS Code プラグイン1](vs_code15.png "VS Codeダウンロード")

![VS Code プラグイン2](vs_code16.png "VS Codeダウンロード")

![VS Code プラグイン3](vs_code17.png "VS Codeダウンロード")


以下のファイルを作成します。  
./project/plugin.sbt

ファイルの中身は以下の内容を記載します。  
```
addSbtPlugin("org.ensime" % "sbt-ensime" % "2.5.1")
```
![VS Code プラグイン4](vs_code18.png "VS Codeダウンロード")


コンソールで以下のコマンドを実行します。  
$sbt ensimeConfig

VS Code 再起動でコード補間etcが実行されます。


