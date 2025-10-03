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
*小谷API26にしたけど21でも問題ない
*プロジェクト名は名前は自分が分かるものなら何でもいいよ

# Bash connect GithubとAndroid Studioを同期

mkdir ~/github
cd ~/github
cp -r "/c/Users/<PCのユーザー名>/AndroidStudioProjects/<プロジェクト名>/"* .
# Git 初期化
git init

# GitHub リポジトリを origin に設定
git remote add origin https://<USERNAME>(Githubのユーザ名)@github.com/<USERNAME>/<REPO>.git

# URL を確認
git remote -v

# ファイル追加
git add .

# commit 作成
git commit -m "Initial commit"

# ブランチ名確認・変更
git branch -M main

# GitHub に push（PAT 使用）
git push -u origin main


# Android Stdio コードファイルの変更後、Bashの方でやること
git add .
git commit -m "変更内容"
git push

