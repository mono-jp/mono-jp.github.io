---
title: Documentation
redirect_from:
  - /Documentation/
  - /Class_Library_Documentation/
  - /Docs/
---

これらのドキュメントは、Monoのコンフィグレーションや、ランタイムやガベージ コレクターその他さまざまなMono固有のツールといったMonoの内部情報など、Mono固有の話題をカバーしています。

.NET Frameworkやクラスライブラリの一般的な情報については、Microsoft [MSDNのページ](http://msdn.microsoft.com/en-us/library/ff361664.aspx)が参照できます。

{% capture docNote %}
私達のドキュメンテーションは、[GitHub](https://github.com/mono/website/docs)上でオープンソースとなっています。もし間違いを見つけたり、ページが改善できると思ったら、ページ タイトルの下にある"Edit page on GitHub"のリンクをクリックしましょう。詳しくは[webサイトに協力する](https://github.com/mono/website#contributing-to-the-website)のセクションを見て下さい。
{% endcapture %}
{% include note.html type='info' message=docNote %}

はじめの一歩
-----------

 - [概要](/docs/getting-started/)
 - Monoをインストールする: [Mac OS X](/docs/getting-started/install/mac/), [Linux](/docs/getting-started/install/linux/), [Windows](/docs/getting-started/install/windows/)
 - [Monoの基本](/docs/getting-started/mono-basics/)
 - [開発環境](/docs/getting-started/development-environments/)
 - [アプリケーションの移植性](/docs/getting-started/application-portability/)と[アプリケーションのデプロイメント](/docs/getting-started/application-deployment/)

Monoについて
-----------

 - [概要](/docs/about-mono/)
 - [サポートするプラットフォーム](/docs/about-mono/supported-platforms/)
 - [言語](/docs/about-mono/languages/)
 - [互換性](/docs/about-mono/compatibility/)と[クラス ステータス](/docs/about-mono/class-status/) 
 - [リリース](/docs/about-mono/releases/)と[バージョンについて](/docs/about-mono/versioning/) 
 - [メンテナー](/docs/about-mono/maintainers/)
 - [履歴](/docs/about-mono/history/), [Monoの懸案事項](/docs/about-mono/concerns-about-mono/)
 - [ロードマップ](/docs/about-mono/roadmap/)と[開発計画](/docs/about-mono/plans/)
 - [脆弱性問題](/docs/about-mono/vulnerabilities/)
 - ショーケース: [スクリーンショット](/docs/about-mono/showcase/screenshots/), [ソフトウェア](/docs/about-mono/showcase/software/), [Monoを利用している企業](/docs/about-mono/showcase/companies-using-mono/), [Monoのロゴ](/docs/about-mono/logos/)

Monoをコンパイルする
------------------

 - [概要](/docs/compiling-mono/), ここにはOS X、Linux、Windowsでのコンパイル方法があります
 - [Gitからのコンパイル](/docs/compiling-mono/compiling-from-git/)と [Tarballからのコンパイル](/docs/compiling-mono/compiling-from-tarball/)
 - [高度なコンパイル オプション](/docs/compiling-mono/advanced-mono-compile-options/)
 - [サポートされていない高度なコンパイル オプション](/docs/compiling-mono/unsupported-advanced-compile-options/)
 - [Mono環境の並列セットアップ](/docs/compiling-mono/parallel-mono-environments/)
 - [最小フットプリント](/docs/compiling-mono/small-footprint/)

FAQ
---

 - [一般](/docs/faq/general/)
 - [セキュリティ](/docs/faq/security/)
 - [技術的な話題](/docs/faq/technical/)
 - [ライセンス](/docs/faq/licensing/)
 - [ドキュメンテーション](/docs/faq/documentation/)
 - [ASP.NET](/docs/faq/aspnet/)
 - [GTK](/docs/faq/gtk/)
 - [WinForms](/docs/faq/winforms/)

データベース アクセス
-------------------

 - [概要](/docs/database-access/)
 - [ADO.NET](/docs/database-access/adonet/)
 - [EntityFramework](/docs/database-access/entityframework/)
 
デバッグおよびプロファイリング
----------------------------

 - [デバッグ - 概要](/docs/debug+profile/debug/)
   - [デバッガー](/docs/debug+profile/debug/debugger/)
 - [プロファイリング - 概要](/docs/debug+profile/profile/)
   - [プロファイラー](/docs/debug+profile/profile/profiler/)
   - [HeapShot](/docs/debug+profile/profile/heapshot/)
   - [DTrace](/docs/debug+profile/profile/dtrace/)
   - [コード カバレッジ](/docs/debug+profile/profile/code-coverage/)

GUI
---

 - [GUIツールキット群](/docs/gui/gui-toolkits/)
 - [WinForms](/docs/gui/winforms/)
 - [Gtk#](/docs/gui/gtksharp/)
 - [Drawing](/docs/gui/drawing/)
 - [libgdiplus](/docs/gui/libgdiplus/)
 - [WPF](/docs/gui/wpf/)

Web
---

 - [ASP.NET](/docs/web/aspnet/)
 - [WCF](/docs/web/wcf/)
 - [FastCGI](/docs/web/fastcgi/)
 - [mod_mono](/docs/web/mod_mono/)
 - [Moonlight](/docs/web/moonlight/)
 - [ASP.NETアプリケーションを移植する](/docs/web/porting-aspnet-applications/)
 - [XSPでクライアント証明書を使用する](/docs/web/using-clientcertificates-with-xsp/)

ツールおよびライブラリ
--------------------

 - [ツール - 概要](/docs/tools+libraries/tools/)
   - [Gendarme](/docs/tools+libraries/tools/gendarme/)
   - [MoMA](/docs/tools+libraries/tools/moma/)
   - [XBuild](/docs/tools+libraries/tools/xbuild/)
 - [ライブあり - 概要](/docs/tools+libraries/libraries/)
   - [MonoMac](/docs/tools+libraries/libraries/monomac/)
   - [XML](/docs/tools+libraries/libraries/xml/)
   - [Mono.Cairo](/docs/tools+libraries/libraries/Mono.Cairo/)
   - [Mono.Cecil](/docs/tools+libraries/libraries/Mono.Cecil/)

高度な話題
---------

 - [ランタイム](/docs/advanced/runtime/)
 - [ガベージ コレクター - SGEN](/docs/advanced/garbage-collector/sgen/)
   - [GCベンチマーク スイート](/docs/advanced/garbage-collector/benchmark-suite/)
 - [AOT](/docs/advanced/aot/)
 - [組み込みランタイム](/docs/advanced/embedding/)
 - [アセンブリとGAC](/docs/advanced/assemblies-and-the-gac/)
 - [P/Invoke](/docs/advanced/pinvoke/)
 - [IOMap](/docs/advanced/iomap/)
 - [monolite](/docs/advanced/monolite/)
 - [Mono LLVM](/docs/advanced/mono-llvm/)
 - [CAS](/docs/advanced/cas/)
 - [COM](/docs/advanced/com/)
   - [COM-Interop](/docs/advanced/com-interop/)
 - [CoreCLR](/docs/advanced/coreclr/)
   - [CoreCLR HowTo](/docs/advanced/coreclr-howto/)
 - [パフォーマンスTips](/docs/advanced/performance-tips/)
 - [SafeHandles](/docs/advanced/safehandles/)
 - [Sandbox](/docs/advanced/sandbox/)
