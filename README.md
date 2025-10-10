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

DLで暇な人へ
https://learngitbranching.js.org/?locale=ja
でGithubに慣れましょう

# =========================================
# 1. GitHub リポジトリを origin に設定
# =========================================
# まだ origin が設定されていない場合のみ
git remote add origin https://github.com/<USERNAME>/<REPO>.git

# ※古いoriginがある場合は削除して再設定
# git remote remove origin
# git remote add origin https://github.com/<USERNAME>/<REPO>.git


# =========================================
# 2. URL を確認
# =========================================
git remote -v


# =========================================
# 3. ファイルを追加
# =========================================
git add .


# =========================================
# 4. コミットを作成
# =========================================
git commit -m "Initial commit"


# =========================================
# 5. ブランチ名を main に変更（必要なら）
# =========================================
git branch -M main


# =========================================
# 6. GitHub へ Push（PATを使用）
# =========================================
git push -u origin main

1. トークンを発行する

    GitHub右上のアイコン → Settings（設定）

    左メニューから Developer settings

    Personal access tokens → Tokens (classic) を選択
    （または「Fine-grained tokens」でもOK）

    「Generate new token」→「classic」選択

    チェックを入れる範囲
    repo
    workflow
    read:org

    「Generate token」をクリックして、出てきた トークン文字列をコピー

2. Git Bashで push するときの入力
    Username for 'https://github.com': <あなたのGitHubユーザ名>
    Password for 'https://github.com': <ここにトークンを貼り付け>

Android Studio側でコード変更後の流れ 

# 変更を確認（オプション）
git status

# 変更ファイルを追加
git add .

# コミット作成（メッセージは変更内容を記述）
git commit -m "MainActivity に NFC タッチ機能追加"

# GitHubへアップロード
git push
