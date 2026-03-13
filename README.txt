配置するファイル
- reservation.html
- slot_admin.html
- available_slots.json

GitHub Pagesに同じフォルダ階層で置いてください。

患者さん用ページ:
- reservation.html
このページは available_slots.json を自動読込します。

先生用管理ページ:
- slot_admin.html
このページから available_slots.json を GitHub API 経由で更新できます。

必要なもの
- GitHub Fine-grained Personal Access Token
- 権限: Contents = Read and write
- トークンはHTML内に保存しないでください

初回手順
1. 3ファイルをGitHubリポジトリへアップロード
2. GitHub Pagesを有効化
3. slot_admin.html を開く
4. GitHubユーザー名 / リポジトリ名 / ブランチ名 / ファイルパス を入力
5. トークンを入力
6. 枠を追加して「GitHubへ保存する」
7. reservation.html を開くと最新の available_slots.json が自動反映されます

注意
- この構成では予約枠の表示は自動更新されます
- ただし患者予約後にその枠を自動で消す仕組みまでは入っていません
- 二重予約を防ぐには別途サーバー処理やGoogle Calendar/Firebase等の連携が必要です
