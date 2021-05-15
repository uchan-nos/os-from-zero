## MikanOS のバグ修正方針

MikanOS の特定のタグ（osdook_dayX）に存在するバグは修正されません。その代わり、バグ報告の中で重要なものはこのページに掲載されます。
タグに対して修正を行うと、Git のコミット履歴を修正する必要が生じ、すでに mikanos リポジトリを clone した人に悪影響が出るからです。

master ブランチの最新コミットに存在するバグは、修正される可能性があります。
master ブランチに対するバグ報告は、サポートサイトの Issues ではなく、できるだけ mikanos リポジトリの Issues に投稿してください。

## MikanOS に存在する既知のバグ

- osbook_day15b ~ osbook_day16f: [osbook_day15b で実行後すぐにTaskBウィンドウが消える](https://github.com/uchan-nos/os-from-zero/issues/42)
- osbook_day06b: [ScanAllBus() で function=0 から探索すべき](https://github.com/uchan-nos/os-from-zero/issues/58)
