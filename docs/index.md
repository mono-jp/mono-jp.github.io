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
私達のWebサイトは、[GitHub](https://github.com/mono/website)上でオープンソースとなっています。もし間違いを見つけたり、ページが改善できると思ったら、ページ タイトルの下にある"Edit page on GitHub"のリンクをクリックしましょう。詳しくは[webサイトに協力する](https://github.com/mono/website#contributing-to-the-website)のセクションを見て下さい。
{% endcapture %}
{% include note.html type='info' message=docNote %}

<dl class="accordion" data-accordion>
    <dd class="accordion-navigation">
        <a class="panel" href="#getting-started"><h2>はじめの一歩</h2></a>
        <div id="getting-started" class="content panel active">
            <ul class="disc">
                <li><a href="/docs/getting-started">概要</a></li>
                <li>Monoをインストールする: <a href="/docs/getting-started/install/mac/">Mac OS X</a>,<a href="/docs/getting-started/install/linux/">Linux</a>,<a href="/docs/getting-started/install/windows/">Windows</a></li>
                <li><a href="/docs/getting-started/mono-basics/">Monoの基本</a></li>
                <li><a href="/docs/getting-started/development-environments/">開発環境</a> </li>
                <li><a href="/docs/getting-started/application-portability/">アプリケーションの移植性</a>と<a href="/docs/getting-started/application-deployment/">アプリケーションのデプロイメント</a></li>
            </ul>
        </div>
    </dd>

   <dd class="accordion-navigation">
        <a class="panel" href="#about-mono"><h2>Monoについて</h2></a>
        <div id="about-mono" class="content panel ">
            <ul class="disc">
                <li><a href="/docs/about-mono/">概要</a></li>
                <li><a href="/docs/about-mono/supported-platforms/">サポートするプラットフォーム</a></li>
                <li><a href="/docs/about-mono/languages/">言語</a></li>
                <li><a href="/docs/about-mono/compatibility/">互換性</a>と<a href="/docs/about-mono/class-status/">クラス ステータス</a></li>
                <li><a href="/docs/about-mono/releases/">リリース</a>と<a href="/docs/about-mono/versioning/">バージョンについて</a></li>
                <li><a href="/docs/about-mono/maintainers/">メンテナー</a></li>
                <li><a href="/docs/about-mono/history/">履歴</a> , <a href="/docs/about-mono/concerns-about-mono/">Monoの懸案事項</a></li>
                <li><a href="/docs/about-mono/roadmap/">ロードマップ</a>と<a href="/docs/about-mono/plans/">開発計画</a></li>
                <li><a href="/docs/about-mono/vulnerabilities/">脆弱性問題</a></li>
                <li>ショーケース: <a href="/docs/about-mono/showcase/screenshots/">スクリーンショット</a> , <a href="/docs/about-mono/showcase/software/">ソフトウェア</a> , <a href="/docs/about-mono/showcase/companies-using-mono/">Monoを利用している企業</a> , <a href="/docs/about-mono/logos/">Monoのロゴ</a></li>
            </ul>
        </div>
    </dd>

   <dd class="accordion-navigation">
        <a class="panel" href="#compiling-mono"><h2>Monoをコンパイルする</h2></a>
        <div id="compiling-mono" class="content panel ">
            <ul class="disc">
                <li><a href="/docs/compiling-mono/">概要</a>, ここにはOS X、Linux、Windowsでのコンパイル方法があります</li>
                <li><a href="/docs/compiling-mono/compiling-from-git/">Gitからのコンパイル</a>と<a href="/docs/compiling-mono/compiling-from-tarball/">Tarballからのコンパイル</a></li>
                <li><a href="/docs/compiling-mono/advanced-mono-compile-options/">高度なコンパイル オプション</a></li>
                <li><a href="/docs/compiling-mono/unsupported-advanced-compile-options/">サポートされていない高度なコンパイル オプション</a></li>
                <li><a href="/docs/compiling-mono/parallel-mono-environments/">Mono環境の並列セットアップ</a></li>
                <li><a href="/docs/compiling-mono/small-footprint/">最小フットプリント</a></li>
            </ul>
        </div>
    </dd>

   <dd class="accordion-navigation">
        <a class="panel" href="#faq"><h2>FAQ</h2></a>
        <div id="faq" class="content panel ">
            <ul class="disc">
                  <li><a href="/docs/faq/general/">一般</a></li>
                  <li><a href="/docs/faq/security/">セキュリティ</a></li>
                  <li><a href="/docs/faq/technical/">技術的な話題</a></li>
                  <li><a href="/docs/faq/licensing/">ライセンス</a></li>
                  <li><a href="/docs/faq/documentation/">ドキュメンテーション</a></li>
                  <li><a href="/docs/faq/aspnet/">ASP.NET</a></li>
                  <li><a href="/docs/faq/gtk/">GTK</a></li>
                  <li><a href="/docs/faq/winforms/">WinForms</a></li>
            </ul>
        </div>
    </dd>

   <dd class="accordion-navigation">
        <a class="panel" href="#database-access"><h2>データベース アクセス</h2></a>
        <div id="database-access" class="content panel ">
            <ul class="disc">
                <li><a href="/docs/database-access/">概要</a></li>
                <li><a href="/docs/database-access/adonet/">ADO.NET</a></li>
                <li><a href="/docs/database-access/entityframework/">EntityFramework</a></li>
            </ul>
        </div>
    </dd>

   <dd class="accordion-navigation">
        <a class="panel" href="#debug-and-profile"><h2>デバッグおよびプロファイリング</h2></a>
        <div id="debug-and-profile" class="content panel ">
            <ul class="disc">
                <li><a href="/docs/debug+profile/debug/">デバッグ - 概要</a>
                    <ul>
                        <li><a href="/docs/debug+profile/debug/debugger/">デバッガー</a></li>
                    </ul>
                </li>
                <li><a href="/docs/debug+profile/profile/">プロファイリング - 概要</a>
                    <ul>
                        <li><a href="/docs/debug+profile/profile/profiler/">プロファイラー</a></li>
                        <li><a href="/docs/debug+profile/profile/heapshot/">HeapShot</a></li>
                        <li><a href="/docs/debug+profile/profile/dtrace/">DTrace</a></li>
                        <li><a href="/docs/debug+profile/profile/code-coverage/">コード カバレッジ</a></li>
                    </ul>
                </li>
            </ul>
        </div>
   </dd>

   <dd class="accordion-navigation">
        <a class="panel" href="#gui"><h2>GUI</h2></a>
        <div id="gui" class="content panel ">
            <ul class="disc">
                <li><a href="/docs/gui/gui-toolkits/">GUIツールキット群</a></li>
                <li><a href="/docs/gui/winforms/">WinForms</a></li>
                <li><a href="/docs/gui/gtksharp/">Gtk#</a></li>
                <li><a href="/docs/gui/drawing/">Drawing</a></li>
                <li><a href="/docs/gui/libgdiplus/">libgdiplus</a></li>
                <li><a href="/docs/gui/wpf/">WPF</a></li>
            </ul>
        </div>
    </dd>

   <dd class="accordion-navigation">
        <a class="panel" href="#web"><h2>Web</h2></a>
        <div id="web" class="content panel ">
            <ul class="disc">
                <li><a href="/docs/web/aspnet/">ASP.NET</a></li>
                <li><a href="/docs/web/wcf/">WCF</a></li>
                <li><a href="/docs/web/fastcgi/">FastCGI</a></li>
                <li><a href="/docs/web/mod_mono/">mod_mono</a></li>
                <li><a href="/docs/web/moonlight/">Moonlight</a></li>
                <li><a href="/docs/web/porting-aspnet-applications/">ASP.NETアプリケーションを移植する</a></li>
                <li><a href="/docs/web/using-clientcertificates-with-xsp/">XSPでクライアント証明書を使用する</a></li>
            </ul>
        </div>
    </dd>

   <dd class="accordion-navigation">
        <a class="panel" href="#tools-and-libraries"><h2>ツールおよびライブラリ</h2></a>
        <div id="tools-and-libraries" class="content panel ">
            <ul class="disc">
                <li><a href="/docs/tools+libraries/tools/">ツール - 概要</a>
                    <ul>
                        <li><a href="/docs/tools+libraries/tools/gendarme/">Gendarme</a></li>
                        <li><a href="/docs/tools+libraries/tools/moma/">MoMA</a></li>
                        <li><a href="/docs/tools+libraries/tools/xbuild/">XBuild</a></li>
                    </ul>
                </li>
                <li><a href="/docs/tools+libraries/libraries/">ライブラリ - 概要</a>
                   <ul>
                      <li><a href="/docs/tools+libraries/libraries/monomac/">MonoMac</a></li>
                      <li><a href="/docs/tools+libraries/libraries/xml/">XML</a></li>
                      <li><a href="/docs/tools+libraries/libraries/Mono.Cairo/">Mono.Cairo</a></li>
                      <li><a href="/docs/tools+libraries/libraries/Mono.Cecil/">Mono.Cecil</a></li>
                   </ul>
                </li>
            </ul>
        </div>
    </dd>

   <dd class="accordion-navigation">
        <a class="panel" href="#advanced-topics"><h2>高度な話題</h2></a>
        <div id="advanced-topics" class="content panel ">
            <ul class="disc">
                <li><a href="/docs/advanced/runtime/">ランタイム</a></li>
                <li><a href="/docs/advanced/garbage-collector/sgen/">ガベージ コレクター - SGEN</a>
                    <ul>
                        <li><a href="/docs/advanced/garbage-collector/benchmark-suite/">GCベンチマーク スイート</a></li>
                    </ul>
                </li>
                <li><a href="/docs/advanced/aot/">AOT</a></li>
                <li><a href="/docs/advanced/embedding/">組み込みランタイム</a></li>
                <li><a href="/docs/advanced/assemblies-and-the-gac/">アセンブリとGAC</a></li>
                <li><a href="/docs/advanced/pinvoke/">P/Invoke</a></li>
                <li><a href="/docs/advanced/iomap/">IOMap</a></li>
                <li><a href="/docs/advanced/monolite/">monolite</a></li>
                <li><a href="/docs/advanced/mono-llvm/">Mono LLVM</a></li>
                <li><a href="/docs/advanced/cas/">CAS</a></li>
                <li><a href="/docs/advanced/com/">COM</a>
                    <ul>
                        <li><a href="/docs/advanced/com-interop/">COM-Interop</a></li>
                    </ul>
                </li>
                <li><a href="/docs/advanced/coreclr/">CoreCLR</a>
                    <ul>
                        <li><a href="/docs/advanced/coreclr-howto/">CoreCLR HowTo</a></li>
                    </ul>
                </li>
                <li><a href="/docs/advanced/performance-tips/">パフォーマンスTips</a></li>
                <li><a href="/docs/advanced/safehandles/">SafeHandles</a></li>
                <li><a href="/docs/advanced/sandbox/">Sandbox</a></li>
                <li><a href="/docs/advanced/signals/">シグナルとサードパーティー製クラッシュレポーター</a></li>
            </ul>
        </div>
    </dd>
</dl>
