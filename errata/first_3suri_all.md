# 初版第3刷の正誤情報（すべて）

重要な正誤情報だけをまとめたリストは [初版第3刷の正誤情報](first_3suri.md) にあります。

- p.54 表2.2 0x00001000の行
    - 誤：`EfiConvensionalMemory`
    - 正：`EfiConventionalMemory`
- p.54 表2.2 0x00100000の行
    - 誤：`EfiConvensionalMemory`
    - 正：`EfiConventionalMemory`
- p.54 第5段落の5行目
    - 誤：4億程度
    - 正：43億程度
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
- p.119 第1段落の6行目
    - 誤：「1.2 結局何をやったのか」を参照
    - 正：「1.5 結局、何をやったのか？」を参照
- p.140 第5段落の6行目
    - 誤：eXtended Host Controller Interface
    - 正：eXtensible Host Controller Interface
- p.228 第3段落の1行目
    - 誤：直後に `Initial Count` レジスタの値を読み出すことで
    - 正：直後に `Current Count` レジスタの値を読み出すことで
- p.255 第2段落の1行目
    - 誤：`Layer::Draw()` に対して描画範囲を指定
    - 正：`Layer::DrawTo()` に対して描画範囲を指定
- p.255 第2段落の2行目
    - 誤：`Layer::Draw()` 側を改造
    - 正：`Layer::DrawTo()` 側を改造
- p.468 第1段落の1行目
    - 誤：108バイト
    - 正：104バイト
- p.490 リスト21.3
    - 誤：cconst
    - 正：const
- p.501
    - 誤：`Task`クラスはもともと、そのタスク用のスタックポインタを保存するための変数`Task::stack_ptr_`を持っています。この変数に並べて`Task::os_stack_ptr_`を持たせました。
    - 正：`Task`クラスはもともと、そのタスク用のスタックポインタを保存するための変数`Task::context_.rsp`を持っています。この変数に加えて`Task::os_stack_ptr_`を持たせました。
        - `stack_ptr_`→`context_.rsp`
        - 並べて→加えて
- p.586 リスト25.3タイトル
    - 誤：（terminal.cpp）
    - 正：（fat.cpp）
- p.635
    - 誤：そういえばfat.cppには`LoadFile()`という似た関数があったので、今実装した`Load()`を利用するように改造しておきましたよ。
    - 正：そういえばfat.cppには`LoadFile()`という似た関数があったので、`Load()`の実装をまねて`Read()`を利用するように改造しておきましたよ。
