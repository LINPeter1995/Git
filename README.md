# Git

版本控制

Git + Sourcetree

Mac 建議裝 Homebrew

https://git-scm.com/downloads/mac

# 初始化 Git 倉庫
git init

# 克隆遠端倉庫
git clone <儲存庫網址repository-url>

# 查看當前倉庫狀態
git status

# 查看 Git 配置
git config --list

# 添加文件到暫存區
git add <檔案名稱file-name>

# 添加所有變更的檔案到暫存區
git add .

# 提交變更
git commit -m "your commit message"

# 查看提交紀錄
git log

# 檢查遠端倉庫
git remote -v

# 從遠端倉庫拉取更新
git pull <遠端名稱remote> <分支名稱branch>

# 推送到遠端倉庫
git push <遠端名稱remote> <遠端名稱branch>

# 查看所有分支
git branch

# 創建新分支
git branch <分支名稱branch-name>

# 切換分支
git checkout <分支名稱branch-name>

# 創建並切換到新分支
git checkout -b <分支名稱branch-name>

# 刪除本地分支
git branch -d <分支名稱branch-name>

# 查看檔案歷史變更
git log <檔案名稱file-name>

# 撤銷本地修改（回退檔案到最後提交的狀態）
git checkout -- <檔案名稱file-name>

# 回退至指定的提交
git reset --hard <提交雜湊值commit-hash>

# 從遠端倉庫回退到指定分支或提交
git reset --hard origin/<分支名稱branch-name>

# 合併分支
git merge <分支名稱branch-name>

# 查看合併衝突
git diff

# 創建標籤
git tag <標籤名稱tag-name>

# 列出所有標籤
git tag

# 推送標籤到遠端
git push origin <標籤名稱tag-name>

# 回退到指定的提交 (保留工作區變更)
git reset --soft <提交雜湊值commit-hash>

# 回退到指定的提交 (保留工作區的變更，但不保留暫存區的變更)
git reset --mixed <提交雜湊值commit-hash>

# 完全回退到指定的提交 (撤銷所有變更，恢復到指定的提交狀態)
git reset --hard <提交雜湊值commit-hash>

# 回退到遠端分支狀態
git reset --hard origin/<分支名稱branch-name>

# 撤銷某個檔案的所有修改，讓它回到最近一次提交的狀態
git checkout -- <檔案名稱file-name>

# 使用新版 Git，撤銷某個檔案的所有修改
git restore <檔案名稱file-name>

# 刪除未追蹤的檔案
git clean -f

# 刪除未追蹤的檔案和資料夾
git clean -fd
