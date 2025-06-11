# 初版第2刷の正誤情報

重要な誤植が見つかり次第掲載していきます。些細な正誤情報も含めたリストは [初版第2刷の正誤情報（すべて）](first_2suri_all.md) をご覧ください。

- p.39 第2段落の6行目
    - 誤：「oは0x65」
    - 正：「oは0x6f」
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
- p.108 表4.4タイトル
    - 誤：クラスのvtable
    - 正：`Base`クラスのvtable
- p.255 第2段落の1行目
    - 誤：`Layer::Draw()` に対して描画範囲を指定
    - 正：`Layer::DrawTo()` に対して描画範囲を指定
- p.255 第2段落の2行目
    - 誤：`Layer::Draw()` 側を改造
    - 正：`Layer::DrawTo()` 側を改造
- p.501 最終段落の2行目
    - 誤：`Task`クラスはもともと、そのタスク用のスタックポインタを保存するための変数`Task::stack_ptr_`を持っています。この変数に並べて`Task::os_stack_ptr_`を持たせました。
    - 正：`Task`クラスはもともと、そのタスク用のスタックポインタを保存するための変数`Task::context_.rsp`を持っています。この変数に加えて`Task::os_stack_ptr_`を持たせました。
        - `stack_ptr_`→`context_.rsp`
        - 並べて→加えて
