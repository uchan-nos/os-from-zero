# 初版第2刷の正誤情報（すべて）

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
- p.255 第2段落の1行目
    - 誤：`Layer::Draw()` に対して描画範囲を指定
    - 正：`Layer::DrawTo()` に対して描画範囲を指定
- p.255 第2段落の2行目
    - 誤：`Layer::Draw()` 側を改造
    - 正：`Layer::DrawTo()` 側を改造
- p.468 第1段落の1行目
    - 誤：108バイト
    - 正：104バイト
- p.586 リスト25.3タイトル
    - 誤：（terminal.cpp）
    - 正：（fat.cpp）
