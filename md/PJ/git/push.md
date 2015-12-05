# 開発中にやること(リモートブランチへの反映)

開発の記録をリモートリポジトリに反映させましょう。  
自分の作成したブランチに対して変更を反映させるため、他の人に影響を与えることはありません。  
少なくとも一日の最後にはこの作業を実施しましょう。  
なお、ローカルリポジトリに登録していない変更はリモートリポジトリには反映されません。

## イメージ図

![push](../img/push.png)

## 作業の流れ

① SourceTreeを起動します。  
② developブランチのソースコードから、最新のソースコードを取り込みます。  
  
![fetch](../img/sourcetree_fetch.png)

③ developブランチの末尾のコミットを指定しOKボタンを押します。  

<img src="../img/sourcetree_marge.png" width="600px">
※**自分が作成したfeatureブランチの状態になっていることを確認**し、マージボタンを押下する。  
  
④ developブランチの末尾のコミットを指定しOKボタンを押します。  

<img src="../img/sourcetree_pull2.png" width="600px">

これを実施することで、developブランチとfeatureブランチの差分を吸収し、  
developブランチへマージ後でもアプリケーションが正常に動作することを確認することが出来ます。  

マージ作業にて競合が発生した場合は、以下サイトを参照して解決してください。　　
http://naichilab.blogspot.jp/2014/01/git-4sourcetreegit.html
  
**⑤ ローカルにてテストを実行して、ソースコードに問題が発生していないことを確認してください。**  
⑥ プッシュボタンを押下してください。  
⑦ **featureブランチにのみ**チェックをいれてください。  
⑧ OKボタンを押してください。これが、イメージ図の**push**です。  

![push](../img/sourcetree_push.png)

## 完了状態

リモートリポジトリに対してローカルの変更を反映させることが出来ました。  
gitBucket（ブラウザ）にて変更を確認してください。  
ブランチは画面の以下箇所にて切り替えることが出来ます。

<img src="../img/gitBucket_end.png" width="700px">