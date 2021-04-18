## [Week 1 hw1] 交作業流程

1. 連結 github classroom 上的個人 repo 
2. 進入頁面後，按code按鈕，複製網頁連結
3. 開啟 Termimnal，輸入 `git clone +指定連結`，將資料 clone 下來
4. 完成後，cd 到剛剛下載的作業資料夾中
5. 輸入`git branch week1` 建立一個叫做 week1 的新 branch
6. 輸入`git checkout week1`，切換 branch 到 week1
7. mv 作業檔案，將寫好的作業放到作業資料夾中
8. 輸入`git status`，確認作業檔案狀態顯示為修改，需要加入提交
9. 輸入`git commit -am"說明文字"`，將新版的檔案 add 進版本管理清單並進行 commit
10. 輸入`git push origin week1`，將作業 push 到 github
11. 回到 github 頁面，至 Pull requests 分頁，按下 "Compare & pull request"，將 week1 的內容 merge 到 master 中
12. 確認一下 Files changed 看看是否正確
13. 如果有交了作業發現錯誤要修正，不需要重新 pull request，只需要 commit -am 後再 push 一次，github 上會新增一個 commit，同時可檢查 Files changed 是否正確
14. 複製 PR 連結，到學習系統的課程總覽，按下繳交作業，貼上連結，送出後完成！


