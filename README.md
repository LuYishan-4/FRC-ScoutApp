![](https://github.com/team7632/FRC-ScoutApp/blob/master/assets/images/favicon.png)
# FRC Scouting System - 7632

![Node.js](https://img.shields.io/badge/Node.js-v16%2B-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-4.x-000000?style=for-the-badge&logo=express&logoColor=white)
![NAS](https://img.shields.io/badge/NAS-Hosted-blue?style=for-the-badge&logo=synology&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

---

## 目錄
* [系統概覽](#系統概覽)
* [快速入門](#快速入門)
  * [登入](#登入)
  * [建立與加入房間](#建立與加入房間)
  * [開始觀賽](#開始觀賽)
    * [前置作業](#前置作業)
    * [正式開始](#正式開始)
      * [AUTO階段](#auto階段)
      * [手動階段](#手動階段)
      * [結算數據](#結算數據)
* [PIT區偵查](#pit區偵查)

---

## 系統概覽

歡迎使用FRC Scouting System - 7632！這是一款專為 FIRST Robotics Competition (FRC) 競賽設計的數據採集與管理系統。本手冊將引導你完成從數據同步到現場採樣的所有流程。

---

## 快速入門

### 登入
 
在真正開始觀賽之前，請先使用google帳號進行登入

---

## 建立與加入房間

<img src="https://github.com/team7632/FRC-ScoutApp/blob/master/screenshot/Screenshot_20260216_234657.jpg" width="400">

進入首頁後會看到三個按鈕：
* **Create New Room**
* **Join Server Room**
* **Fetch TBA Schedule**
---
### Create New Room

* 可以讓使用者自行新增房間，自訂隊伍編號及場次。

* 按下**Create New Room**後，請填寫 **ROOM IDENTIFIER**，並按下 **LAUNCH DATA HUB**則該房建新增完成。

* 房主可在 **Join Server Room** 中看到剛剛新增的房間。

* 房主進入該房間後，可按下右上角盾牌圖示，進行場次，隊伍編號，和人員分配。

---
### Join Server Room

* 讓使用者加入已創建的房間，進行觀賽，而觀賽隊伍及場次由房主分發。

<div align="center">
<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_234709.jpg" width="400">
<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_234800.jpg" width="400">
</div>

---

### Fetch TBA Schedule

為了自動化分配任務，系統支援官方場次數據匯入：
* 此頁面中使用者，搜尋並選擇對應的年份與賽事（如2025，New Taipei city)
* 若獲取成功，系統會顯示  **TBA PAYLOAD READ** ，並自動預載所有資格賽的隊伍分配。
* 按下  **LAUNCH DATA HUB**  則創建含該賽事隊伍分配的房間，無須手動入。
* **注意**：若無網路或官方尚未發布日程，可選擇手動輸入隊伍號碼。

<div align="center">
<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_234715.jpg" width="400">
<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_234741.jpg" width="400">
</div>
---

## 開始觀賽

### 前置作業

* 使用者按下 **Join Server Room** 並進入房間後，請等待房主分配，此時畫面為下圖：

<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_234800.jpg" width="400">

* 當使用者畫面顯示隊伍顏色及隊伍編號時，表示房主已完成分配，而畫面上的隊伍編號則是您所要觀賽的隊伍，如下圖：

<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_234750.jpg" width="400">

* 此時您可按下畫面下方的**START SCOUTING** ，系統會彈出視窗向您確認場次，顏色及隊伍編號，若確認無誤按下 **READY** 則 **開始觀賽！**

---
## 正式開始

### AUTO階段

<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_235008.jpg" width="400">

* 進入觀賽畫面，首先會看的是"AUTO階段"請透過畫面上的 "**+**"，"**-**" 紀錄機器在AUTO階段的行為及得分。

* 如果機器有自動階段離開或者自動階段吊掛時可按下 **Leave Lin** 或者 **Auto Hang** ，若機器兩者都有，則兩個按鈕都按下。

AUTO階段還有個功能為AUTO路徑繪製:

**使用說明**
* **繪製路徑**：在場地地圖上依序點擊，系統將自動連線形成路徑。
* **插入指令**：在特定點位切換至 Command 模式，為該路徑點附加動作說明。
* **等待指令 (Wait)**：記錄機器人在該點位的停留時間。
* **路徑回放 (Play)**：點擊右側綠色播放按鈕，可模擬路徑的執行過程。
* **編輯與修正**：
  * **Undo**：撤銷上一步操作。
  * **Clear**：清除當前畫板上的所有路徑數據。

<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_235014.jpg" width="400">
---

### 手動階段

* 手東階段操作與AUTO階段相同透過畫面上的 "+"，"-" 紀錄機器在手動階段的行為及得分。

* 在比最賽最後階段，若您偵查的機器有吊掛，請在"ENDGAME STATUS”區點選機器吊掛的層級，若機器沒有吊掛，則點選"NONE"。

> **重要:** 所有數據填寫完畢後請按下"COMPLETE & CYNC DATA"，進入結算數據填寫。

---

### 結算數據

<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_235030.jpg" width="400">
</div>

* **Shooting Accuracy (射擊準確度)：**
  透過滑動條記錄機器人的命中率，區分從 「Low Precision」 到 「Sniper Accuracy」 的表現評級。
* **Driver Performance (操作手表現)：**
  提供快速標籤進行評價。
* **Scout Notes (觀賽筆記)：**
  提供自由文字欄位，記錄機器人的穩定性、防禦表現或發生的機械故障細節。

填寫完畢後點擊 **FINISH MATCH ANALYSIS** 即可上傳完整分析報告至雲端數據庫。

---

## PIT區偵查

透過按下首頁左上角四個格子，選擇 pit Mode ，即可進入PIT偵查。

### 1. Pit Tracker：進度與隊伍概覽

此介面為巡查任務的總表，協助團隊掌握數據採集進度。
* **進度追蹤**：頂部顯示目前已完成的隊伍數量與總隊伍數（如 0 / 29 COMPLETED）。
* **隊伍列表**：以卡片形式排列所有參賽隊伍（如 Team 78, 88...），並清楚標示該隊伍目前的狀態為 PENDING（待處理）。
* **搜尋功能**：支援透過隊伍號碼快速定位特定機器人位置。

### 2. 機器人檔案照片 (Photo)

這是進入特定隊伍（如 Team 78）後的第一個分頁。
* **影像存檔**：提供大型點擊區域，引導 Scouter 現場拍攝或上傳機器人實體外觀照片。
* **視覺識別**：確保分析數據時能與機器人實際外型對應，方便操作員辨識對手。

### 3. 機器規格細節 (Spec)
此分頁用於記錄機器人的硬體配置與設計限制。
* **底盤類型 (Drivetrain Type)**：內建選單供選擇，例如截圖中的 Swerve (MK4/i)。
* **載具容量 (Max Ball Capacity)**：記錄機器人單次可攜帶的物件最大數量。
* **觀察筆記 (Observation Notes)**：提供自由輸入區域，用於記錄機器人的特殊結構、穩定性或其他技術特點。

### 4. 自動階段路徑分析 (Path)
此分頁整合了戰術繪製功能，用於記錄隊伍在自動階段的移動路徑。
* **多路徑管理**：支援針對同一隊伍建立多套方案（如 Auto 1），並可透過 ADD NEW PATH 增加更多預設路徑。
* **路徑繪製工具欄：**
  * **Point**：設定移動路徑上的關鍵座標點。
  * **Wait**：標註機器人在路徑中需停留等待的時間點。
  * **Command**：在特定位置加入執行動作指令。
* **編輯控制**：提供 undo (復原) 與 clear (清空) 功能，並可點擊綠色播放鍵預覽繪製好的路徑。

> **數據同步**:完成照片、規格與路徑設定後，點擊底部的 UPLOAD PIT DATA 即可將完整檔案上傳至雲端系統。
