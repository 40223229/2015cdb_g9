# Gitbook 電子書建立與協同設定
使用說明: http://help.gitbook.com/github/index.html

操作步驟:

    在 Github 中建立一個帶有 README.md 檔案的公開倉儲
    在 Gitbook 建立帳號, 進入後建立一本電子書
    電子書建立後, 選擇"Link to Github"
    輸入同步 Github 倉儲連結, 系統傳回設定已經存檔之訊息, 此設定會將 Github 倉儲內的 README.md 檔案取回 Gitbook 對應電子書中
    此時 Gitbook 電子書與 Github 倉儲資料, 已經雙向同步, 分別在兩端編輯推送存檔的資料內容, 都會自動同步到另一端
    假如希望每次在電子書資料更新時, Gitbook 會自動建立電子書, 則按下"Add a deployment webhook"

操作影片:

Q: 是否可以將 markdown 資料以外的內容放入 gitbook 電子書資料中?

A: 可以, gitbook 利用 SUMMARY.md 與 README.md 來安排電子書的內容, 其中 README.md 為內定的 Introduction, 而 SUMMARY.md 則為目錄架構, 定義各章節標題與對應儲存的檔案名稱.

使用者可以在 gitbook 對應的 github 倉儲中, 設法利用 git 放入其他專案執行過程中所需要的其他資料.

Q: 為何在 gitbook 中儲存以中文命名的檔案, 最前頭需要加上底線符號?

A: 因為目前的 gitbook 系統無法對應以中文開頭命名的檔案, 因此必須在中文名稱前加上 ASCII 可以辨識的任何符號, 在此選擇加入底線符號.
