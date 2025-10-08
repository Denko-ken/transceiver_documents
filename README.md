# transceiver_documents
トランシーバー開発プロジェクトにおけるドキュメント等を管理する

## GitHub 開発フローの手順

以下は、GitHubを使った基本的な開発の流れです。  
タスク（Issue）に対応し、ブランチを作成して作業を行い、Pull Requestを経てmainブランチにマージする手順を示します。

#### ① Issueを作成する
1. GitHubリポジトリの「Issues」タブを開く
2. 「New Issue」ボタンをクリック
3. 以下を入力して作成
   - title（例：SRSの登録）
   - description（目的・背景・要件など）
   - Assignees （担当メンバー）
   - Labels（該当するラベル）

#### ② ブランチ作成
1. フェッチしてリポジトリを最新にする
2. masterからブランチを新規作成<br>ブランチ名は「**issue #1**」の場合「**issue-1**」
3. ブランチをチェックアウト

#### ③ コミット・プッシュ
1. issueの内容を実施
2. 変更内容をコミット<br>コメントの1行目にはissueのタイトルを貼り付ける<br>例：READMEにドキュメント編集の流れを記載する #1
3. プッシュしてリモートに反映 

#### ④ プルリクエスト
1. GitHubでリポジトリを開く
2. Push後に表示される「Compare & pull request」ボタンをクリック<br>または「Pull requests」→「New pull request」
3. 以下を設定：
   - Baseブランチ： main<br>
   - Compareブランチ： 作業ブランチ（例：issue-1）
   - title（issueと同じ内容）
   - description（目的・背景・要件など）
   - Reviewers（レビューして欲しいメンバー）
   - Assignees （担当メンバー）
   - Labels（該当するラベル）

#### ⑤ masterマージ
1. レビューしたメンバーはコメントを付ける
2. 問題が無ければマージを実施
---