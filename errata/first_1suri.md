# 初版第1刷の正誤情報

重要な誤植が見つかり次第掲載していきます。些細な正誤情報も含めたリストは [初版第1刷の正誤情報（すべて）](first_1suri_all.md) をご覧ください。

- p.34 第2段落の3行目
    - 誤：「**A.1　開発環境のインストール**」
    - 正：「**付録A.01　WSLのインストール**」
- p.35 第1段落の3行目
    - 誤：「**A.1　開発環境のインストール**」
    - 正：「**付録A　開発環境のインストール**」
- p.35 第1段落の4行目
    - 誤：「**A.2　WSLでQEMUを使う準備**」
    - 正：「**付録A.02　WSLでQEMUを使う準備**」
- p.39 第2段落の6行目
    - 誤：「oは0x65」
    - 正：「oは0x6f」
- p.39 第3段落の3行目
    - 誤：「**A.8　ASCIIコード表**」
    - 正：「**付録F　ASCIIコード表**」
- p.49 第2段落直後の埋め込みリスト
    - 誤：MikanLoader.dec
    - 正：MikanLoaderPkg.dec
- p.49 第2段落直後の埋め込みリスト
    - 誤：MikanLoader.dsc
    - 正：MikanLoaderPkg.dsc
- p.49 第4段落
    - 誤：「付録A　EDK IIのファイル説明」
    - 正：「**付録C　EDK IIのファイル説明**」
- p.51 表2.1
    - [正しい表のイメージ](https://github.com/uchan-nos/os-from-zero/issues/3#issuecomment-803728531)
    - ヘッダ行（網掛け部分）には「設定項目」「設定値」が来るのが正しい。
    - 最終行は不要。
- p.55 表2.3 Type=4の行
    - 誤：EfiBootServicesCode
    - 正：EfiBootServicesData
- p.56 リスト2.6
    - 最終行がリスト外に飛び出しているが、リストに含めるのが正しい。
- p.62 図2.4
    - 誤：`int* q`
    - 正：`int* p`
- p.63 図2.5
    - 2つ目の「0xffc8」は「0xffd8」が正しい。
    - アドレスは上から 0xffc8、0xffd0、0xffd8、0xffdc、0xffe0、0xffe8、0xffec、0xfff0 となる。
- p.64 第1段落の3行目
    - 誤：9ンバ
    - 正：メンバ
- p.72 3.3 第4段落の4行目
    - 誤：`_Z3addii`
    - 正：`_Z3fooii`
- p.73 第4段落直後のコマンド
    - 誤：
        ```
        $ cd $HOME/workspace/mikanos/kernel
        $ git checkout osbook_day03a
        ```
    - 正：
        ```
        $ cd $HOME/workspace/mikanos
        $ git checkout osbook_day03a
        $ cd kernel
        ```
- p.80 第5段落の6行目
    - 誤：0x669f028
    - 正：0x101010
- p.108 第1段落の4行目
    - 誤：vtableというものを実現しています
    - 正：vtableを用いて実現しています
- p.108 表4.4タイトル
    - 誤：クラスのvtable
    - 正：`Base`クラスのvtable
- p.137 リスト6.4タイトル
    - 誤：（graphics.hpp）
    - 正：（osbook_day06cのgraphics.hpp）
- p.255 第2段落の1行目
    - 誤：`Layer::Draw()` に対して描画範囲を指定
    - 正：`Layer::DrawTo()` に対して描画範囲を指定
- p.255 第2段落の2行目
    - 誤：`Layer::Draw()` 側を改造
    - 正：`Layer::DrawTo()` 側を改造
- p.429 リスト18.18
    - リスト最終行と脚注1が重なってしまっている
    - リストの最終行は `v = v * 10 + (s[i] - '0');`
    - 脚注1は「＊1　RPN：Reverse Polish Notation」
- p.501
    - 誤：`Task`クラスはもともと、そのタスク用のスタックポインタを保存するための変数`Task::stack_ptr_`を持っています。この変数に並べて`Task::os_stack_ptr_`を持たせました。
    - 正：`Task`クラスはもともと、そのタスク用のスタックポインタを保存するための変数`Task::context_.rsp`を持っています。この変数に加えて`Task::os_stack_ptr_`を持たせました。
        - `stack_ptr_`→`context_.rsp`
        - 並べて→加えて
- p.716 第1段落の4行目
    - 誤：WSL（**A.1** を参照）
    - 正：WSL（**A.01** を参照）
