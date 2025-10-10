# Nonoichi-Stamp
MainActivity.kt,AndroidManifest.xml

# Set up
1.Git Bashをインストールする(以下のサイトを参考に)
https://qiita.com/suke_masa/items/404f06309bb32ca6c9c5

2.Android Stdioをインストールする(以下のサイトを参考に)
https://codeforfun.jp/how-to-install-android-studio-windows-and-mac/

3.Android Stdioで新規プロジェクト作成する(以下のサイトを参考に)
https://courses.codeforfun.jp/courses/1597880/lectures/47723566
*C:\Users\<PCのユーザー名>\AndroidStudioProjects\<プロジェクト名>
*小谷はAPI26にしたけど21でも問題ない
*プロジェクト名は名前は自分が分かるものなら何でもいいよ

4.Github Bashでこのコードを打つ
git clone https://github.com/<USERNAME>/Nonoichi-Stamp.git

# 毎回の開発前にやること
1. 今のブランチの確認
 git branch
 (ここでfeature/〇〇になっていることを確認
 →もしなってなかったらgit checkout feature/〇〇で変更)

2. リモートの最新の状態を取得
 git fetch origin

3. 同じブランチの最新を反映
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
