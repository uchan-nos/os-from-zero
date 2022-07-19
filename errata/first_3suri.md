# 初版第3刷の正誤情報

重要な誤植が見つかり次第掲載していきます。些細な正誤情報も含めたリストは [初版第3刷の正誤情報（すべて）](first_3suri_all.md) をご覧ください。

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
- p.228 第3段落の1行目
    - 誤：直後に `Initial Count` レジスタの値を読み出すことで
    - 正：直後に `Current Count` レジスタの値を読み出すことで
- p.255 第2段落の1行目
    - 誤：`Layer::Draw()` に対して描画範囲を指定
    - 正：`Layer::DrawTo()` に対して描画範囲を指定
- p.255 第2段落の2行目
    - 誤：`Layer::Draw()` 側を改造
    - 正：`Layer::DrawTo()` 側を改造
