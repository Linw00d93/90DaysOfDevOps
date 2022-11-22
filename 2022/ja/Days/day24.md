---
title: '#90DaysOfDevOps - ネットワーク・オートメーション - 24日目'
published: false
description: 90DaysOfDevOps - ネットワーク・オートメーション
tags: "devops, 90daysofdevops, learning"
cover_image: null
canonical_url: null
id: 1048805
---
## ネットワーク・オートメーション

### ネットワーク・オートメーションの基本

ネットワーク・オートメーションの主なドライバー:

- アジリティの実現
- コスト削減
- エラーの排除
- コンプライアンスの確保
- 集中管理

自動化の導入プロセスは、各ビジネスに特有のものです。よりアジャイルな環境を維持・創造するためには、組織に最適なアプローチを特定し、採用することが重要です。(私たちは、DevOpsの全体像、文化の変化、そしてこれがもたらす自動化されたプロセスに関して、冒頭で同じようなことを述べました)

これを分解すると、自動化しようとしているタスクやプロセスが、ステップバイステップの体系的なアプローチに従いながら、どのようにエンドユーザー・エクスペリエンスやビジネス価値を達成・向上させようとしているのかを特定する必要があるのです。

「もし、あなたがどこに行くのか分からなければ、どんな道でもそこに連れて行ってくれるでしょう。

最終的な目標を知り、その目標達成に向けて一歩一歩作業を進めるためのフレームワークや設計構造を持ち、ビジネスの成果に基づいて様々な段階での自動化の成功を測定します。

既存のアプリケーションをモデル化したコンセプトを構築する自動化に関するコンセプトをバブルの中で設計する必要はない。なぜなら、それはアプリケーション、サービス、インフラストラクチャに適用する必要があるからです。

### ネットワーク自動化の考え方

タスクを特定し、ネットワークの変更要求に関するディスカバリーを行い、最も一般的な問題やソリューションを自動化するための問題を把握する必要があります。

- 現在、手動で対応しているすべての変更要求とワークフローのリストを作成します。
- 最も一般的で、時間がかかり、エラーを起こしやすい作業を決定します。
- ビジネス主導のアプローチで、リクエストに優先順位をつけます。
- これは、自動化プロセスを構築するためのフレームワークであり、何が自動化されなければならず、何が自動化されてはならないか、ということです。

そして、タスクを分割し、異なるネットワーク機能がどのように機能し、互いに影響し合っているかを分析する必要があります。

- インフラ/ネットワークチームは、アプリケーションを展開するために複数のレイヤーで変更チケットを受け取ります。
- ネットワークサービスに基づいて、それらを異なる領域に分割し、それらがどのように相互作用するかを理解します。
    - アプリケーションの最適化
    - ADC (アプリケーションデリバリーコントローラー)
    - ファイアウォール
    - DDI (DNS、DHCP、IPAMなど)
    - ルーティング
    - その他
- ビジネスや文化の違いに対応し、チーム間のコラボレーションを実現するために、さまざまな依存関係を特定します。

再利用可能なポリシー、再利用可能なサービスタスク、プロセス、インプット/アウトプットを定義し、簡素化する。

- 様々なサービス、プロセス、インプット/アウトプットのオファリングを定義する。
- 導入プロセスを簡素化することで、新規および既存のワークロードの市場投入までの時間を短縮する。
- 標準的なプロセスがあれば、マルチスレッドなアプローチとデリバリーのために、個々のリクエストに順次対応させることができる。

ポリシーとビジネス特有のアクティビティを組み合わせる。このポリシーを実行することで、ビジネスにどのような効果があるのでしょうか？時間の節約？お金の節約になりますか？より良いビジネス成果をもたらすか？

- サービスタスクが相互運用可能であることを確認する。
- ビジネスサービスを作成するために、インクリメンタルサービスタスクを関連付けます。
- 必要に応じて、サービスタスクの関連付けや再関連付けを柔軟に行えるようにします。
- セルフサービス機能を導入し、運用効率を向上させます。
- 複数のテクノロジー・スキルセットが、監視とコンプライアンスに貢献し続けることができるようにします。

可用性とサービスを維持しながら、ポリシーとプロセスを追加・改善し、**反復**します。

- 既存のタスクを自動化することから小さく始めます
- 自動化プロセスに慣れることで、自動化の恩恵を受けられる他の分野を特定できるようにします。
- 自動化の取り組みを繰り返し、必要な可用性を維持しながら、少しずつ敏捷性を高めていきます。
- 段階的なアプローチをとることで、成功への道が開かれます。

ネットワークサービスのオーケストレーション

- アプリケーションを迅速に提供するためには、デプロイメントプロセスの自動化が必要です。
- アジャイルなサービス環境を構築するには、技術的なスキルセットを超えてさまざまな要素を管理する必要があります。
- 自動化とデプロイの順番をコントロールするために、エンド・ツー・エンドのオーケストレーションの準備をしましょう。

## ネットワーク・オートメーション・ツール 

良いニュースとしては、ネットワークの自動化に使用するツールは、他の自動化の分野や、これまでに取り上げたもの、今後のセッションで取り上げるものと概ね同じであるということです。

オペレーティング・システム - このチャレンジを通して、私はLinux OSで学習のほとんどを行うことに集中しています。その理由はLinuxのセクションで述べましたが、クロスOSプラットフォームとはいえ、今日触れるツールのほとんどすべては、そもそもLinuxベースのアプリケーションまたはツールから始まっています。

統合開発環境（IDE） - ここでも、IDEとしてVisual Studio Codeをお勧めする以外、あまり言うことはありません。

構成管理 - 構成管理のセクションはまだですが、構成の管理と自動化のためにAnsibleがこの分野で人気があることは明らかです。AnsibleはPythonで書かれていますが、Pythonの知識は必要ありません。

- エージェントレス
- SSHのみ必要
- 大規模なサポートコミュニティ
- 豊富なネットワークモジュール
- プッシュ型
- YAMLで設定
- オープンソース

[Ansibleネットワークモジュールへのリンク](https://docs.ansible.com/ansible/2.9/modules/list_of_network_modules.html)

また、構成管理セクションで**Ansible Tower**について触れますが、これはAnsibleのGUIフロントエンドとして見てください。

CI/CD - CI/CDのコンセプトとツールについてはまた後ほど詳しく説明しますが、ネットワークだけでなく、サービスやプラットフォームのプロビジョニング全般に渡るものなので、少なくともここで触れておくことは重要です。

特に、Jenkins はネットワークの自動化のためのツールを提供しており、また、人気のあるツールのようです。

- gitリポジトリを監視して、変更を開始します。

バージョン管理 - これも後ほど詳しく説明します。

- Gitは、あなたのローカルデバイス上でコードのバージョン管理を提供します - クロスプラットフォーム
- GitHub, GitLab, BitBucket などは、リポジトリを定義し、コードをアップロードするオンラインウェブサイトです。

GolangとPythonは接戦で、Pythonがネットワークオートメーションの勝者であるように思います。

- ここで特筆すべきはNornirで、Pythonで書かれた自動化フレームワークです。これはAnsibleの役割を担っているようですが、特にネットワークオートメーションに特化しているようです。[Nornirのドキュメント](https://nornir.readthedocs.io/en/latest/) 

APIの分析 - Postmanは、RESTfulなAPIを分析するための素晴らしいツールです。APIを構築、テスト、修正するのに役立ちます。

- POST >> リソースオブジェクトを作成する。
- GET >> リソースを取得する。
- PUT >> リソースを作成または置き換えます。
- PATCH >> リソースオブジェクトを作成または更新します。
- Delete >> リソースを削除します。

[Postmanダウンロード](https://www.postman.com/downloads/)

### その他特記すべきツール

[Cisco NSO (Network Services Orchestrator)](https://www.cisco.com/c/en/us/products/cloud-systems-management/network-services-orchestrator/index.html)

[NetYCE - Simplify Network Automation](https://netyce.com/)

[ネットワークテスト自動化](https://pubhub.devnetcloud.com/media/genie-feature-browser/docs/#/)

この3日間で、これまでカバーしてきたことをさらに実践し、Pythonとネットワークの自動化に関する作業を行う予定です。

私たちはこれまでネットワークのトピックをすべてカバーすることはできませんでしたが、フォローしながらも、以下に追加するリソースから学び続けることができるように、これを十分に広くしたいと思いました。

## リソース

- [3 Necessary Skills for Network Automation](https://www.youtube.com/watch?v=KhiJ7Fu9kKA&list=WL&index=122&t=89s)
- [Computer Networking full course](https://www.youtube.com/watch?v=IPvYjXCsTg8)
- [Practical Networking](http://www.practicalnetworking.net/)
- [Python Network Automation](https://www.youtube.com/watch?v=xKPzLplPECU&list=WL&index=126)

[25日目](day25.md)でお会いしましょう。