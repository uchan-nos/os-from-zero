# 初版第6刷の正誤情報（すべて）

重要な正誤情報だけをまとめたリストは [初版第6刷の正誤情報](first_6suri.md) にあります。

- p.501 最終段落の2行目
    - 誤：`Task`クラスはもともと、そのタスク用のスタックポインタを保存するための変数`Task::stack_ptr_`を持っています。この変数に並べて`Task::os_stack_ptr_`を持たせました。
    - 正：`Task`クラスはもともと、そのタスク用のスタックポインタを保存するための変数`Task::context_.rsp`を持っています。この変数に加えて`Task::os_stack_ptr_`を持たせました。
        - `stack_ptr_`→`context_.rsp`
        - 並べて→加えて
- p.635 リスト27.18直後の段落の2行目
    - 誤：そういえばfat.cppには`LoadFile()`という似た関数があったので、今実装した`Load()`を利用するように改造しておきましたよ。
    - 正：そういえばfat.cppには`LoadFile()`という似た関数があったので、`Load()`の実装をまねて`Read()`を利用するように改造しておきましたよ。
