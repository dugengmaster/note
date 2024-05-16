# [Git and GitHub for Beginners - Crash Course](https://www.youtube.com/watch?v=RGOj5yH7evk) 筆記
## Git 是什麼?
免費且開源的版本控制系統。
## 那什麼是版本控制?
- 版本控制是一種管理文件、電腦程式、大型網站以及其他資訊集合變更的系統。在程式開發中，代表的是一種追蹤程式碼變化的方法。  
- 每當開發者提交更新時，這些變更都會被記錄在 Git 儲存庫（repository）裡，這不僅允許開發者查看隨時間的變化，還能幫助他們檢視特定變更的內容，理解當時做出變更的原因，並且在發現錯誤或需要恢復到先前的狀態時，能夠追蹤到具體的提交點。  
- 此外，版本控制系統支援多人協作，使得多個開發者可以在同一個項目上工作，而不會互相干擾。系統會幫助解決版本之間的衝突，並保證項目的整體一致性。
## 影片中需要學習的術語
- Directory -> 資料夾
- Terminal or Command Line -> 文字命令介面
- CLI -> 命令列介面
- cd -> 變更目錄
- Code Editor -> 用於編寫代碼的文字處理器
- Repository -> 專案的儲存庫
- Github -> 一個用於在線托管你的倉庫的網站
- VSCode -> Windows 開發的程式碼編輯器 Visual Studio Code
- Commit message -> 提交訊息
## 在 Github 建立遠端儲存庫
1. 先註冊一個在 [Github](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home) 的個人帳號並登入。
2. 登入後的頁面叫做 `儀表板`。
3. 點擊畫面左側 <span style="background-color:#09b43a; color:#000; border-radius:3px; padding:1px;">New</span> 或是畫面右側<span style="border-radius:3px; border: 1px solid #999; padding:1px;"> <span style="display: inline-block; justify-content: center; align-items: center; width: 10px; height: 10px; margin-top: 20px">+</span> ▼</span>  號的下拉式選單並選擇 New repository 建立新的儲存庫。 
![圖片](images/hub.png)
### 建立測試用 repo ( Repository的簡寫 )
1. 在 Repository name* 用來輸入repo的名稱。影片範例輸入 demo-repo。
2. 在 Description (optional) 用來描述repo大致的用途。影片範例輸入 Demo for Github Intro video。
3. 最後點擊 <span style="background-color:#09b43a; color:#000; border-radius:3px; padding:1px;">Create repository</span> 。
![圖片](images/hub2.png)
### 建立一個名為 `README.md` 的 Markdown 檔案
Markdown 是一種簡單的[語法](https://hackmd.io/@eMP9zQQ0Qt6I8Uqp2Vqy6w/SyiOheL5N/%2FBVqowKshRH246Q7UDyodFA?type=book)，用來格式化此類檔案中的文字。
`README.md`是每個專案最基本的檔案，其中包含描述該專案的用途文字以及任何相關資訊。
1. 點擊 creating a new file。
2. 在 <span style="border: 1px solid #ccc; padding: 5px; display: inline-block;">`Name your file...`</span> 框框中輸入 README.md。
3. 輸入以下內容：

    ```markdown
    # Demo

    Some description
    ```
4. 點擊畫面右上角 <span style="background-color:#09b43a; color:#000; border-radius:3px; padding:1px;">Commit changes</span> 後會跳出新的對話視窗，`Commit message` 欄位可以輸入你想要描述的訊息，輸入完成後再點擊對話視窗內的 <span style="background-color:#09b43a; color:#000; border-radius:3px; padding:1px;">Commit changes</span> 。

至此，你已經建立了你在 GitHub 上的第一個檔案。
### 在 Github 上編輯檔案
1. 當你在GitHub儲存庫中建立並保存 `README.md` 檔案後，你會看到這個檔案名稱變成一個可點擊的連結。點擊這個連結，會跳轉到該檔案的詳細檢視頁面。在這個頁面上，你可以查看、編輯檔案的內容，並查看歷史版本等。
2. 點擊右側 <svg aria-hidden="true" focusable="false" role="img" class="octicon octicon-pencil" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" style="display:inline-block;user-select:none;vertical-align:text-bottom;overflow:visible"><path d="M11.013 1.427a1.75 1.75 0 0 1 2.474 0l1.086 1.086a1.75 1.75 0 0 1 0 2.474l-8.61 8.61c-.21.21-.47.364-.756.445l-3.251.93a.75.75 0 0 1-.927-.928l.929-3.25c.081-.286.235-.547.445-.758l8.61-8.61Zm.176 4.823L9.75 4.81l-6.286 6.287a.253.253 0 0 0-.064.108l-.558 1.953 1.953-.558a.253.253 0 0 0 .108-.064Zm1.238-3.763a.25.25 0 0 0-.354 0L10.811 3.75l1.439 1.44 1.263-1.263a.25.25 0 0 0 0-.354Z"></path></svg> 的圖標，進入編輯模式。
![圖片](images/hub3.png)
3. 在第三行 `Some description` 的後面增加 `!`：

    ```markdown
    # Demo

    Some description!
    ```
4. 點擊畫面右上角 <span style="background-color:#09b43a; color:#000; border-radius:3px; padding:1px;">Commit changes</span> ，在新的對話視窗輸入你想要描述的訊息再點擊對話視窗內的 <span style="background-color:#09b43a; color:#000; border-radius:3px; padding:1px;">Commit changes</span> 。

這樣就能離開編輯模式，並儲存你剛才的更動。  
### 檢視修改的歷史紀錄
如果你想檢視剛剛儲存的更動，你可以按照以下步驟操作：
1. 在 GitHub 儲存庫的主頁面，找到並點擊 `README.md` 檔案名稱，這將帶你進入該檔案的詳細檢視頁面。
2. 在該頁面的右上角，找到並點擊 <svg aria-hidden="true" focusable="false" role="img" class="octicon octicon-history" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" style="display:inline-block;user-select:none;vertical-align:text-bottom;overflow:visible"><path d="m.427 1.927 1.215 1.215a8.002 8.002 0 1 1-1.6 5.685.75.75 0 1 1 1.493-.154 6.5 6.5 0 1 0 1.18-4.458l1.358 1.358A.25.25 0 0 1 3.896 6H.25A.25.25 0 0 1 0 5.75V2.104a.25.25 0 0 1 .427-.177ZM7.75 4a.75.75 0 0 1 .75.75v2.992l2.028.812a.75.75 0 0 1-.557 1.392l-2.5-1A.751.751 0 0 1 7 8.25v-3.5A.75.75 0 0 1 7.75 4Z"></path></svg> History 按鈕。
![圖片](images/hub4.png)
3. 進入該頁面後，你將看到該檔案的所有歷史紀錄列表，包括每次更動的提交訊息、提交人以及提交日期和時間。
![圖片](images/hub5.png)
4. 在歷史紀錄列表中，點擊你想要查看的某次提交訊息（例如 `Update README.md`），這將帶你進入該次提交的詳細更動紀錄頁面。這個提交訊息是一個超連結，點擊它可以查看該次提交的具體更動內容。
![圖片](images/hub6.png)
5. 在詳細更動紀錄頁面中，你會看到檔案的變動內容。
>- 未被上色的區塊代表這些行未被更動。
>- <span style="background-color: #631c03 ;color: white;">帶有 <span style="display: inline-block; width: 20px; text-align: center;">-</span> 號的紅色區塊代表這些行已經被刪除。</span>
>- <span style="background-color: #0e4429 ;color: white;">帶有 <span style="display: inline-block; width: 20px; text-align: center;">+</span> 號的綠色區塊代表這些行已經新增於此檔案中。</span>
## 關於 Git 的術語
![pic](images/vW8p89H_d.png)
- `Working Directory` -> 工作目錄，這是你的本地檔案系統中的工作區域，在這裡你可以自由編輯和修改檔案。
- `Staging Area` -> 暫存區，這是一個處於工作目錄和本地儲存庫之間的中間層，用來準備下一次提交的文件變更。
- `Local Repository` -> 本地儲存庫，這是儲存在你本地機器上的倉庫，包含了所有提交的記錄。
- `Remote Repository` -> 遠端儲存庫，這是儲存在遠端伺服器上的倉庫，可以與其他人的儲存庫進行同步。
## Git 的命令
- `init` -> 在目前的資料夾內創建一個新的本地儲存庫。這是開始使用 Git 追蹤資料夾中檔案的第一步。
- `clone` -> 從遠端伺服器（例如 GitHub）上複製一個 Git 儲存庫到本地儲存庫。這個命令會將遠端儲存庫的所有檔案、分支和版本記錄都複製到本地。
- `status` -> 顯示當前工作目錄和暫存區的狀態。這包括顯示哪些文件被修改過但還沒被暫存，哪些文件已經被暫存但還未提交，以及哪些文件目前由 Git 追蹤。
- `add` -> 將新檔案或已修改的檔案添加到暫存區，準備進行提交。這一步是告訴 Git 你想要包含哪些改變在下一次提交中。
- `commit` -> 將暫存區域的變更記錄提交到儲存庫歷史中。每一次提交都會有一個關聯的提交信息，說明這次變更的內容。
- `push` -> 將本地的分支變更推送到遠端儲存庫。這樣其他人就可以看到你所做的修改。
- `pull` -> 從遠端儲存庫下載最新的變更並合併到本地儲存庫。這用於保持本地和遠端儲存庫的同步。
- `ignore` -> 指定 Git 應忽略並不追蹤的文件或目錄。這通常是通過在 Git 倉庫的根目錄下創建一個名為 `.gitignore` 的文件來實現的。在 `.gitignore` 文件中，你可以列出所有你不希望 Git 添加到版本控制中的文件和目錄的模式。
### 檔案追蹤狀態
檔案在工作目錄下有兩種狀態：**已追蹤**和**未追蹤**。  
**已追蹤檔案**分為
1. 未修改：這些檔案自上次提交後沒有變更，不會在 `git status` 中顯示。
2. 未暫存的修改：（Unstaged changes）：這些檔案已經被修改但尚未添加到暫存區。在 `git status` 的輸出中會以<span style="color: #d74a32;">紅色顯示</span>，提醒你需要進行暫存。
3. 已暫存的修改（Staged changes）：這些檔案已經用 `git add` 命令添加到暫存區，準備被提交。在 `git status` 的輸出中會以<span style="color: #09b43a;">綠色顯示</span>。

**未追蹤檔案**則是新添加到工作目錄中尚未被 Git 追蹤的檔案，它們在 `git status` 的輸出中也會以<span style="color: #d74a32;">紅色顯示</span>。你可以選擇`添加到暫存區`或`忽略`。

複製遠端儲存庫到本地儲存庫後，所有檔案預設為**已追蹤**且**未修改**。當你修改檔案後，可將其預存並提交，然後繼續這個循環。
![圖片](images/lifecycle.png)
## 開始操作 Git
如果你是 Mac 或 Linux 作業系統的使用者，你的電腦應該已經安裝了 Git，你可以在 Terminal 輸入 git --version 來檢查安裝的版本。  
如果尚未安裝，強烈建議檢視 [Atlassian](https://www.atlassian.com/git/tutorials/install-git) 的教學，它將引導你完成如何在任意作業系統安裝 Git。
- 影片的作者強烈建議 Mac 使用者安裝 Homebrew 版本。
### 接下來要安裝程式碼編輯器
- 推薦安裝 [Visual Studio Code](https://code.visualstudio.com/)。這是一款 Microsoft 製作的免費程式碼編輯器，被學習編碼的人與專業人士廣泛使用。
### 在 VSCode 開啟一個測試資料夾
![錄製螢幕的GIF](./images/open%20folder.gif)
### 將遠端儲存庫複製到本地資料夾
1. 點擊畫面左上角 `<> Code` 返回到儲存庫頁面。
2. 點擊畫面中間的 <span style="background-color:#09b43a; color:#000; border-radius:3px; padding:1px;"><> Code ▼</span>。
3. 看到中間的網址，點擊它旁邊的 <svg aria-hidden="true" focusable="false" role="img" class="octicon octicon-copy" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" style="display: inline-block; user-select: none; vertical-align: text-bottom; overflow: visible;"><path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path></svg> 這會把你遠端儲存庫的網址複製下來。
4. 點擊 <kbd>Ctrl</kbd> + <kbd>`</kbd> 組合鍵呼叫 VSCode 的 Terminal，輸入以下命令：

    ```terminal
    git clone 剛剛複製的網址
    ```
5. 完成後，你將有一個複本的本地儲存庫，其中包含遠端儲存庫的所有文件和歷史記錄。
6. 進入該資料夾，以開始在本地環境中工作。你可以使用命令 `cd` 儲存庫名稱 來變更目錄到新複製的本地儲存庫。
    ```terminal
    cd demo-repo
    ```
    本地儲存庫內其實有個隱藏的資料夾，在大多數操作系統中，`.git` 作為隱藏資料夾默認是不顯示的。
- 在 macOS 或 Linux 中：
你可以在 Terminal 使用`ls -a`命令來列出包括隱藏文件和資料夾的所有內容。
- 在 Windows 中：你可以在 cmd 使用`dir /a` 命令來列出包括隱藏文件和資料夾的所有內容。這個隱藏的資料夾 `.git` 存儲了該儲存庫的所有版本控制信息，包括提交記錄、分支、標籤等。
### 在本地儲存庫編輯檔案
1. 開啟本地資料庫內的 `README.md` 新增一些內容
    
    ```markdown
    # Demo

    Some description!

    ## Subheader

    Watch tutorial on YouTube
    ```
2. 修改這個檔案之後需要透過提交在 Git 中儲存。首先，在 terminal 使用 `git status` 命令：

    ```terminal
    git status
    ```
    status 命令會顯示所有已更新、建立或刪除但尚未儲存在提交中的檔案。
    ![圖片](images/git1.PNG)
3. 將已修改的檔案添加到暫存區：
    - 添加當前目錄下的所有修改
    ```terminal
    git add .
    ```
    - 添加特定文件
    ```terminal
    git add README.md
    ```
    在這一步後，你可以再次使用 `git status` 來查看哪些檔案已被添加到暫存區，哪些還沒有。

    ![圖片](images/git2.PNG)
4. 一旦所有需要的修改都已添加到暫存區，你可以使用 `git commit` 命令來提交這些修改。提交時加入適當的提交訊息是個好習慣，這有助於未來理解這些修改的目的。
    ```terminal
    git commit -m "Add new content to README"
    ```
    再次使用 git status 命令，可以看到目前沒有待提交的修改，這表明所有的變更都已經提交了，沒有未解決的修改或新增文件。

    ![圖片](images/git3.PNG)

## SSH Keys
為了將本地儲存庫的專案推送到你在 Github 帳號下的遠端儲存庫，必須向 Github 證明你是該帳戶的所有者。因此，你必須以某種方式將本地
## 將本地儲存庫的檔案推送到遠端儲存庫
在完成本地儲存庫的更新後，用 `git push` 指令推送到託管你的專案之遠端儲存庫。

