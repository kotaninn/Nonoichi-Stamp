# Nonoichi-Stamp
MainActivity.kt,AndroidManifest.xml

# 毎回の開発前にやること
1. 今のブランチの確認
 git branch
 (ここでfeature/〇〇になっていることを確認
 →もしなってなかったらgit checkout feature/〇〇で変更)

2. リモートの最新の状態を取得
 git fetch origin
*プロキシに阻まれて学校Wi-Fiではできない

4. 同じブランチの最新を反映
 git pull origin feature/step-counter

# 毎回の開発後にやること
1. 変更したすべてのファイルをステージング
git add .

2. コミットメッセージは何を変更したかを書く
git commit -m "(例　歩数表示機能を追加)"

3. GitHub の main ブランチに送る
git push origin feature/(担当のリポジトリ，例　ui)

4. GitHub の最新変更をローカルに取り込む
git pull origin main



DLで暇な人へ
https://learngitbranching.js.org/?locale=ja
でGithubに慣れましょう
