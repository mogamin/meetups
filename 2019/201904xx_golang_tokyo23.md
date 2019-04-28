# golang.tokyo #23
* https://golangtokyo.connpass.com/event/126673/


## 絶対に分かるポインタ
* Softdesign GO
    * 入門GO
* ポインタ

## Goをはじめるあたって知っておいてほしいツールやテスト
* golang.orgを参照しなさい。
    * https://golang.org/
    * http://golang.jp/ は古い
* gophers.slack.com
* golanng.weeklyを読もう(木曜日配信)
* 便利なツール
    * 環境変数を表示する 
        * go env
    * コードをformatする
        * gofmt
            * optionがいくつもある
            * options
                * -d:diff
                * -l
                * -w
                * -s
        * go fmt
            * gofmt -l -wと同じ働き
    * コード内容を静的解析する、コンバイらには検知できないものを見つけてくれる
        * go vet
    * リンターに書ける
        * golint
 
## テストについて
* テストについて
    * Test{関数名}(小文字で始まらない)
    * _test.goで終わる名前を作成する。
    * ..
* TableDrivenTest
* TestMain
    * テストの前処理を設定することができる
* Testの実行
    * go test -run ''       #すべてのテストをする
    * go test -run Bear
    * go test -run Bear/A
    * go test -run /A
* Testingができること
    * ベンチマーク
    * カバレッジ
    * テストをスキップする
* Go Playgroundでもテストを書くことができる。
* しっておくとよいこと
    * グローバルとプライベート
        * 小文字では自前ると、パッケージの中だけ。
        * 大文字で始まるとパッケージの外（グローバル）から呼べる。
    * defar // 関数の最後に実行するとか
    * switch
        * breakがいらない
    * 関数の戻り値
        * 複数の値が戻せる
    * 技術書展でGoが大好きになる本を出したよ。BOOTHで出すかもね。
    * 

## Delveを用いたデバッグ & pprofを用いたプロファイリング
* コードを描いたあとの点について
* Delve
    * golangのデバッグツール
* install
    * go get -u github.com/go-xxxxxxxx
* pprofについて


## LT
* GoReleaser/簡単にデリバリするツール？
    * cross compile
    * single binary
    * 一般的には次のうちどれか？
        * go get
            * goの環境がそもそも必要
            * HEADでcompileしてしまう
        * Guthub release
            * ブラウザからダウンロード、解答、PATHはいやただよね。
    * package managerを使う
        * リリースすることが一番大事。
        * 環境構築が必要ない
        * マニフェストファイルで管理ができる。（非推奨になった？）
    * Formulaの管理が面倒
        * リリースするたびにコミットが必要
    * ./goreleaser.yml
    * goreleaserコマンド
    * goxというツールが有名(hashicorp)
    * ghr(mercari)
    * git.ioってなんだ？
    * @micnncim
