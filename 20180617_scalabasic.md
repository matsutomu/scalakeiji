

# scala 構文 リンク集
  まず実行するために・・・
  - giter8  
  https://www.scala-sbt.org/1.x/docs/sbt-new-and-Templates.html#Template+Resolver  
  https://www.scala-sbt.org/1.x/docs/sbt-new-and-Templates.html  
  http://takezoe.hatenablog.com/entry/2017/01/02/161519  

  ```
  object Sample extends App {
    println("Hello World")
  }
  ```

  もしくは

  ```
  object Sample {
    def main(args: Array[String]) = {
      println("Hello World")
    }
  }
  ```

  構文の説明を読んで、OSSでどのような実例があるかを見て行きたいと思います。

## 基本構文
  以下のサイトを読み進めながら進行します。
  https://dwango.github.io/scala_text/control-syntax.html

### val / var
  - 通常 val  
    https://github.com/gitbucket/gitbucket/blob/163fcd86e035be52f706d0fbd7e1522e7f5e9a10/src/main/scala/gitbucket/core/util/Keys.scala#L16

  - 型指定あり val


  - 貴重なvar  
    https://github.com/gitbucket/gitbucket/blob/163fcd86e035be52f706d0fbd7e1522e7f5e9a10/src/main/scala/gitbucket/core/util/JDBCUtil.scala#L74


### if

  - val 初期化あり1  
    https://github.com/scalatra/scalatra/blob/86d0c1b120723dd80a518ade01ebfa0d99f8626b/core/src/main/scala/org/scalatra/servlet/FileUploadSupport.scala#L82

  - val 初期化あり2  
    https://github.com/scalatra/scalatra/blob/86d0c1b120723dd80a518ade01ebfa0d99f8626b/core/src/main/scala/org/scalatra/servlet/RichRequest.scala#L80

  - 副作用  
    https://github.com/scalatra/scalatra/blob/86d0c1b120723dd80a518ade01ebfa0d99f8626b/core/src/main/scala/org/scalatra/i18n/I18nSupport.scala#L21

  - メソッド戻り値1  
    https://github.com/scalatra/scalatra/blob/86d0c1b120723dd80a518ade01ebfa0d99f8626b/core/src/main/scala/org/scalatra/ScalatraFilter.scala#L62

  - メソッド戻り値2  
    https://github.com/scalikejdbc/scalikejdbc/blob/6b5485f13020cffc4d3eaf9572b0b038f4fa038a/scalikejdbc-config/src/main/scala/scalikejdbc/config/TypesafeConfigReader.scala#L126

### while
  - 待機ループ  
    https://github.com/scalikejdbc/scalikejdbc/blob/c44bd048f0737290e586b5b2fc1834216f662f03/scalikejdbc-core/src/main/scala/scalikejdbc/ConnectionPool.scala#L181

  - do - while  
    https://github.com/scalikejdbc/scalikejdbc/blob/36492f6c3c4c388168ecfcc25ecbdf1843bc9c7e/scalikejdbc-streams/src/test/scala/scalikejdbc/streams/TestDBSettings.scala#L40

### for
  - 単純 for  
    https://github.com/gitbucket/gitbucket/blob/cadd1282991762b5c85f10dfadce170f4d4af401/src/main/scala/gitbucket/core/util/DatabaseConfig.scala#L112

  - if & yield  
    https://github.com/scalatra/scalatra/blob/3c7b7c3f24dbe334c0531a4241d09c97bb8da6b8/core/src/test/scala/org/scalatra/RouteTest.scala#L20  

  - about yield  
    https://docs.scala-lang.org/tutorials/FAQ/yield.html


### try
  - 例外キャッチ  
    https://github.com/gitbucket/gitbucket/blob/2b2669978f575d74c7ed1cad54ca05759e2d16ed/src/main/scala/gitbucket/core/util/JGitUtil.scala#L840

  - 例外をThrow  
    https://github.com/gitbucket/gitbucket/blob/163fcd86e035be52f706d0fbd7e1522e7f5e9a10/src/main/scala/gitbucket/core/util/FileUtil.scala#L86

  - finally  
    https://github.com/gitbucket/gitbucket/blob/163fcd86e035be52f706d0fbd7e1522e7f5e9a10/src/main/scala/gitbucket/core/util/FileUtil.scala#L51

### match
  - 文字列でマッチ
    https://github.com/scalikejdbc/scalikejdbc/blob/0260e7373563a4fe3ed136da2dc66241e1f6d553/scalikejdbc-mapper-generator-core/src/main/scala/scalikejdbc/mapper/LineBreak.scala#L4

  - ifガード
    https://github.com/gitbucket/gitbucket/blob/410627661634381b267da18ca3e90593108cf16f/src/main/scala/gitbucket/core/util/FileUtil.scala#L42  
    https://github.com/gitbucket/gitbucket/blob/cadd1282991762b5c85f10dfadce170f4d4af401/src/main/scala/gitbucket/core/util/LDAPUtil.scala#L117  

  - ifガード（複数条件）  
    https://github.com/scalatra/scalatra/blob/3c7b7c3f24dbe334c0531a4241d09c97bb8da6b8/core/src/main/scala/org/scalatra/RouteRegistry.scala#L55

  - データ型  
    https://github.com/scalatra/scalatra/blob/2.7.x/core/src/main/scala/org/scalatra/servlet/FileUploadSupport.scala#L75

  - List  
    http://aperiodic.net/phil/scala/s-99/p01.scala

## コレクション
  参考  
  https://dwango.github.io/scala_text/collection.html  


## tips
  - mkString

  - String Interpolation



## クラス

### クラス色々

### オブジェクト

### ケースクラス

### トレイト


## 関数

## Implicit


## エラー処理
### Option
  https://github.com/scalatra/scalatra/blob/2.7.x/core/src/main/scala/org/scalatra/servlet/RichRequest.scala#L58

### Either

### Try


# work

## Style

http://seratch.hatenablog.jp/entry/20120128/1327762079
https://docs.scala-lang.org/style/

## quiz

### S-99
   [S-99](http://aperiodic.net/phil/scala/s-99/) (http://aperiodic.net/phil/scala/s-99/)

### Aizu Online Judge
[Aizu Online Judge](http://judge.u-aizu.ac.jp/onlinejudge/)   (http://judge.u-aizu.ac.jp/onlinejudge/)  

   - ITP2_1_C
   http://judge.u-aizu.ac.jp/onlinejudge/description.jsp?id=ITP2_1_C&lang=jp


   - ITP2_3_C - "Count"  
   http://judge.u-aizu.ac.jp/onlinejudge/description.jsp?id=ITP2_3_C&lang=jp



### AtCoder
[AtCoder](https://atcoder.jp/)  (https://atcoder.jp/)



## etc
・"." が不要な例
https://github.com/gitbucket/gitbucket/blob/4f92739d7375960ee2464aaff2f9e872caa38dcb/src/test/scala/gitbucket/core/service/ServiceSpecBase.scala#L24

・ローンパターン  
・色々なロケットシンボル
