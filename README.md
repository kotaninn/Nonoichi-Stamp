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

毎回の開発後にやること
git add .             　　　　　　 # 変更したすべてのファイルをステージング
git commit -m "歩数表示機能を追加"  # コミットメッセージは何を変更したかを書く
git push origin main  　　　　　　 # GitHub の main ブランチに送る
git pull origin main  　　　　　　 # GitHub の最新変更をローカルに取り込む



DLで暇な人へ
https://learngitbranching.js.org/?locale=ja
でGithubに慣れましょう
