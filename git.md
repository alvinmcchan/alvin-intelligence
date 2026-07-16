https://github.com/alvinmcchan/alvin_project
git push origin HEAD:main

## push
git status
git add .
git commit -m "new PC0110"
git push origin main
or 
git push 

--------------------------------------------------------

## git clone & Setting
git clone https://github.com/alvinmcchan/ac_strategy.git
git clone https://github.com/alvinmcchan/wSTA.git
git push origin main

--------------------------------------------------------

## 新增遠端分支
git push -u origin PC0110

--------------------------------------------------------

## 連結遠端分支
git branch --set-upstream-to=origin/PC0110 PC0110

--------------------------------------------------------

## 確認遠端分支清單
git fetch --all
### check 遠端所有分支
git branch -r
### check 所有分支
git branch -a
### check 現在分支
git branch 
### 知道分支和遠端的追蹤狀態
git branch -vv


--------------------------------------------------------

## 切換分支
git checkout PC0110
git checkout main
## 建立並切換到新分支
git checkout -b new-branch-name

--------------------------------------------------------

## pull
git pull

--------------------------------------------------------

## push
git status
git add .
git commit -m "test remote by 2026.02.12 on PC0110"
git push origin main
or 
git push 

…or create a new repository on the command line
echo "# telegram-bot" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/alvinmcchan/tongsheng.git
git push -u origin main

…or push an existing repository from the command line
git remote add origin https://github.com/alvinmcchan/telegram-bot.git
git branch -M main
git push -u origin main

--------------------------------------------------------


## 建立 Pull Request (推薦做法)
在 GitHub 網站上操作：

進入你的 repository。

點選 Pull requests → New pull request。

選擇 base: main，compare: PC0110。

建立 PR，檢查差異，確認後合併。

這樣能清楚看到兩個分支的差異，並且保留合併紀錄。

## 合併分支 (Merge)
如果你希望把 PC0110 的內容合併到 main：

bash
# 切換到 main 分支
git checkout main

# 合併 PC0110 分支
git merge PC0110

# 推送到遠端
git push origin main


## add Checkpoint



## 在 master 分支合併 PC0110
git checkout origin/master
git merge PC0110
git commit -m "merge master by 2026.02.12 on PC0110"
git push origin master
git checkout origin/PC0110
git checkout PC0110

git checkout origin/main

只顯示衝突檔案

git diff --name-only --diff-filter=U

查看衝突的詳細內容

git diff

刪除檔案

git rm runGit.bat

用 Git 刪除並提交

git rm -r runGitFolder
git commit -m "Remove ai_resource"
git push origin master


