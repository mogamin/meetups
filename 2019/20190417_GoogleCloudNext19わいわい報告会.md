# Google Cloud NEXT'19 わいわい報告会
* https://mercaridev.connpass.com/event/125881/

## GothamGoにいってきた！（体調不良のためリモートかも） @tenntenn
??


## xx
* Anthos(あんそす)
* CloudRun
    * BETA is now available.
    * Cloud Run
    * Cloud Run on GKE
    * Knativeを使っている
* Cloud Code
    * is available.
* Traffice Director
    * Networking
* Cloud Data Fusion
    * ETLのパイプラインをここで定義できる？
    * BigQueryBIEngineとはなんだ？
* Cloud Auto ML
    * AutoML Tables BETA is available
    * マシンラーニングに詳しくない人でもテーブルを用意するだけでいいんだよ。系？？
* Sttategic open-source partnerships
* Enterprise Ecosystem
    * 各ベンダーの製品もAnthos上で動かすことを狙っている。


## わかめまさひろ
* 全般的にK8s中心の話になっている。逃げられない。ある程度は覚悟を決める必要があるかもね。
* Spanner Internals
    * Spannerとは？
        * Relational DBと同じsemantics
            * Schemas, ACID, Transactions, SQL
        * Horizontal Scale
            * ScaleOutができる。MySQLではできない。
        * Paxosアルゴリズム
            * 分散合意のためのプロトコル
            * TrueTime API
                * TxOps
        * Eventaual consitency辛いか？
            * Strong consistencyは、人生が豊かになる


## cloud codeについて @tenling
* Cloud Code
    * https://github.com/GoogleContainerTools/skaffold


## DataAnalytics系プロダクト発表紹介 @orfeon
* Cloud Dataflow
    * Streaming Engine & Streaming Autoscaling
        * 状態管理をサービスとして分るし、性能とコスパと可用性向上
    * Dataflow SQL
        * BiqQueryUIからSQLで記述した処理をdataflow実行できるように
    * Dataflow FlexRS(Beta)
        * Preemptivble VMで併用できるようにする

* Cloud Dataflow - Steaming Engine
* AutoML Tables
    * kaggleの上位を狙っていける


## networking (Traffic Director)について @lainra
* service mesh
    * decoupling ths nework features
    * Data plane(proxy mesh)
* Service Mesh Key Capabilityes
    * Telemetry
    * Security
    * Traffic Control
* Envoy, the universal data plane
    * Network filter
    * HTTP filter
    * Listener filter
    * Health checker
    * Transport sockets
    * Address resolver
    * Clustering
    * Retry policy

## JavaとGoogle Cloud NExt 2019 @shota_st1
---
xx
