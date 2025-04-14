# Source Tree

File-Clone/New

URL-github哪個倉庫

PATH-檔案位置

取檔名

用vscode做檔案操作

Stage	加入到暫存區（準備 Commit）

Unstage	從暫存區移出（回到未暫存狀態）

Discard	丟棄本地變更，還原為最後一次提交的狀態

Resolve Conflicts	解決合併衝突

External Diff	用外部比較工具（如 Beyond Compare）開啟對比

Add	加入 Git 追蹤

Remove	將檔案從 Git 移除（還留在電腦上）

Ignore	加入 .gitignore，以後不追蹤這個檔案

Reset current branch to this commit	將目前分支回朔到此 Commit（有三種模式）
└─ Mixed	重設提交紀錄，但保留變更（會回到未暫存狀態）
└─ Soft	重設提交紀錄，變更都保留在暫存區
└─ Hard	重設提交紀錄，刪除所有變更（慎用）

Revert commit	建立一個「反向的 commit」來取消這筆變更

Create Branch	從這個 commit 建立一個新的分支

Merge	將這個 commit 合併到目前分支

Tag	為這個 commit 建立一個標籤（tag）

Checkout this commit	切換到這個 commit（會進入 detached HEAD 狀態）

Cherry Pick	把這筆 commit 的變更套用到目前分支

Checkout	切換到這個分支

Merge	把這個分支的變更合併到當前分支

Delete	刪除本地分支

Push	推送這個分支到遠端（如 GitHub）

Rename	重新命名分支

Track Remote Branch	建立追蹤此遠端分支的本地分支

Checkout	建立一個本地分支並切換過去

Pull	從遠端拉下更新

Push	將分支推送到遠端

Delete Remote Branch	刪除遠端分支（謹慎操作）
