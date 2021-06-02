# 初版第2刷の正誤情報（すべて）

重要な正誤情報だけをまとめたリストは [初版第2刷の正誤情報](first_2suri.md) にあります。

- p.39 第2段落の6行目
    - 誤：「oは0x65」
    - 正：「oは0x6f」
- p.54 表2.2 0x00001000の行
    - 誤：`EfiConvensionalMemory`
    - 正：`EfiConventionalMemory`
- p.54 表2.2 0x00100000の行
    - 誤：`EfiConvensionalMemory`
    - 正：`EfiConventionalMemory`
- p.54 第5段落の5行目
    - 誤：4億程度
    - 正：43億程度
- p.58 リスト2.8
    - 1行目は空白1個分しかインデントされていないが、以下の通り、2行目以降と揃えて、空白2個でインデントするのが正しい。
    ```
    ␣␣CHAR8 memmap_buf[4096 * 4];
    ␣␣struct MemoryMap memmap = {sizeof(memmap_buf), memmap_buf, 0, 0, 0, 0};
    ␣␣……
    ```
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
- p.215 第3段落の1行目
    - 誤：**リスト 9.1** 1 に
    - 正：**リスト 9.11** に
- p.255 第2段落の1行目
    - 誤：`Layer::Draw()` に対して描画範囲を指定
    - 正：`Layer::DrawTo()` に対して描画範囲を指定
- p.255 第2段落の2行目
    - 誤：`Layer::Draw()` 側を改造
    - 正：`Layer::DrawTo()` 側を改造
- p.442 図19.2の右から2つ目の枠
    - 誤：`PD[0]` … `PDP[511]`
    - 正：`PD[0]` … `PD[511]`
- p.443 図19.3（図19.2と同様の修正）
    - 誤：`PD[0]` … `PDP[511]`
    - 正：`PD[0]` … `PD[511]`
- p.443 図19.3中段
    - 誤：`PG`
    - 正：`PD`
- p.468 第1段落の1行目
    - 誤：108バイト
    - 正：104バイト
- p.586 リスト25.3タイトル
    - 誤：（terminal.cpp）
    - 正：（fat.cpp）
- p.726 リストC.3の2行目
    - その他の行と字間を揃える（均等割付をやめ、左詰めにする）
    - 誤：`␣␣␣U e f i A p p ……`
    - 正：`␣␣UefiApp……`
    - 字間を揃えた結果、インデントが半角空白2個となり、3行目（`␣␣UefiLib`）と揃うのが正しい
