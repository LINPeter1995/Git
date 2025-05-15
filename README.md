git init : 建立一個git repository
git status : 查看目前檔案的現況(也就是在commit之後不同的部分，如果在commit之後沒有改過則不會出現)
git add <檔名> : 新增檔案到git中(新增的檔案用git status查看會從紅色變成綠色)
git commit : 類似存檔的概念(會進到編輯器當中，預設為vim，打 :q 或 :q! 可以退出)
git commit -m "<訊息>" : 不會進到編輯器中，可以輸入這次commit的訊息(訊息通常會寫這次commit修改了甚麼東西)
git log : 查看commit了甚麼東西 (如果要結束就在終端打q)
git remote add <自訂名稱> <網址> : 通常會結合github，把這個本地端的檔案連結到網址中
git remote : 列出所有的remote
git push -u <remote 名稱> <branch 名稱> : 把我們現在的 branch 推到 remote，也就是在github中的repo，而-u是代表把預設的remote設成origin，也就是之後我們沒有指定remote時都會推到origin
git clone <網址> : 在電腦中把github上面的檔案下載
git log : 查看目前這個檔案的所有紀錄
git reset – <檔案> : 把git add過的檔案unstage回去
git checkout – <檔案> : 把檔案回到上次git commit的狀態
git reset –soft HEAD~1 : 會往前推1個commit，並且會有git log 的紀錄，保留住修改的部分
git checkout -b <branch 名稱> : 建立新branch並且切換過去
git branch : 查看電腦上的branch (如果要結束就在終端打q)
git branch -a : 查看電腦上的所有branch(包含remote)
git branch -d <branch名稱> : 刪除電腦上的branch，但github上如果有的話不會刪掉
git switch <要去的 branch> : 切換branch(須注意所有檔案都要先commit才能switch)
git pull : 把預設的upstream新進度抓下來
git rebase <要rebase 到哪個分支> : 把目前分支的起始點移到最新進度
git rebase –continue : 解決好上面rebase的衝突之後繼續rebase(通常會不只一個衝突發生，所以需要continue好幾次)
git push -f : 強制把現在電腦上的紀錄push到remote (不建議在主分支使用)
