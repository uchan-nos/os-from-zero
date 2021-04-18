# 初版第1刷の正誤情報（すべて）

重要な正誤情報だけをまとめたリストは [初版第1刷の正誤情報](first_1suri.md) にあります。

- p.34 第2段落の3行目
    - 誤：「**A.1　開発環境のインストール**」
    - 正：「**付録A.01　WSLのインストール**」
- p.35 第1段落の3行目
    - 誤：「**A.1　開発環境のインストール**」
    - 正：「**付録A　開発環境のインストール**」
- p.35 第1段落の4行目
    - 誤：「**A.2　WSLでQEMUを使う準備**」
    - 正：「**付録A.02　WSLでQEMUを使う準備**」
- p.38 第2段落直後の埋め込みリスト
   - 以下のように、「F A C E」の位置を2進数4桁と揃える
    ```
    = 1111 1010 1100 1110
    =    F    A    C    E
    = 0xFACE
    ```
- p.39 第2段落の6行目
    - 誤：「oは0x65」
    - 正：「oは0x6f」
- p.39 第3段落の3行目
    - 誤：「**A.8　ASCIIコード表**」
    - 正：「**付録F　ASCIIコード表**」
- p.40 1.6の最終段落の最終行
    - 誤：完全な差分が分かります。
    - 正：完全な差分が分かります。詳しくは「**付録B.01 MikanOSのバージョン間の差分確認**」を参照してください。
- p.43 第3段落の3行目
    - 誤：**EfiMain()**
    - 正：`EfiMain()`
- p.49 第2段落直後の埋め込みリスト
    - 誤：MikanLoader.dec
    - 正：MikanLoaderPkg.dec
- p.49 第2段落直後の埋め込みリスト
    - 誤：MikanLoader.dsc
    - 正：MikanLoaderPkg.dsc
- p.49 第4段落
    - 誤：「付録A　EDK IIのファイル説明」
    - 正：「**付録C　EDK IIのファイル説明**」
- p.50 第1段落の4行目
    - 誤：`#nclude`
    - 正：`#include`
- p.51 表2.1
    - [正しい表のイメージ](https://github.com/uchan-nos/os-from-zero/issues/3#issuecomment-803728531)
    - ヘッダ行（網掛け部分）には「設定項目」「設定値」が来るのが正しい。
    - 最終行は不要。
- p.52 リスト2.3
    - 誤：EDK IIのUefi.h体
    - 正：EDK IIのUefi.h
- p.52 リスト2.4
    - 誤：リスト2.4　EDK IIのUefiBaseType.h
    - 正：**リスト2.4　EDK IIのUefiBaseType.h**
- p.55 表2.3 Type=4の行
    - 誤：EfiBootServicesCode
    - 正：EfiBootServicesData
- p.55 表2.3 Type=7の行
    - s→t
    - 誤：EfiConvensionalMemory
    - 正：EfiConventionalMemory
- p.56 リスト2.6タイトル
    - 「の仕様」の「様」が1mmほど上方にズレているが、ズレていないのが正しい。
- p.56 リスト2.6
    - 最終行がリスト外に飛び出しているが、リストに含めるのが正しい。
- p.58 第2段落の3行目
    - 誤：**リスト 2.** 7 のように
    - 正：**リスト 2.7** のように
- p.58 リスト2.8
    - 1行目は空白1個分しかインデントされていないが、以下の通り、2行目以降と揃えて、空白2個でインデントするのが正しい。
    ```
    ␣␣CHAR8 memmap_buf[4096 * 4];
    ␣␣struct MemoryMap memmap = {sizeof(memmap_buf), memmap_buf, 0, 0, 0, 0};
    ␣␣……
    ```
- p.62 図2.4
    - 誤：`int* q`
    - 正：`int* p`
- p.63 図2.5
    - 2つ目の「0xffc8」は「0xffd8」が正しい。
    - アドレスは上から 0xffc8、0xffd0、0xffd8、0xffdc、0xffe0、0xffe8、0xffec、0xfff0 となる。
- p.64 第1段落の3行目
    - 誤：9ンバ
    - 正：メンバ
- p.64 最終段落の2行目
    - 誤：「.」}
    - 正：「.」
- p.66 第1段落直後の埋め込みリスト
    - 埋め込みリストの2行目以降のインデント（半角スペース2個）を解除する。正しい形は以下。
    ```
    EFI_FILE_PROTOCOL* memmap_file;
    EFI_FILE_PROTOCOL** ptr_ptr = &memmap_file;
    root_dir->Open(
    ␣␣␣␣root_dir, ptr_ptr, L"\\memmap",
    ␣␣␣␣EFI_FILE_MODE_READ | EFI_FILE_MODE_WRITE | EFI_FILE_MODE_CREATE, 0);
    ```
- p.68 脚注1
    - 誤：使えます。。
    - 正：使えます。
- p.72 3.3 第4段落の4行目
    - 誤：int foo(int, int)
    - 正：`int foo(int, int)`
- p.72 3.3 第4段落の4行目
    - 誤：`_Z3addii`
    - 正：`_Z3fooii`
- p.73 第2段落の2行目
    - 誤：\_\_asm\_\_()
    - 正：`__asm__()`
- p.74 第1段落の5行目
    - 誤：`fno-rtti`
    - 正：`-fno-rtti`
- p.76 第3段落の4行目
    - 誤：「コラム3.2　ポインタのキャスト」
    - 正：「**コラム3.2　ポインタのキャスト**」
- p.77 第5段落の3行目
    - 誤：C++の整数同士
    - 正：C言語の整数同士
- p.80 第5段落の6行目
    - 誤：0x669f028
    - 正：0x101010
- p.82 第2段落の1行目
    - 誤：今後作っていくOSでは、文字列だけではなくウィンドウやマウスカーソルなど、
    - 正：今後作っていくOSでは、ウィンドウやマウスカーソルなど、
- p.82 箇条書き第4項目
    - 誤：RBG
    - 正：RGB
- p.83 第2段落の3行目
    - 誤：RBG
    - 正：RGB
- p.87 コラム3.2 第3段落の2行目
    - 誤：型情報（int）
    - 正：型情報（`int`）
- p.88 第2段落の1行目
    - 誤：「3.3　初めてのカーネル」
    - 正：「**3.3　初めてのカーネル**」
- p.91 第3段落の1行目
    - 誤：変数r1に書く操作
    - 正：変数`r1`に書く操作
- p.91 箇条書き第3項目
    - 誤：指す先の型はint
    - 正：指す先の型は`int`
- p.94 第2段落の1行目
    - 誤：「第3章　画面表示の練習とブートローダ」
    - 正：「**第3章　画面表示の練習とブートローダ**」
- p.94 埋め込みリスト
    - 誤：`clang++ -I/home/uchan/osbook/devenv/x86_64-elf/include/c++/v1 -I/home/uchan/osbook/evenv/x86_64-elf/include -nostdlibinc -D__ELF__ -D_LDBL_EQ_DBL -D_GNU_SOURCE -D_POSIX_TIMERS -O2 --target=x86_64-elf -fno-exceptions -ffreestanding -c main.cpp`
    - 正：`clang++ -I/home/uchan/osbook/devenv/x86_64-elf/include/c++/v1 -I/home/uchan/osbook/devenv/x86_64-elf/include -I/home/uchan/osbook/devenv/x86_64-elf/include/freetype2 -nostdlibinc -D__ELF__ -D_LDBL_EQ_DBL -D_GNU_SOURCE -D_POSIX_TIMERS -O2 -Wall -g --target=x86_64-elf -ffreestanding -mno-red-zone -fno-exceptions -fno-rtti -std=c++17 -c main.cpp`
- p.99 最終段落の3行目
    - 誤：図4.1
    - 正：**図4.1**
- p.101 第3段落の3行目
    - 誤：「コラム3.1　レッドゾーン」
    - 正：「**コラム3.1　レッドゾーン**」
- p.106 第2段落の6行目
    - 誤：「4.4　vtable」
    - 正：「**4.4　vtable**」
- p.106 第3段落の4行目
    - 誤：意味的にきれいにプログラム
    - 正：意味的にきれいなプログラム
- p.107 第5段落の6行目
    - 誤：知人やosdev-jpに質問するといいでしょう。
    - 正：知人や本書のサポートサイトに質問するといいでしょう。
- p.108 第1段落の4行目
    - 誤：vtableというものを実現しています
    - 正：vtableを用いて実現しています
- p.108 第3段落の5行目
    - 誤：Base::Func
    - 正：`Base::Func`
- p.108 表4.4タイトル
    - 誤：クラスのvtable
    - 正：`Base`クラスのvtable
- p.110 第3段落の2行目
    - 誤：「第19 章　ページング」
    - 正：「**第19 章　ページング**」
- p.110 最終段落の1行目
    - 誤：図4.4
    - 正：**図4.4**
- p.137 リスト6.4タイトル
    - 誤：（graphics.hpp）
    - 正：（osbook_day06cのgraphics.hpp）
- p.143 表6.1
    - ビット位置「10:8」と「7:0」のフォントを、その他と揃える
- p.215 第3段落の1行目
    - 誤：**リスト 9.1** 1 に
    - 正：**リスト 9.11** に
- p.429 リスト18.18
    - リスト最終行と脚注1が重なってしまっている
    - リストの最終行は `v = v * 10 + (s[i] - '0');`
    - 脚注1は「＊1　RPN：Reverse Polish Notation」
- p.716 第1段落の4行目
    - 誤：WSL（**A.1** を参照）
    - 正：WSL（**A.01** を参照）
- p.726 リストC.3の2行目
    - その他の行と字間を揃える（均等割付をやめ、左詰めにする）
    - 誤：`␣␣␣U e f i A p p ……`
    - 正：`␣␣UefiApp……`
    - 字間を揃えた結果、インデントが半角空白2個となり、3行目（`␣␣UefiLib`）と揃うのが正しい
