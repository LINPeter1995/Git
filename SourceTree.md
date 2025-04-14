# Source Tree

File-Clone/New

URL-github哪個倉庫

PATH-檔案位置

取檔名

用vscode做檔案操作

-------------------------------------------------------------------------------

Stage（加入暫存區）	

就像是先把你寫好的檔案「暫時放進打包區」，準備等一下打包（Commit）送出去。你沒 Stage 的檔案，不會被 Commit 到版本紀錄裡。

Unstage（移出暫存區）	

把剛剛放進去準備打包的東西先拿出來，不想這次提交它了。比如你改了三個檔案，但這次只想提交兩個，就可以把不想交的 Unstage 掉。

Discard（丟掉變更）	

把你改過的檔案全部還原成上次 Commit 的樣子，沒 Commit 前的小改動會直接消失。很危險，要小心用，記得先備份重要修改！

Resolve Conflicts（解衝突）	

如果你 Pull 或 Merge 之後，Git 不知道要選哪一版（你改了、別人也改了），就會出現衝突。這個功能是讓你打開工具，手動決定要保留誰的版本。

External Diff（用外部工具比較差異）	

如果你有安裝像是 Beyond Compare、Meld 這種好用的比對工具，可以用這個功能打開看「改了哪些地方」。看得更清楚、更舒服。

Add（加入 Git 追蹤）	

有些檔案是新的，還沒被 Git 管理過，這個功能會讓 Git 開始追蹤它們的變化。也就是「開始注意這個檔案的歷史紀錄」。等同於 git add。

Remove（從 Git 移除）	

從版本控制中移除這個檔案，但本地硬碟上還會留著，不是刪掉檔案，是告訴 Git「以後不要再管這個檔案」。等同於 git rm --cached。

Ignore（加進 .gitignore）	

這檔案以後都不要被 Git 管（例如 log 檔、設定檔等），就會自動加入到 .gitignore 檔案中。這樣 Git 不會再一直提示你說「這個檔案未被追蹤」。

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
