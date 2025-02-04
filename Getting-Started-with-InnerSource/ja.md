# チーム間コラボレーションへの強力なアプローチ

近年、オペレーティングシステム、クラウドコンピューティング、JavaScript フレームワークをはじめとするさまざまな OSS(Open Source Software: オープンソースソフトウェア) の普及に触発され、_インナーソース_ という標語のもと、その強力な OSS 由来のプラクティスを模倣して内部のコラボレーションに取り入れようとする企業が増えています。
このページでは、インターネット商取引の大手である PayPal の経験から、インナーソースがエンジニア、経営者、マーケティング/PR 部門にどのような利益をもたらすかを見ていきます。

インナーソースによるプロジェクトマネジメントの魅力を理解するために、そもそも OSS 開発がなぜここまで成功してきたのか、その要因を考えてみましょう。

* プログラマーは、マネージャーやチームだけでなく、ユーザーやコントリビューターといった幅広い人々と自分の仕事を共有します。ほとんどの OSS プロジェクトでは、世界中の誰もが自由にコードをみることができ、コメントを残し、検証することにより新しいスキルを学ぶことができ、また、ニーズに合わせてカスタマイズしたり、改善したコードの変更を提出することができます。
* 該当プロジェクトをもとにした新しいコードリポジトリ(ブランチ)を自由に作成できるため、コードが元々に作られた目的以外の使用にも対応できます。通常、さまざまなブランチを元のマスターブランチにマージするためのルールと、それを支援する技術があります。
* 地理的に離れた場所にいる人々が、別々の時間に、同じコードで作業したり、同じプロジェクトに異なるコードのファイルを提供することができます。
* コミュニケーションは、口頭で非公式に共有されるのではなく、文書化されて公の場に投稿される傾向があり、それはプロジェクトの履歴を残すことになり、また新しいプロジェクトメンバーに学習の機会を提供することになります。
* ユニットテストの作成は、重要なプログラミングタスクになります。「ユニットテスト」は、誤った入力を拒否したり、特定の条件下で適切な分岐を行ったりするなど、特定の孤立した動作をチェックする小さなテストです。オープンソースとインナーソースでは、本番稼働中の障害からの保護のために、変更がチェックインされる際、テストが常に実行されます。

単一の組織における見地と制御の範囲内にとどまるという点で、インナーソースは従来のオープンソースとは異なります。
プロジェクトの"オープン性"は組織内に限定されますが多くのチームにまたがります。
これにより、組織は部外者にコードが公開されることを恐れることなく、競争の源泉である企業秘密をコードに埋め込むことができます。
同時に、組織全体にわたる人々によって提供される多様な視点やクリエイティビティの恩恵を受けることができます。

組織がインナーソースプロジェクトの一部を一般に公開し、それらを効果的に OSS に変えることを選択するケースもよくあります。
OSS の技術と管理手法が社内で使用されていれば、プロジェクトを公の場に移すことは非常に容易になります。

インナーソース戦略を採用する利点は以下の通りです。

* 組織横断的なコードの再利用が飛躍的に進みます。各チームのプログラマーは、他のチームによって開発されたモジュールのコードとアーキテクチャを理解し、コードをコントリビュートすることができます。
* このようなチーム間のコラボレーションが、比較的摩擦の少ないものになります。受け取ったチームがコントリビュートされたコードを書き直すことはほとんどなくなり、上層部における議論も必要なくなります。
* プログラマーはユニットテスト、コードカバレッジ、継続的インテグレーションを使い、開発の初期段階でバグを取り除くことを学ぶことができるため、開発はより速くなります。チームメンバー間で交わされるコメントのやり取りには時間がかかりますが、新しいプログラマーがシステムについて早く学ぶことができるようになるため、それ以上の効果があります。
* プログラマーは自分のコードをより良く文書化することを学ぶようになり、それは公式なドキュメント(コード内のコメントや文書)や、非公式なドキュメント(ディスカッションリスト) に対しても効果があります。ドキュメントはプロジェクトの履歴を提供して外部の人間が理解する助けになるため、より多くの人がプロジェクトにコントリビュートできるようになります。

## OSS の原則が機能する場

インナーソースがあなたの組織に対して何をもたらすかを考える前に、これらのプラクティスの源泉であるであるフリーでオープンソースのソフトウェアムーブメントがうまく機能している場所と、歴史的にあまり成功していない場所について考察することが重要です。

### 組織横断的なコラボレーション

OSS の開発は、チーム・企業・国の境界を越えて、世界中の個人が Linux や Apache のような主要なコンピューティングシステムの進歩に協力することを可能にします。
無骨なハッカーがどこかの地下室でコードを書くというステレオタイプは(かつてそれが適切だったとしても)時代遅れです。
Linux のような OSS プロジェクトにおける中心的なコントリビューターは、今や大企業に勤めています。

多くの重要な OSS プロジェクトは、個々のプログラマーによる発案から始まりましたが、それはよく大企業に採用されていきます。
また、PayPal をはじめとして、大企業の中から OSS プロジェクトが生まれるケースもあります。
どのような組織であっても OSS の成功に欠かせないのは、内部の人々が、外部の人々にソフトウェアにおける開発・テスト・文書化・プロモーションの主要な役割をさせることと、すべてのコントリビューターに可能な限り公平な競争の場を提供することです。

### 地理的に分散した開発とアジャイルなプログラミングの違い

OSS の国境を越えた活動は、アジャイルやスクラムのような一般的な企業の開発アプローチと強く対照的です。
後者の開発手法は、1 つのオフィスで顔を合わせて仕事をするチームのために設計されたものであることは明らかです。
このようなプロジェクトでは、開発者は一緒に仕事をするだけでなく、ソフトウェアユーザーやその他のステークホルダーと定期的に会わなければなりません。
このような非公式な情報共有により、ドキュメンテーションや正式な要件の必要性を減らすことができます。
しかし、このような開発手法は、単一の作業現場ではないようなより大きな環境においては、あまり上手くいきません。

アジャイルやスクラムが拡張性という代償を払うとすれば、OSS 開発はスピードという代償を払うことになります。
OSS プロジェクトは、1 つのオフィスで働く専門チームほど速く動くことができません。
締め切りが(時には狂気的なほど)厳しいスタートアップ・ベンチャーにとって、この代償は明らかに大きな違いとなります。
この違いは、[インフラのための価値](#インフラのための価値)で説明するように、それぞれの開発モデルに適したソフトウェアの種類にも微細な影響を及ぼします。

進行速度に制限があるにもかかわらず、多くの OSS プロジェクトは、厳しい納期を守り、予測可能なリリースを行っています。
しかし、予測可能性を高めるために機能を犠牲にすることも少なくありません。
特定のリリースで計画されている機能を拡張することの中には、期限を過ぎないように後回しにしなければならないものも含まれているかもしれません。

実を言うと、アジャイルなプログラミングは必ずしも OSS 開発の敵ではありません。
実際、文献においてこの2つを組み合わせたチームが報告されています [^stol2014]。
しかし、彼らにおいては要件と前提が異なるということを理解することが、OSS をよりよく理解することに繋がるでしょう。

### 継続的なテストと開発
大半の OSS プロジェクトでは、寄せられるコントリビューションの一つ一つを厳しく客観的にテストする仕組みを設けています。
これにより品質は保たれ、協力者間の信頼も醸成されます。
例えば、ユニットテストや継続的インテグレーションといった標準的な技術が採用されており、それらの技術を正しく使うための規範も徹底されています。
OSS 開発者は品質管理をより科学的にしているのです。

OSS においてテスト駆動開発は求められないものの、ユニットテストは非常に重視されています。
コントリビューション対象の OSS プロジェクトにおける品質保証チームの有無にかかわらず、コントリビューターは自身の書いたコードを保証するためのユニットテストも合わせて書くことが求められます。
コードを変更するにはテスト実行ツールと所定の手続きが必要であり、変更がリポジトリに取り込まれるためにはテスト結果が潔白であることが求められます。
こうすることにより、変更されたコードが意図通りに動くことだけでなく、それ以外のコードに悪影響がないことも確かめられるのです。

コードカバレッジの測定や静的コード解析といった現代的な技術は、OSS の世界ではさほど見かけませんが、PayPal では積極的に使われています。

まとめると、テストと継続的インテグレーションは 2 つの重要な役割を担っています。
まずひとつは勿論のこと、プロダクトが壊れないようにすることです。
ですが、それだけではなく、大きな責任を持つに相応しい開発者を見つけるのにも役立つのです。
例えば、_トラステッドコミッター_ [^trusted-committer] という憧れの称号に相応しい開発者を見つけるには、受け入れられたコミットの数で判断することが通例です。
トラステッドコミッターは、他の開発者の成果をレビューして採否を判定する役割を持ちます。
また、自身はそうしたレビュープロセスを経ることなく変更する権限を持ちます。
さらに、品質基準を満たさないコードを提出した伸び盛りの開発者を育てる役割も担います。

### 明文化の重要性 [^documentation]

さらなる OSS の信念は徹底的な明文化です。
これは、関係者の地理的な位置とタイムゾーンが多様であることに起因しています。
ユーザー向けドキュメントは多くの OSS プロジェクトで手薄になりがちなのですが(実はプロプライエタリプロジェクトでも同様に手薄です)、開発者の考える想定、意志決定、実装については積極的に記されます。

こうした実状は「包括的なドキュメントよりも動くソフトウェアを」優先する[アジャイルソフトウェア開発宣言](https://agilemanifesto.org/iso/ja/manifesto.html)とは対照的です。
OSS コミュニティ(という開発者中心の世界)でも動くソフトウェアが正義とされるものの、実現できた事柄についてはドキュメントに残すことが依然として重視されています。
これは一般的なアジャイルに対する特徴として覚えておくべきことです。

OSSにおける議論や状況説明といったあらゆるコミュニケーションは明文化されます。
例えば、多くのプロジェクトで GitHub に書き込まれるコメントが開発を左右していることでしょう。
メーリングリストは議論による意思決定に欠かせないツールとなっているでしょう[^mailing-list]。
「メーリングリストに書かれていることだけが事実だ」という言い回しを聞いたことのある読者も多いのではないでしょうか。

意思決定と実装の詳細を明文化することの価値として、新たに参加しようとする人々のためにプロジェクトの歴史を綴ることが挙げられます。
時間をかけて経緯を読み解けば、プロジェクトの文化や学びのある経験を誰でも知ることができるのです。

そして、協働するには同じ言語を用いる必要があることにも注意が必要です。
関わる人々が地理的にばらばらである OSS プロジェクトでは、ご存知の通り英語が共通言語となっています(他の言語を用いる重要なプロジェクトもありますが)。
読み書きの方が会話よりも民主的なコミュニケーションを促します。
なぜなら外国語を流暢に話せるようになるよりも、書けるようになる方が簡単だからです。
よって、多くの人々は、結束力は高いものの馴染みのない言語を使うチームよりも、OSS プロジェクトに参加できるのです。

### インフラのための価値

OSS は低レイヤーで成功してきました。
ここで言う低レイヤーとは、OS、ハイパーバイザー、コンパイラーやエディターといった開発者が使うツール、コードの脆弱性を見つけるためのセキュリティツール、その他ユーザーに見えない場所に置かれているものが該当します。

一方、ユーザーインターフェース(UI)はそうではなく、OSS として開発することに根強い反発があることがわかっています。
エンドユーザー向けの OSS として広く普及したものはなかなかありません。
Mozilla Firefox は珍しい例なのです。

その理由を知るヒントは、[OSS 開発とアジャイル開発の比較](#地理的に分散した開発とアジャイルなプログラミングの違い)を読み返すとわかるでしょう。
アジャイル開発が広く採用されている理由は、開発者がユーザーとの密接な対話を続けられる方法だからです。
対話を通じたフィードバックを得てから数日のうちに作業を始められます。
一方、ほとんどの OSS プロジェクトでは、α 版や β リリースといった昔ながらの方法でユーザーの反応を得ています。

[ユニットテストに重点を置いていることも](#継続的なテストと開発)、OSS がインフラに向いていることを表しているでしょう。
アジャイルの専門家である Mike Cohn は、2009年にテストピラミッド[^test-pyramid] という概念を提唱しました。
この概念では、UI のテストを最上位、ユニットテストを最下位とした複数の階層が設けられ、ユニットテストを最も重視して機能テストとの依存を減らすことが説明されています。

UI をユニットテストで確認することは困難であり、できたとしてもその信頼性と価値は低いものになってしまいます。
そこで、システム全体の動作と、ユーザーの操作が期待する結果を生むことを確認できる機能テストの出番というわけです。

要するに、OSS の品質と信頼を盤石なものとするテストプロセスにおいて、UI のテストは弱いのです。
このことも、UI を持つ OSS が少ない理由かもしれません。

### OSS に相応しいレベルの発見

OSS とフリーソフトウェアは、Microsoft の Windows や Oracle の Database といったプロプライエタリソフトウェア[^proprietary-software]と比較されてきました。
現在では、SaaS(Software as a Service)という提供モデルがプロプライエタリソフトウェアの開発で一般的になってきました。
SaaS では [^not-only-SaaS]、どの部分を何の方法で開発するかを決めることになります。
インナーソース か、オープンソースか、あるいはアジャイルのような関係者を限定するチーム志向の方法なのかという選択です。
この選択には本章がガイドラインとして役立つでしょう。

多くの企業では、いくつかを組み合わせた選択をしています。
そうした企業は、ビジネスのコアとなるソフトウェアを SaaS の背後に隠しておく一方で、インフラに相当するソフトウェアを自由に公開・共有しています。
また、そのような企業は[クローズドコア](http://radar.oreilly.com/2011/12/could-closed-core-prove-a-more.html)と呼ばれることがあります[^closed-core]。
インフラ部分を OSS にすることにより、プログラミングに関わる数多の人々が利益を受け、社員の採用と教育が効率的になり、企業は外からのコントリビューションを受け取ることができるようになるのです。

## PayPal が インナーソース を採用するまで

PayPal が インナーソース を採用するまでの過程には企業としての意志決定の積み重ねがあり、歴史的で大規模なものです。
インナーソース の採用は、それまでに何度かあった企業変革と同様に、ツールと企業文化の戦略的変更として進められました。

PayPal が インナーソース を採用する以前に行われた変革とその結果は次の通りです。

* 開発速度を向上させる技術の調査と適用 (例：多くのプロジェクトが Java から JavaScript または Node.js に移行した)
* 採用した新技術に関係する OSS コミュニティと開発モデルへの興味が醸成された
* 社内と社外どちらの協働でも GitHub が使われるようになった
* 品質に高い関心が払われるようになった

つまり、PayPal では インナーソース を採用する前からオープンソースにゆかりのある技術を部分的に採用していたということです。
また、一部の社内用コードを OSS 化することにも取り組みました。
逆の順序、すなわち社内という限られた空間で OSS 由来の方法を実践してから OSS を公開するという道を辿る企業もいることでしょう。
ただ、その方が一般的に難しいと考えられています。
どちらの順序にしても、OSS のツールと、協働的な開発プロセスを促進する GitHub のようなツールを熟知していることが重要です。

PayPal における様々な変化は同時に発生し、明らかに相互に影響しています。
以降の節ではそれらを紐解き、各変化を個別に説明してゆきます。

### 末端から始める

PayPal のインナーソースは、米国外で働く地域セールスエンジニアから始まりました。
彼らは、各地域の利用者の好みに合わせたり、地域向けのプロモーションに役立てるためにユーザー向けのコードを修正しました。
しかし、そうしたプログラマーたちが行った変更が、すぐにコアチームに受け入れられるわけではありませんでした。
バイスプレジデントなどが介入してマージを求め、そのあとで反対するコアエンジニアがマージ前に変更を書き戻すこともありました。

その一方で、他のチームの開発者との間で飛び交う緊急の E メールのやり取りで、不十分なドキュメントをカバーしていました。
これらのメールには重要な情報が含まれていましたが、その他の多くの開発者が目にすることはありませんでした。
多くの地域組織では、そうしたメッセージをそれぞれ独自の Wiki にカット＆ペーストする試みを始める始末でした。

多くの地域のエンジニアがサンノゼの本社に飛んできて、1ヶ月間コアチームから直接教えを受けました。
しかし、信頼できるコミッターを育てる手法としては、知識を十分に広めたとはいえず、投資に見合うものではありませんでした。
ドキュメントの作成も進みませんでした。
エンジニアたちが母国に帰国した後は、遠方のため、文書による問い合わせを通じて、コアメンターシップを探すことを余儀なくされました。

その結果、インナーソースのほうが良い方法かもしれないと考えられました。
各チームはインナーソースによってプロジェクトが本当に効率化することに気づきました。
そして、コア側の信頼できるコミッターも、そのプロセスがはるかに優れていることに気づきました。
リモートエンジニアは GitHub からコードサンプルをプルすることができました。

コアチームは、より上手に各地域のコラボレーターたちと連携する方法を学べただけでなく、地域のコントリビューターたちへの指導を通じて、モジュール性と理解しやすさを高めるためにコアコードのどこをリファクタリングすればよいかのヒントを得るようになりました。
また、異なる地域で行われた作業のパターンに気づくことができたため、経験豊富な地域のエンジニアを、他の地域の仲間のメンターに採用することができました。

### よりスピーディな開発プロセス

PayPal の黎明期は比較的モノリシックな C++ プラットフォームでスタートしました。
その後、レガシーな要素は C++ が残りながらも、新規開発については Java の Spring を使って、よりモジュール化された方法で行われるようになりました。
その移行後も、開発者の Jeff Harrell が言うには、各製品に多くの「部族内知識」が埋め込まれていました。
そのため、小さな変更であっても導入には数週間が必要で、新入社員には6週間のトレーニング期間が必要だったのです。

3年前、PayPal は Node.js を採用し、大きな変化を遂げました。
PayPal の Node.js 開発者である Poornima Venkatakrishnan によると、Node.js のプラットフォームはまずプロトタイピングのために使用されました。
その結果に満足した開発者たちは、本番環境に導入したいと考えました。
まずは Spring プラットフォームと Node.js で同じ機能を並行して開発する実験を試みました。
開発時間・コード行数・開発に必要なエンジニアの数などを基準に、二つのプラットフォームを比較したのです。
Node.js は明らかに勝っていました。

PayPal が Node.js を採用するという発表は、多くのプログラマーを、特に C++ から Java への移行が長くて大変だったことを記憶しているプログラマーを心配させました。
しかし、PayPal は、Node.js への移行がまったく違うものであることを示しました。
PayPal は、移行トレーニングにわずか2日間のスケジュールを組みました。
Harrell によると、参加者はすぐに、自分たちが新しく、活気があり、エキサイティングな世界に入ったことを実感したといいます。
さらに、JavaScript の分野のリーダーである Douglas Crockford をトレーニングのスタッフとして迎えられたことも幸運でした(Crockford は、非常に人気の高い書籍 _[JavaScript: The Good Parts](http://shop.oreilly.com/product/9780596517748.do)_ の著者であり、オライリーの _[JavaScript Master Classビデオ](http://shop.oreilly.com/product/9780596809614.do)_ の制作者でもあります)。

現在、PayPal の新機能開発チームの大半は Java を利用していますが、その一方で、Node.js チームが開拓したインナーソースのプラクティスを採用しているチームが存在します。

### OSS との関わり

Node.js に移行するためのトレーニングは、多くの教材がオンラインで利用できたことと、Node.js は前回の Java への移行に比べてカスタマイズの必要性が少なかったことから、簡単に短時間で実施できました。
また、スタッフが自分自身の学習プロセスを継続できるよう準備するには、基本的に2日間のトレーニングで十分でした。

Harrell によると、基本的な情報は社内のメーリングリストでシニアプログラマーに尋ねる代わりに、単に StackOverflow などのサイト (あるいは検索エンジンなど) で検索すれば良いということを PayPal のプログラマーに伝えるのに時間がかかったそうです。
しかし、やがて情報の問い合わせは OSS コミュニティへのひたむきな取り組みにまで広がりました。

多くの企業は OSS の技術が単に高品質で無料であるということで魅力的を感じる一方、採用することで OSS コミュニティへの継続的な参入につながると考えています。

これが PayPal が Node.js を採用したときに起こったことです。
今では Node.js はかなり成熟した技術になっています。
ピークを過ぎ、JavaScript プログラマーは代わりの技術を探していると指摘するコメンテーターもいるほどです(本節の後半で説明するように、OSS 技術の変化のペースによって、採用するテクノロジーに関する意思決定が変わります)。
しかし、PayPal が Node.js コミュニティに参入したのはコミュニティの初期段階でした。
そのため十分にコントリビューションする余地があったのです。
PayPal は、Node.js Foundation と ECMAScript Technical Committee 39 の会員となり、非常に積極的に活動をしました。

プログラマーの自己学習と新規採用社員の即戦力化という2つの目標を促進するため、PayPal は JavaScript と Node.js へ移行する際に、他の人気の OSS のツールを積極的に導入しました。
例えば、テストには広く使われている Selenium、継続的インテグレーションには Jenkins、Java のテストには TestNG、JUnit、Mockito といった具合です。
その過程で、PayPal は、[Nemo](https://github.com/paypal/nemo) (当初は Matt Edelman によって開発されました)や、[SeLion](http://selion.io)、そして [Illuminator](https://github.com/paypal/Illuminator) といった、OSS のコンポーネントと互換性のあるツールをいくつか開発し OSS で提供しました。

PayPal が Node.js を採用したのは開発初期であったため、いくつかのツールが不足していました。
そこで PayPal はこの機能不足を解消するために Node.js アーキテクチャを制御するフレームワークである [Kraken](http://krakenjs.com/) を開発しました。
他の PayPal の社内コードで見るような「部族内知識」から解放され、一般的な価値を持たせるためにチーム自身がこの Kraken を OSS として開発すると決めたのだと Harrell はいいます。
Kraken はおそらく彼らの最も成功した OSS プロジェクトになりました。

Venkatakrishnan は、この時 PayPal に導入した OSS 由来のプラクティスを次のように挙げています。

* 高い品質基準を設定すること。コードをコミットする前にコードカバレッジテストが実行され、カバレッジが少なくとも90%以上でなければならない。コードのプッシュに対して自動ビルドが実行され、そのコードがマージされるのに十分な品質があるか確認される必要がある。
* リポジトリにあるすべてのコードに対して、ドキュメントを必須とすること。
* すべてのディスカッションを GitHub 上で行うこと。これにより、チーム外の人々からの意見収集が促進され、コラボレーションが可能になる。社内プロジェクト用のプライベートな GitHub リポジトリと、OSS 用のパブリックな GitHub リポジトリを設ける。
* すべての専門知識を単一のチームから得る必要はないとエンジニアに教えること。OSSでは、世界中のどこからでも支援を受けることができる。OSS プロジェクトにコントリビュートすることで、会社の知名度が上がり、コミュニティに対するコミットメントを示すことができる。
* チームで行った仕事に対する誇りを育み、その成果をカンファレンスで話したり、PayPal の技術ブログに書いたりするよう奨励すること。

Harrell はソフトウェアスタックの上位に行けば行くほど、技術の変化が激しいと指摘しています。
この技術の変化はソフトウェア開発においては常に付きまとうものであり、OSS であればなおさらです。
そのため PayPal はチームに対し、絶えず自分たちのスキルを評価することを推奨しています。
開発者たちには継続的に学習することが期待されているのです。

代替ツールの評価は、必然的にチームごとに採用するツールが異なるという多様性をもたらします。
開発者の Matt Edelman は、この現象は OSS に特によく見られると指摘しています。
なぜならプログラマーは、Unix の父である Ken Thompson が提案した「多くの小さなプログラムが一緒に動く」という言葉に沿ってツールを開発するのが好きだからです。

そのため PayPal のチームでは React や Angular など、さまざまな最新技術が使用されています。
ただプログラマーには、ライブラリを推奨する前にパイロットプロジェクトで試し、代替案をよく比較した上で選択することが求められます。

OSS のアーキテクチャは、機能の拡張を可能にするプラグインを備えていることがよくあります。
Edelman によると、PayPal は Kraken のプラグインの一部を社内で (インナーソースモデルを通じて) 開発し、その他を OSS として開発しているそうです。

### GitHub コラボレーション

ある企業がモダンなコード開発において特殊な重要性を持つ地位を築いています。
それは GitHub です。
もともとは開発を容易にするためのバージョン管理ソフトウェアであるGitを用いたSaaSプラットフォームでしたが、現在では開発者が欠かせないと感じる機能を備え、非常に洗練されたコラボレーションプラットフォームへと進化しました。
詳細については次の2点が参考になります [Git for Teams](http://shop.oreilly.com/product/0636920034520.do)と [Collaborating with Git video](http://shop.oreilly.com/product/0636920034872.do) です。

PayPal では、Kraken のように OSS プロジェクトのコードを GitHub に置くだけでなく、社内に GitHub Enterprise を設置することで、社内のプログラマーがパブリックの GitHub のユーザーと同じようにコラボレーションできるようにしています。
コードレビューやコミット、テストは OSS と同じように行われますが、社内リポジトリの上で行われています。
最も重要なことは、PayPal の各チームメンバーがチーム外部のプログラマーからも新しいコードを受け取るという事が習慣化されているという事です。

Edelman によると、GitHub とインナーソースに移行する前は、PayPal のプログラマーは他のチームに対しては小さなバグ修正を提供するくらいしかできなかったと言います。
もし彼らがより大きなまとまりのコードを提供をする場合、受け取ったチームはコードを精査し、場合によってはゼロからコードを書いた場合と比べて変わらないような事がたまに起きていました。
チーム間でのコードのやりとりについては、高いレベルのマネージャが関与しなければならないこともしばしばでした。

しかし最近では、新機能に対して大幅に書き換える事なくチェックインできるようになりました。
その理由の1つは、ドキュメントに対する新しい考えです。
インナーソースのプロジェクトは、システムを深く理解する少数の特権を持つプログラマーだけでなく、より多くの社内プログラマの上に成り立っていなければならないと Edelman は強調しています。
誰もがプロジェクトを学習し、大きな仕様変更が発生するような提案もすることができるのです。

また、ドキュメント(コードと GitHub のコメントの両方)によって、開発者はアーキテクチャ変更の必要性を理解するようになります。
仮にあなたももし4回に分けて様々な人に、なぜそれが複雑になっていて直感的ではなのかを説明しなければならないとしたら、考え方が変わるでしょう。

また、プログラマーが国を超えて力を発揮することで、知的な成長や仕事のやりがいを感じるようになります。
プログラマーは、コードの設計についてより包括的に考えるようになり、同時にコードレビューやテスト、ドキュメントの書き方などの新しいスキルも身につけることができます。
インナーソースは "全員のパフォーマンスを底上げする" と、Edelman は言っています。

Edelman は、コアインフラストラクチャ内のモジュールで見つかったあるセキュリティ関連のバグについて言及しています。
ある機能が、仕様書(RFC)に正確に沿っていなかったのです。
当初、インフラ・チームの外から彼らに対して修正するように圧力がかかり、多くのメールが飛び交いました。
しかし、ある外部のメンバー(セキュリティは専門外)が RFC を見て、自分でも修正できることに気づいたのです。
そして、その修正案を提出したところ、コアインフラチームがすぐにそれをマージしてくれました。
この逸話は、プログラマーが自発的に行動することの重要性と、きちんと文書化された標準に従うことの価値という、2つの原則を示しています。

### 品質の向上

同時期に、PayPal はプラットフォームの大部分を Node.js に移行し、OSS のプラクティスを採用しつつ、品質向上への取り組みを開始しました。
品質保証のリーダーである Doug Simmons によると、PayPal のこの目標に向けたステップは以下の通りでした。

* より多くのユニットテスト
* 継続的インテグレーション
* コードレビュー
* より多くのコードカバレッジレポート
* 静的解析

すべての会話が公の場で行われる必要はありませんが、GitHub のコメントプロセスはいくつかの点で品質を向上させています。
トラステッドコミッターは、自分のコードをリポジトリに受け入れたいと願っている新人プログラマーのメンターとしても効果的に機能します。
投稿者とトラステッドコミッターの間で交わされるコメントのやりとりは、投稿者にとっても他のプログラマーにとっても、見ながら学習ができる良い教材となります。

### 文化の変化

インナーソースの採用という大きな企業の動きには、従業員の不安と期待への慎重な対応が求められます。
PayPal はこの変化を支援するために、外部の OSS 開発専門家を雇用しました。

多くの企業のオブザーバーは、従業員が他チームにコードを提供する事への自信を与えることが、最も重要な文化的変化だと同意しているようです。
これは、完全なドキュメンテーションと優れたメンタリングで達成できますが、 Edelman は、スタッフの習慣を、バグに苦情を言うものから修正するものへ変えなければならないと指摘しています。

Harrell は、チームメンバーを説得して、チーム外の PayPal プログラマーがコントリビューションできるようにしたことを覚えています。
チームメンバーは、外部のコードのチェックにばかり時間をとられ、自分たちがコードを書けなくなるのではないかと、よく反対していました。
別の企業の調査では、新しいコントリビューションは自分のメンテナンスの手間を増やすことになると、プログラマーが心配していました [^stol2011]。

しかし、厳密なテストとビルドプロセスでコントリビューションの質を確保していたため、これらの欠点は予想より少なかったことはご承知のとおりです。
いずれにしても、コントリビューションのチェックには高いスキルが必要だと、 Harrell は述べています。
そして、コントリビューションはチームが作成したコードの価値を高めていきました。

Edelman は、「モジュールの作者には、品質と一貫性の基準を維持しつつ、コミュニティからのフィードバックや変更に対してオープンであることで、ソフトウェアの価値を高めていくことが期待されます」と述べています。
彼によると、開発者はテストを書いたりコードレビューをしたりすることへの不満から、それを主張するようになったそうです。

品質面では、プログラマーがインナーソースのバグレポートを提出すると、まずはモジュールの担当者に送られます。
このプログラマーは、そのバグレポートを影響を受けるコードのコントリビューターに渡すことができます。

モジュラーアーキテクチャと明確な API 定義は、チーム外からのコントリビューションを促進するために不可欠だということが、多くのプログラミングチームにより確認されています。

インナーソースの開発プラクティスは、本質的に OSS の開発プラクティスと同じなので、社内で開発されたプロジェクトを OSS 化するのは非常に簡単です。
技術的にチームがすべきことは、コードをパブリックリポジトリに移動して、社内メンバーからのバグレポートやコードコントリビューションに対して行ってきたことを、社外で行うだけです。

ただし、いくつか法的な壁に直面する可能性があります。
プログラマーが外部のコードをプロジェクトに組み込んだ場合を例に挙げます。
このとき法務部門は、すべてのライセンスを調査して、彼らがコードをオープン化する権利を持つか、それらのコードのライセンスと組み込んだコードのライセンスとの間に互換性があるかを確認しなければなりません。
また、ブランドレビューが必要な場合もあります。
PayPal では、法務チームが OSS 専門家と相談し、必要な手順をウェブベースで行えるようにしました。

現代のプログラマーは、変化が成長につながることを学びます。
新しい技術やツールはさておき、文化を変えることで、機敏に行動し、最新のスキルを身につけ続けることができるのです。
インナーソースは、これらすべての成果への第一歩です。

[^stol2014]: Stol, KJ, P. Avgeriou et al. [“Key Factors for Adopting Inner Source.”](http://www.brian-fitzgerald.com/wp-content/uploads/2014/05/TOSEM-2014-stol.pdf) _ACM Transactions on Software Engineering Methodology (TOSEM)_ (2014): Vol 23, No 2.

[^stol2011]: Stol, KJ, AB Muhammad, et al. [“A comparative study of challenges in integrating Open Source Software and Inner Source Software.”](http://www.cs.rug.nl/paris/papers/IST11.pdf) _Information and Software Technology_ 53 (2011): 1319–1336\.

[^documentation]: 訳注: 原文では The Importance of Documentation と書かれています。ここでの documentation とは文書にすることだけでなく、チャットやチケットのコメントも含むため、明文化と表現しました。

[^test-pyramid]: 訳注: この文脈で手動テストは含まれないことに注意してください。Mike Cohn は [Succeeding with Agile](https://www.mountaingoatsoftware.com/books/succeeding-with-agile-software-development-using-scrum) または [The Forgotten Layer of the Test Automation Pyramid](https://www.mountaingoatsoftware.com/blog/the-forgotten-layer-of-the-test-automation-pyramid) の中で Test Automation Pyramid と記しています。"自動テストピラミッド" の方が正確な訳ですが、日本では "テストピラミッド" という呼称が普及しています。

[^mailing-list]: 訳注: 2022 年現在では Gitter や Slack といったチャットツールがメーリングリストに代わって利用される場合も増えているでしょう。

[^proprietary-software]: 訳注: プロプライエタリ(proprietary)とは、"独占的"、"専売" を意味する形容詞です。プロプライエタリソフトウェアとは、1社が独占的に提供し、ソースコードやその他の中間成果物が非公開であるソフトウェアを主に意味します。本文のように、OSS の対義語として使われる場合がほとんどです。

[^not-only-SaaS]: 訳注: SaaS に限らず、デスクトップアプリや組込みソフトウェアでも同様の選択をすることがあるでしょう。

[^closed-core]: 訳注: オープン・クローズ戦略の方が日本の企業人にとって馴染みがあるのではないでしょうか。ただし、オープン・クローズ戦略はソフトウェアの開発や提供の方法ではなく知財マネジメントの文脈で語られることに注意が必要です。興味のある読者は[経済産業省発行の2013年版ものづくり白書](https://www.meti.go.jp/report/whitepaper/mono/2013)第3節 その3を参照するとよいでしょう。

[^trusted-committer]: 訳注: OSS において、コミッターは開発方針やコード変更の最終判断を担う中心的存在です。インナーソースでは、ある組織内のソフトウェアに対して一定以上の貢献をしたと信頼された人は、その組織内の所属部署に関わらずトラステッドコミッターと呼ばれます。お墨付きコミッターと言ってもよいかもしれません。

## 著者紹介

**Andy Oram** は、 O'Reilly Media の編集者です。
1992 年から同社に勤務しており、現在はオープンソース技術とソフトウェアエンジニアリングを専門としています。
O'Reilly での彼の著作には、米国で初めて出版された Linux の書籍や、2001 年に出版された _Peer-to-Peer_ 、2007年のベストセラー _Beautiful Code_ などがあります。
