# 2023ソフトウェア工学
2023/7/5
github演習

***
## gitの機能

- コミット  
  ファイルの作成・変更・削除を記録する。
  
- レポジトリ  
  gitが管理するプロジェクトのフォルダ

  
   - ローカルレポジトリ
     > 個々のプロジェクト実行環境
   - リモートレポジトリ
     > 共有の管理場所
      
- ブランチ  
  作業を枝分かれさせ共同・並列作業を可能にする。
- gitフロー  

***
## gitのコード
- グローバルセッティング  
  > - gitの設定  
   git config –global  
   git config –global user.name yourname  
   git config –global user.email yourname@example.com  

***
## gitコマンド
- 設定・確認系
  > - git init  
  >  gitの初期化・設定開始
  > - git status  
  >  ワークツリーのステータスを表示
  > - git config  
  >  設定周りの確認・変更
  > - git log  
　   ログを表示  
    -- onelineでコミットメッセージの1行のみの一覧表示  
  > - git diff  
　  ファイルの差分を表示

- コミット系
 > - git add  
 >   ステージングエリアに追加
 > - git commit  
 >   コミットの実行

- 修正系
 > - git commit --amend --no-edit  
 >   コミットの修正
 > - git checkout  
 >   削除されたファイルを復旧や過去コミットの復元など（元に戻す変更がstaging area/index内にある場合）
 > - git reset  
 >   コミットのリセット
 > - git revert  
 >  「コミットの変更を打ち消す」コミット
 > - git rm  
 >   ファイルとindex情報の削除

- リモート系
 > - git clone  
 >   レポジトリをコピー
 > - git pull  
 >   リモートレポジトリの同期	
 > - git push  
 >   変更をアップロードする
 > - git request-pull  
 >   プルリクエスト：変更依頼
 > - git remote  
 >   リモートレポジトリの設定

- ブランチ系
 > - git branch  
 >   ブランチの作成
 > - git checkout  
 >   ブランチの切り替え
 > - git merge  
 >   ブランチの統合
 > - git clone  
 >   レポジトリをコピー
 > - git push  
 >   変更をアップロードする
***
## githubフロー
1. 分岐を作成
  > - ブランチを作成することで既定のブランチに影響を与えずに作業するスペースを作成する。またコラボレーターに作業をレビューする機会を与える。
2. 変更を加える
  > - ブランチでリポジトリに必要な変更を加える。その後ブランチにコミットしてプッシュする。 
3. pull request を作成する
  > - 変更に関するフィードバックをコラボレーターに依頼する pull request を作成する。一部のリポジトリでは pull request 
  をマージする前に承認レビューが必要となる。
4. レビューコメントに対応する
  > - レビュー担当者は質問、コメント、提案を残す必要がある。レビュー担当者は pull request 全体や特定の行またはファイルにコメントを追加することが可能。
5. pull request をマージする
  > - pull request が承認されたら pull request をマージする。これによりブランチが自動的にマージされ、変更が既定のブランチに表示される。
6. ブランチを削除する
  > - pull request がマージした後ブランチを削除する。これはブランチでの作業が完了したことを示し、誤って古いブランチを使用することを防ぐ。



