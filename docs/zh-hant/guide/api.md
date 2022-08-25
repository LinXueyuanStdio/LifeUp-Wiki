<h1 align="center" padding="100">開放介面與呼叫</h1>

<p align="center">創造無限可能性！</p>





?> 在 v1.90 版本中，`人升`既開放了多種功能介面，歡迎任意外部應用聯動。<br/>亦提供了商品的“連結”效果，使用者可以直接使用商品來呼叫外部應用或者《人升》的介面。<br/>這可以使你的`人升`獲得無限的可能性，但也需要你有一定的學習理解和動手能力。



## 場景示例

| 呼叫方                                    | 場景                                                         | 備註     |
| ----------------------------------------- | ------------------------------------------------------------ | -------- |
|**人升 ->外部應用**<br/>商品的“連結”效果 | **使用商品後：**<br/>1. 使用瀏覽器訪問某個網頁<br/>2. 跳轉微信掃一掃，或指定小程式<br/>3. 自動新增記賬記錄（[如《錢跡》支援記賬介面](http://docs.qianjiapp.com/plugin/auto_tasker.html)）<br/>4. 儲存自動化工具 Tasker 配置（甚至分享到櫥窗），使用後自動將配置匯入 Tasker<br/>5. ... （只要外部應用支援該方法呼叫） | 任意使用者都可呼叫<br/>Tasker 是一款自動化工具，並且它支援將配置匯出成 Uri |
|**人升 ->人升**<br/>商品的“連結”效果     | **使用商品後：**<br/>1. 開啟人升某個頁面<br/>2. 提升 ATM 利率<br/>3. 彈窗讓使用者選擇商品，降低商品價格（降價券）<br/>4. 觸發某個任務完成<br/>5. 彈出自定義的激勵語訊息<br/>6. 創造任務獎勵模板，只需要輸入名稱即可自動建立任務<br/>7. 彈窗詢問使用者的分支選擇，創造情景化的小互動<br/>8. 更多應用內的操作... | 👑僅限會員使用 |
|**外部應用/網頁 ->人升**                 | **配置自動化工具：**<br/>1. 判斷每天第一次開啟手機的時間，完成早起任務，或者直接觸發“晚起”懲罰<br/>2. 每背完 25 個單詞，刷一次特定的 NFC 卡片，自動打卡任務<br/>3. GPS 判斷到達某個新地方，解鎖“新地點”成就<br/>4. 每天連線打工 WIFI 時，觸發解鎖條件進度增長。累計 20 天的時候，解鎖「打工人」成就<br/>5. 每天首次連線家裏 WIFI 時，獎勵自己“到家”金幣<br/>6. 捕獲其他番茄或專注軟體的通知，自動將計時記錄到人升中<br/>7. 捕獲運動類、背單詞類軟體的完成或結束通知，自動發放「力量」、「學識」經驗值<br/>8. 在自己設定的時間段內，每開一次手機，觸發一次懲罰<br/>9. ...<br>**外部應用聯動/自己開發應用：**<br/>1. 若不滿意「人升」的番茄鍾：可以自己開發計時軟體，可以是網頁應用或安卓應用，透過介面與「人升」聯動，以新增計時記錄或新增獎勵<br/>2. 改動一些智力小遊戲（如下文中有個 Wordle 例子），成功完成遊戲時，觸發「人升」傳送獎勵<br/>3. 開發應用與「人升」聯動實現應用鎖功能 | 👑僅限會員使用 |

<br/>換種說法，上述所有場景其實都是「事件」觸發了「操作」。

而`人升`本次更新是提供了「使用商品」這個事件觸發點，然後是提供了各式各樣的「操作」（獎勵、完成任務等等）。

如果你需要

- 點選網頁按鈕
- 刷 NFC 卡片
- 每天起床第一次解鎖螢幕

這種事件，就需要外部應用的介入。



如果是應用內的指標事件，你可以透過搭配成就來實現。

**如果你想實現，力量達到5級後，提升 ATM 利率0.01%。就可以透過功能組合實現：**

> 成就跟蹤力量等級 -> 達到5級後，自動解鎖成就 -> 獲取特殊商品獎勵 -> 使用後提升 ATM 利率。

諸如番茄鍾專注時長之類的場景也能舉一反三。

---

## 使用建議

**如果你不熟悉網路或計算機基礎知識，**你可以直接在櫥窗搜尋、進貨相關的商品；也可以嘗試根據示例或者其他人的商品，編輯引數。

**如果你熟悉相關基礎知識，**可以嘗試閱讀下述的介面文件，自己編輯出所需的效果。並且搭配自動化軟體（如 Tasker）使用，即便不會編輯 Tasker 的配置，只要你能成功安裝 Tasker，也能在櫥窗或者其他社羣匯入其他人分享的自動化配置。

**如果你有程式設計基礎，**可以嘗試開發網頁、安卓應用與人升聯動。這個網頁就是個超簡單的例子。或者編寫自動化工具的配置，分享給大家！

---

## 呼叫外部 APP

如果你想要在「人升」中呼叫外部應用，只需要為商品新增“連結”效果，並**輸入網頁或應用專屬連結**，再使用該商品即可完成呼叫。



**以下是一些示例（你也可以前往「世界」-「櫥窗」-「呼叫」檢視帶有介面呼叫效果的物品）：**

- 瀏覽器開啟百度：https://www.baidu.com
- 微信：[weixin://](weixin://)
- <del>微信掃一掃（可能失效了）：[weixin://scanqrcode](weixin://scanqrcode)</del>
- 支付寶掃一掃：[alipayqr://platformapi/startapp?saId=10000007](alipayqr://platformapi/startapp?saId=10000007)
- 支付寶螞蟻森林：[alipays://platformapi/startapp?appId=60000002](alipays://platformapi/startapp?appId=60000002)
- 支付寶高德地圖：[alipays://platformapi/startapp?appId=2018070960585195](alipays://platformapi/startapp?appId=2018070960585195)
- 支付寶記賬：[alipay://platformapi/startapp?appId=20000168](alipay://platformapi/startapp?appId=20000168)
- QQ：[mqq://](mqq://)
- 網易雲：[orpheuswidget://](orpheuswidget://)
- 網易雲聽歌識曲：[orpheuswidget://recognize](orpheuswidget://recognize)
- 錢跡的自動化記賬介面：[自動化記賬介面 · 錢跡使用者指南 (qianjiapp.com)](http://docs.qianjiapp.com/plugin/auto_tasker.html)
- ...

理論上，只要外部 APP 開放了對應的連結，你就可以透過使用商品的方式進行跳轉。

**你可以透過百度搜索`URL Schemes`的方式搜尋你需要的應用連結。**

**這些連結與「人升」無關，「人升」只提供跳轉功能。**

**因此我們不會也沒人力維護連結列表。<del>但我們後續會考慮支援櫥窗分享此型別商品。</del>（目前已支援櫥窗分享）**



---

## 呼叫人升

如果你：

- 需要在「人升」中呼叫「人升」的介面，也是隻需要為商品新增“連結”效果，並**輸入網頁或應用專屬連結**，再使用該商品即可完成呼叫。
- 透過網頁呼叫，則只需要超鏈接跳轉我們的介面連結即可。
- 透過自己開發的 APP 呼叫，只需要使用 Intent 跳轉對應的介面連結即可。
- 透過自動化工具（如 Tasker）呼叫，在合適的地方填入對應的介面連結即可。



**一些例子：**

當你點選下面這個連結，「人升」會彈出提示“你學會了呼叫！”。

[lifeup://api/toast?text=你學會了呼叫！&type=1&isLong=true](lifeup://api/toast?text=你學會了呼叫！&type=1&isLong=true)

當你點選下面這個連結，「人升」中會獲得一個金幣，並且獲得原因為“學習API呼叫”。

[lifeup://api/reward?type=coin&content=學習API呼叫&number=1](lifeup://api/reward?type=coin&content=學習API呼叫&number=1)

當你把連結複製到商品的“連結”效果中，使用商品也能夠觸發類似的效果。



**一個外部應用聯動的例子：**

[Wordle Clone (lifeupapp.fun)](https://wiki.lifeupapp.fun/zh-hant/example/wordle/index.html)

Wordle 是猜單詞的小遊戲：猜長度為 5 的單詞。橙黃色代表答案的單詞中包含該字母。綠色代表包含且位置正確。

**該版本的 Wordle 支援與「人升」聯動：**

1. 當你猜中了單詞，能夠獲得 10 點金幣。並且有對應的獲得原因。
2. 當你最終也沒猜中單詞，會有安慰獎 1 點金幣。

![](_media/api/wordle.png ':size=30%')

<br/>

**與 Tasker 聯動的例子：**

> Tasker 呼叫的方式是，選擇`操作類別`-`程式`-`快捷方式`。在快捷方式一欄輸入 lifeup:// 開頭的連結即可。

每天 5 點後第一次解鎖螢幕，能觸發完成一個名稱包含“起床”的任務。

**注意：你需要先自己建立這個名字包含“起床”的每日任務。**

如果你已經安裝了 Tasker，[點選這裏可以匯入已經配置好的任務。](taskerproject://H4sIAAAAAAAAAKVWTW/TQBA9p78iskRPxV7biZNQxyiFHCpFCLVVLxzQKt6kWxzHsrdBvRWEVFS1KkgIIW6IigKqWi6IEvFv2qThxF9g1rv5atyKlEs8nje7fjtv3ir2Co6ekPA+ZjgdhUVFSbstWlR0Jc1aRcVSkaojxZlJ2Q/DZo16JC4KIDYNJd0iRcXgaMquupgRR7cslLFMlMnqRt7WRJLDZBQ2MlnTMG2NDOCah+uRAytEwFPUdUzD1uDB3xrURY4OBXHAM36DON2T/c7Bl4ujo/PTre7Rh97hx99vnv35tds7/NTZf9053u2+fHW2tdv7/qPT3jnb2rM1voqvLreIz+KzVJs+Gj0JHKXpAlWEEByAh7xeixfE4TID1v2letJSKztcmbLvNX2XMtr0KzQSn6Q1UT6Cif0kEVPCKdtbi5xbPnnq4k1b4y8y3wwcHZoDD5kIAbO1sF9ha4OdBQltjIU4UnwQLq0mtU2U2ZxG5qoXOCzcIJDzgknhdTNv5tE/CG9eEr6QKHz24vnP3vHB+Wm7++6k+/bbxfsXMAgADHVeoQ0ylFn0orbmgEDwK94aDjCC3/iNxRiTGIsx1hD94nsltGudVFm/Xevoym4ZOSOHCmPd8jFseN5ud/a2e9tfOzufxcQCeyzpB9SNwAZzvCFxzJOMB3p+jneFiWTMiRPhMXd0TIhBoOfHqQCJjJWxcnrBmsKfIAY3n9QkCCn3B1CCgCdK1cEM4yqTPciNeiKbKYx6YpmFojqsD2d+MOiAirJF6VEo40bDXlFBijaBGddg5jhma4JrAm09gbaZQ6O0I+LUsBfBeEcys7Dhu9It8Vmk/VahKk7Ctwdm9glTXerXPRpV11Tsu2GTuiqL7191qVwpr5YerDxeLS0tlhYq5WVn1mPz0ApYUQpDvCmuZ222zuZhQqbc62YUbrPNgDiPKuu4hVUP+3VV8JmegNhJ3k28O/JaEv2bGAp9MBQerZGN4I6m4YCCEo3AI4zc5QYpimt9MC4j0oJXgcikFwpJXkAoa6IrvYAsM1/IXfZC4f+8kLuBFxK7oyebZQpDjGGZa7CsxMwEzJKYPmGyvhLiKf5nODN/AQAzsyt1CAAA)



![](_media/api/tasker_01.png ':size=30%')

![](_media/api/tasker_02.png ':size=30%')

<br/>

** MacroDroid 的呼叫方式：**

> MacroDroid 也是一款自動化工具，它可以免費下載，UI也更加易用。

1. 增加宏，然後設定你所需要的條件（或者稍後設定）
2. 新增`動作`
3. 選擇`應用程式`
4. 選擇`開啟網站`
5. 在`輸入網址`一欄輸入 `lifeup://` 開頭的 URL 地址
6. 【取消勾選】下面的所有可選項，比如不要勾選`URL引數編碼`...
7. 儲存即可，可以點選該動作，然後選擇`測試`動作進行驗證

<br/>

**透過該功能，無論你是否會開發，你都可以無限擴充套件人升的可能性！**

具體呼叫規則請看下文。

---

## 介面文件

### 基礎知識 - 示例

| 型別     | 說明                                                         |
| -------- | ------------------------------------------------------------ |
| 示例     | [lifeup://api/toast?text=你學會了呼叫！&type=1&isLong=true](lifeup://api/toast?text=你學會了呼叫！&type=1&isLong=true) |
| 介面格式 | 固定字首/方法名?引數1=數值1&引數2=數值2                      |
| 固定字首 | lifeup://api/                                                |
| 方法名   | toast                                                        |
| 引數     | ?text=你學會了呼叫！&type=1&isLong=true                      |

<br/>

### 基礎知識 - 轉義

如果你的引數的數值裡面有+、空格、=、%、&、#等特殊符號，需要轉義處理：

| 特殊字元 | 代表含義                     | 替換內容 |
| :------- | :--------------------------- | :------- |
| +        | URL 中+號表示空格            | +        |
| 空格     | URL中的空格可以用+號或者編碼 | %20      |
| /        | 分隔目錄和子目錄             | %2F      |
| ?        | 分隔實際的URL和引數          | %3F      |
| %        | 指定特殊字元                 | %        |
| #        | 表示書籤                     | %23      |
| &        | URL 中指定的引數間的分隔符   | %26      |
| =        | URL 中指定引數的值           | %3D      |

比如上述例子中的文字內容，如果要最終提示的文字是：?text=你學會了呼叫！

則需要替換文字中的特殊符號`?`和`=`為，最終效果為：

[lifeup://api/toast?text=%3Ftext%3D你學會了呼叫！&type=1&isLong=true](lifeup://api/toast?text=%3Ftext%3D你學會了呼叫！&type=1&isLong=true)

<br/>

### 基礎知識 - 人升資料 ID

「人升」中的資料儲存基本都會有一個唯一 id。

下述的部分介面支援修改**指定**的商品、完成**指定**的任務。

爲了讓「人升」能找到對應的資料，你需要為其提供 id。

**你可以啟用「設定」-「實驗」-「開發者模式」，即可在應用內的各個詳情頁面檢視到資料的原始id。**

比如力量（1），它的屬性id就是1。

#### 事項 id

可以在事項詳情頁面檢視。

id：如果是重複任務，每次重複，id都會更新。

gid: 事項組id，針對同一個重複任務，其 gid 都不會發生變化。

#### 清單 id

開啟「開發者模式」後，在「選擇清單」彈窗檢視。

#### 屬性 id

開啟「開發者模式」後，在「自定義屬性」頁面檢視。

#### 商品 id

「開發者模式」，然後點選商品檢視詳情檢視。

#### 成就條件 id

為成就自定義解鎖條件「需要外部API呼叫以解鎖」後，可以在詳情頁面看到條件id

<br/>

### 彈出訊息

**方法名：**toast

**說明：**彈出各種樣式的訊息

**示例：**[[lifeup://api/toast?text=好好生活，好好吃飯！&type=1&isLong=true](lifeup://api/toast?text=好好生活，好好吃飯！&type=1&isLong=true)](lifeup://api/goto?page=lab)

**解釋：**以獎勵樣式彈出提示“好好生活，好好吃飯！”，並且顯示較長時間。

> 點選示例的連結可以測試效果

| 引數   | 含義             | 取值            | 示例           | 是否必須 | 備註                                                         |
| ------ | ---------------- | --------------- | -------------- | -------- | ------------------------------------------------------------ |
| text   | 要提示的文字訊息 | 任意文字        | 你學會了呼叫！ | 是       |                                                              |
| type   | 文字樣式型別     | 數字從0到6其一  | 1              | 否       | 0 - 普通樣式<br/>1 - 獎勵樣式<br/>2 - 番茄樣式<br/>3 - 成功樣式<br/>4 - 提示樣式<br/>5 - 警告樣式<br/>6 - 錯誤樣式 |
| isLong | 顯示時長         | true 或者 false | true           | 否       | true - 長<br/>false - 短                                     |

<br/>

### 獎勵

**方法名：**reward

**說明：**直接提供獎勵，可定製獎勵理由

**示例：**

- 獲得 1 點金幣，獲得原因為「學習API呼叫」。且原因會在金幣詳情頁面展示：

  [lifeup://api/reward?type=coin&content=學習API呼叫&number=1](lifeup://api/reward?type=coin&content=學習API呼叫&number=1)

- 獲得 300 點「學識、創造力」經驗值，獲得原因為「學習API呼叫」。且原因會在經驗值詳情頁面展示：

  [lifeup://api/reward?type=exp&content=學習API呼叫&number=300&skills=2&skills=6](lifeup://api/reward?type=exp&content=學習API呼叫&number=300&skills=2&skills=6)

- 獲得 1 個模糊匹配「金幣」商品，獲得原因為「學習API呼叫」。且原因會在倉庫歷史頁面展示：

  [lifeup://api/reward?type=item&content=學習API呼叫&number=1&item_name=金幣](lifeup://api/reward?type=item&content=學習API呼叫&number=1&item_name=金幣)

| 引數      | 含義             | 取值                                   | 示例        | 是否必須 | 備註                                                         |
| --------- | ---------------- | -------------------------------------- | ----------- | -------- | ------------------------------------------------------------ |
| type      | 獎勵型別         | 目前僅支援：<br/>coin<br/>exp<br/>item | coin        | 是       | coin - 金幣<br/>exp - 經驗值<br/>item - 商品                 |
| content   | 獎勵原因         | 任意文字                               | 學習API呼叫 | 是       |                                                              |
| skills    | 技能（屬性）     | 大於 0 的數字陣列                      | 1           | 否       | 僅當 type 為 exp 時可用<br/>支援陣列（如&skills=1&skills=2&skills=3）<br/>獲取方式請檢視上文 「基礎知識 - 人升資料 ID」 |
| number    | 獎勵數量         | 大於 0 的數字                          | 1           | 是       | 如果是金幣，取值最大為999999<br/>如果是經驗值，取值最大為99999<br/>如果是商品，取值最大為99 |
| item_id   | 商品id           | 大於 0 的數字                          | 1           | 否*      | 僅當 type 為 item 時可用                                     |
| item_name | 商品名稱         | 任意文字                               | 金幣        | 否*      | 僅當 type 為 item 時可用，模糊匹配                           |
| silent    | 是否要禁用UI提示 | true 或者 false                        | false       | 否       | 預設為 false                                                 |

<br/>

### 懲罰

**方法名：**penalty

**說明：**直接提供懲罰，可定製懲罰理由

**示例：** *基本同獎勵介面

- 懲罰 1 點金幣，獲得原因為「睡了懶覺」。且原因會在金幣詳情頁面展示：

  [lifeup://api/penalty?type=coin&content=睡了懶覺&number=1](lifeup://api/penalty?type=coin&content=睡了懶覺&number=1)

- 懲罰 300 點「力量」經驗值，原因為「睡了懶覺」。且原因會在經驗值詳情頁面展示：

  [lifeup://api/penalty?type=exp&content=睡了懶覺&number=300&skills=1](lifeup://api/penalty?type=exp&content=睡了懶覺&number=300&skills=1)

- 懲罰 1 個模糊匹配「金幣」商品，原因為「睡了懶覺」。且原因會在倉庫歷史頁面展示：

  [lifeup://api/penalty?type=item&content=睡了懶覺&number=1&item_name=金幣](lifeup://api/penalty?type=item&content=睡了懶覺&number=1&item_name=金幣)

| 引數      | 含義             | 取值                                   | 示例     | 是否必須 | 備註                                                         |
| --------- | ---------------- | -------------------------------------- | -------- | -------- | ------------------------------------------------------------ |
| type      | 懲罰型別         | 目前僅支援：<br/>coin<br/>exp<br/>item | coin     | 是       | coin - 金幣<br/>exp - 經驗值<br/>item - 商品                 |
| content   | 懲罰原因         | 任意文字                               | 睡了懶覺 | 是       |                                                              |
| skills    | 技能（屬性）     | 大於 0 的數字陣列                      | 1        | 否       | 僅當 type 為 exp 時可用<br/>支援陣列（如&skills=1&skills=2&skills=3）<br/>獲取方式請檢視上文 「基礎知識 - 人升資料 ID」 |
| number    | 獎勵數量         | 大於 0 的數字                          | 1        | 是       | 如果是金幣，取值最大為999999<br/>如果是經驗值，取值最大為99999<br/>如果是商品，取值最大為99 |
| item_id   | 商品id           | 大於 0 的數字                          | 1        | 否*      | 僅當 type 為 item 時可用                                     |
| item_name | 商品名稱         | 任意文字                               | 金幣     | 否*      | 僅當 type 為 item 時可用，模糊匹配                           |
| silent    | 是否要禁用UI提示 | true 或者 false                        | false    | 否       | 預設為 false                                                 |

<br/>

### 任務

#### 新增任務

**方法名：**add_task

**說明：**自動新增任務

**示例：**

[lifeup://api/add_task?todo=這是自動新增的任務&notes=備註&coin=10&coin_var=1&exp=2048&skills=1&skills=2&skills=3&category=0&item_name=金幣](lifeup://api/add_task?todo=這是自動新增的任務&notes=備註&coin=10&exp=2048&skills=1&skills=2&skills=3&category=0&item_name=金幣)

**解釋：**向預設清單（id為0）中新增一個內容為“這是自動新增的任務”，備註為“備註”，金幣獎勵為10~11隨機，經驗值獎勵為2048，選擇的技能id為1、2、3（一般對應前3個內建屬性），商品獎勵為模糊搜尋一件“金幣”商品。

| 引數        | 含義           | 取值                 | 示例 | 是否必須 | 備註                                                         |
| ----------- | -------------- | -------------------- | ---- | -------- | ------------------------------------------------------------ |
| todo        | 任務內容       | 任意文字             | coin | 是       | coin - 金幣                                                  |
| notes       | 備註           | 任意文字             | 備註 | 否       |                                                              |
| coin        | 金幣獎勵       | 大於 0 的數字        | 10   | 否       | 取值最大為999999                                             |
| coin_var    | 金幣獎勵偏移值 | 大於 0 的數字        | 1    | 否       | 如果該數值大於0，完成任務時，金幣會隨機計算區間為[coin, coin+coin_var] |
| exp         | 經驗值獎勵     | 大於 0 的數字        | 1    | 否       | 取值最大為99999                                              |
| skills      | 屬性（技能）id | 大於 0 的數字陣列    | 1    | 否       | 支援陣列（即&skills=1&skills=2&skills=3）<br/>獲取方式請檢視上文 「基礎知識 - 人升資料 ID」 |
| category    | 清單id         | 大於或等於 0 的數字  | 0    | 否       | 0 或不傳遞代表預設清單，不能選擇智慧清單<br/>獲取方式請檢視上文 「基礎知識 - 人升資料 ID」 |
| frequency   | 重複頻次       | 數字，取值範圍見備註 | 0    | 否       | 預設為0<br/>0 - 單次<br/>1 - 每日<br/>大於 0 的其他數字 - 每 N 日<br/>-1 - 無限<br/>-4 - 每月<br/> -5 - 每年 |
| importance  | 重要程度       | 數字 [1, 4]          | 1    | 否       | 預設為1                                                      |
| difficulty  | 困難程度       | 數字 [1, 4]          | 2    | 否       | 預設為1                                                      |
| item_id     | 獎勵商品的id   | 大於 0 的數字        | 1    | 否       | 如需獎勵商品，只需要提供id或名稱其一<br/>獲取方式請檢視上文 「基礎知識 - 人升資料 ID」 |
| item_name   | 獎勵商品的名稱 | 任意文字             | 寶箱 | 否       | 如需獎勵商品，只需要提供id或名稱其一<br/>名稱會用於模糊匹配  |
| item_amount | 獎勵數量       | [1, 99]              | 1    | 否       | 預設為1                                                      |

<br/>

#### 完成任務

**方法名：**complete

**說明：**觸發任務完成，只會搜索到未完成的任務

**示例：**

- 完成id為1的任務：[lifeup://api/complete?id=1](lifeup://api/complete?id=1)
- 完成「任務組id」為1的任務：[lifeup://api/complete?gid=1](lifeup://api/complete?gid=1)
- 根據名字搜尋任務並完成：[lifeup://api/complete?name=開始使用&ui=true](lifeup://api/complete?name=開始使用&ui=true)

**解釋：**

每個任務都有一個 id。

對於重複任務而言，每次重複id都會重新整理，但「任務組id」會保持不變。

id 的獲取方法為「實驗」頁面開啟「開發者模式」，然後在「任務詳情」頁面即可檢視。

| 引數 | 含義           | 取值          | 示例 | 是否必須 | 備註                                           |
| ---- | -------------- | ------------- | ---- | -------- | ---------------------------------------------- |
| id   | 任務id         | 大於 0 的數字 | coin | 否*      | 任務id；如果是重複任務，每次重複，id都會更新。 |
| gid  | 任務組id       | 大於 0 的數字 | 備註 | 否*      | 任務組id；                                     |
| name | 名稱           | 任意文字      | 10   | 否*      | 模糊搜尋，只會完成搜索到的其中一個任務         |
| ui   | 是否展示彈窗UI | true 或 false | true | 否       | 預設為 false，只在後臺顯示一條訊息             |

**注意：**

1. 爲了能夠匹配到任務，id、gid、name 必須提供其一。

<br/>

### 商店設定

**方法名：**shop_settings

**說明：**調整各種商店設定

**示例：**

-
將ATM利率設定為0.01%：[lifeup://api/shop_settings?key=atm_interest&value=0.01](lifeup://api/shop_settings?key=atm_interest&value=0.01)
-
每次點選將利率提升0.01%：[lifeup://api/shop_settings?key=atm_interest&value=0.01&set_type=relative](lifeup://api/shop_settings?key=atm_interest&value=0.01&set_type=relative)

| 引數     | 含義         | 取值                                                         | 示例         | 是否必須 | 備註                                                         |
| -------- | ------------ | ------------------------------------------------------------ | ------------ | -------- | ------------------------------------------------------------ |
| key      | 型別         | 目前僅支援：<br/>atm_interest<br/>credit_interest<br/>line_of_credit<br/>discount_rate_for_returning | atm_interest | 是       | atm_interest - ATM日利率<br/>credit_interest - 貸款日利率<br/>line_of_credit - 可貸款金額<br/>discount_rate_for_returning - 退貨打折比例 |
| value    | 數值         | 浮點數（小數點）                                             | 0.01         | 是       | 不同的 key 對應不同的數值範圍                                |
| set_type | 如何設定數值 | 以下數值其一：<br/>absolute<br/>relative                     | absolute     | 否       | absolute - 絕對取值，即直接將目標設定為 value<br/>relative - 相對取值，在原數值的基礎上增加或減少 |

<br/>

### 跳轉

**方法名：**goto

**說明：**跳轉「人升」中的某個頁面

**示例：**[lifeup://api/goto?page=lab](lifeup://api/goto?page=lab)

**解釋：**跳轉到實驗頁面

| 引數 | 含義 | 取值                                                         | 示例 | 是否必須 | 備註 |
| ---- | ---- | ------------------------------------------------------------ | ---- | -------- | ---- |
| page | 頁面 | 固定以下數值其一：<br/>main<br/>setting<br/>about<br/>pomodoro<br/>feelings<br/>achievement<br/>history<br/>add_task<br/>add_achievement<br/>add_achievement_cate<br/>exp<br/>coin<br/>backup<br/>add_item<br/>lab<br/>custom_attributes<br/>pomodoro_record<br/>dlc<br/>pomodoro_record<br/>synthesis<br/>pic_manage | lab  | 是       |      |

<br/>

### 商品

#### 新增商品

**方法名：**add_item

**說明：**建立商品，圖示僅支援網路地址，暫不支援自定義使用效果。

**示例：**[lifeup://api/add_item?name=休息10分鐘&desc=去好好休息一小段時間吧！&price=10&action_text=休息](lifeup://api/add_item?name=休息10分鐘&desc=去好好休息一小段時間吧！&price=10&action_text=休息)

**解釋：**建立一個名稱為「休息10分鐘」，描述為「去好好休息一小段時間吧！」，操作文案為「休息」的價格10金幣的商品。

| 引數             | 含義         | 取值             | 示例         | 是否必須 | 備註                 |
| ---------------- | ------------ | ---------------- | ------------ | -------- | -------------------- |
| name             | 商品名稱     | 任意文字         | 休息10分鐘   | 是       | 商品名稱             |
| desc             | 描述         | 任意文字         | 獲得一個禮物 | 否       |                      |
| icon             | 圖示         | 任意文字         |              | 否       | 圖示應為網路地址 URL |
| price            | 價格數值     | 數字 [0, 999999] | 1            | 否       |                      |
| action_text      | 操作按鈕文案 | 任意文字         | 休息         | 否       |                      |
| disable_purchase | 是否禁用購買 | true 或 false    | 1            | 否       | 預設 false           |
| stock_number     | 庫存數       | [-1, 99999]      | 1            | 否       |                      |

<br/>

#### 調整商品

**方法名：**item

**說明：**對指定 id 的商品的各種操作，僅支援【在架】商品。

**示例：**[lifeup://api/item?id=1&set_price=1&set_price_type=relative&own_number=1&own_number_type=relative](lifeup://api/item?id=1&set_price=1&set_price_type=relative&own_number=1&own_number_type=relative)

**解釋：**對 id 為 1 的商品，將其價格提升 1 金幣，並提升擁有數 1

| 引數              | 含義                      | 取值                                     | 示例         | 是否必須 | 備註                                                         |
| ----------------- | ------------------------- | ---------------------------------------- | ------------ | -------- | ------------------------------------------------------------ |
| id                | 商品id                    | 大於0的數字                              | 1            | 否*      | 獲取方式請檢視上文 「基礎知識 - 人升資料 ID」                |
| name              | 商品名稱                  | 任意文字                                 | 寶箱         | 否*      | 用於未知 id 時，模糊搜尋商品，並非修改名稱                   |
| set_name          | 修改名稱                  | 任意文字                                 | 寶箱         | 否       | 不可為空                                                     |
| set_desc          | 修改描述                  | 任意文字                                 | 獲得一個禮物 | 否       |                                                              |
| set_icon          | 修改圖示                  | 任意文字                                 |              | 否       | 圖示應為網路地址 URL                                         |
| set_price         | 調整價格數值              | 數字                                     | 1            | 否       |                                                              |
| set_price_type    | 調整價格方式（絕對/相對） | 以下數值其一：<br/>absolute<br/>relative | relative     | 否       | absolute - 絕對取值，即直接將目標設定為 value<br/>relative - 相對取值，比如在原數值的基礎上增加或減少 |
| own_number        | 調整擁有數                | 數字                                     | 1            | 否       |                                                              |
| own_number_type   | 調整價格方式（絕對/相對） | 以下數值其一：<br/>absolute<br/>relative | relative     | 否       | absolute - 絕對取值，即直接將目標設定為 value<br/>relative - 相對取值，比如在原數值的基礎上增加或減少 |
| stock_number      | 庫存數                    | 大於或等於 0 的數字                      | 1            | 否       |                                                              |
| stock_number_type | 調整價格方式（絕對/相對） | 以下數值其一：<br/>absolute<br/>relative | relative     | 否       | absolute - 絕對取值，即直接將目標設定為 value<br/>relative - 相對取值，比如在原數值的基礎上增加或減少 |

**注意：**

1. 爲了搜索到商品，必須提供 id 或 name 其一。

<br/>

#### 調整開箱效果

**方法名：**loot_box

**說明：**修改指定箱子的開箱效果，支援調整機率、獎勵數和增加內容物。（暫不支援刪除）

**示例：**[lifeup://api/loot_box?name=金幣箱&sub_name=【大】袋金幣&set_type=relative&probability=1&fixed=false](lifeup://api/loot_box?name=金幣箱&sub_name=【大】袋金幣&set_type=relative&amount=1&probability=1&fixed=false)

**解釋：**增加金幣箱中的【大】袋金幣的比重 1 點。

| 引數        | 含義                  | 取值                                     | 示例         | 是否必須 | 備註                                                         |
| ----------- | --------------------- | ---------------------------------------- | ------------ | -------- | ------------------------------------------------------------ |
| id          | 商品id                | 大於0的數字                              | 1            | 否*      | 獲取方式請檢視上文 「基礎知識 - 人升資料 ID」                |
| name        | 商品名稱              | 任意文字                                 | 金幣箱       | 否*      | 用於未知 id 時，模糊搜尋商品，並非修改名稱                   |
| sub_id      | 箱子內容物的 id       | 大於0的數字                              | 1            | 否*      | 箱子內容物的 id                                              |
| sub_name    | 箱子內容物的名稱      | 任意文字                                 | 【大】袋金幣 | 否*      | 用於箱子內容物未知 id 時，模糊搜尋商品                       |
| set_type    | 調整方式（絕對/相對） | 以下數值其一：<br/>absolute<br/>relative | relative     | 否       | absolute - 絕對取值，即直接將目標設定為 value<br/>relative - 相對取值，比如在原數值的基礎上增加或減少 |
| amount      | 獎勵數                | 數字                                     | 1            | 否       | 某個單一物品的獎勵個數                                       |
| probability | 獎勵比重              | 數字                                     | relative     | 否       | absolute - 絕對取值，即直接將目標設定為 value<br/>relative - 相對取值，比如在原數值的基礎上增加或減少 |
| fixed       | 是否是固定獎勵        | 大於或等於 0 的數字                      | 1            | 否       |                                                              |

**注意：**

1. 爲了搜索到商品，必須提供 id 或 name 其一。
1. 爲了搜索到內容物，必須提供 sub_id 或 sub_name 其一。

<br/>

### 新增番茄記錄

**方法名：**add_pomodoro

**說明：**新增番茄計時記錄

**示例：**

- 新增時長為 25 分鐘（1500000 毫秒）的計時記錄，並指向名稱包含學習的任務：[lifeup://api/add_pomodoro?task_name=學習&duration=1500000](lifeup://api/add_pomodoro?task_name=學習&duration=1500000)
- 新增2022-08-01 11:00:00 - 2022-08-01 12:00:00 的計時記錄：[lifeup://api/add_pomodoro?start_time=1659322800000&end_time=1659326400000](lifeup://api/add_pomodoro?start_time=1659322800000&end_time=1659326400000)

**解釋：**

任務id/任務組id的解釋可以檢視上文的「完成任務」介面。



| 引數            | 含義         | 取值                          | 示例          | 是否必須 | 備註                                          |
| --------------- | ------------ | ----------------------------- | ------------- | -------- | --------------------------------------------- |
| start_time      | 計時開始時間 | 時間戳                        | 1659322800000 | 否*      | 可以百度瞭解時間戳的定義                      |
| duration        | 專注時長     | 數字（毫秒）<br/>需大於 30000 | 1500000       | 否*      |                                               |
| end_time        | 計時結束時間 | 時間戳                        | 1659326400000 | 否*      |                                               |
| reward_tomatoes | 是否獎勵番茄 | true 或者 false               | true          | 否       | 預設為 true                                   |
| task_id         | 任務id       | 大於 0 的數字                 | coin          | 否       | 獲取方式請檢視上文 「基礎知識 - 人升資料 ID」 |
| task_gid        | 任務組id     | 大於 0 的數字                 | 備註          | 否       | 獲取方式請檢視上文 「基礎知識 - 人升資料 ID」 |
| task_name       | 名稱         | 任意文字                      | 10            | 否       | 模糊搜尋，只會搜索到的其中一個任務            |

**注意：**

1. start_time, duration, end_time 必須提供其一。
2. 在只有 duration 的情況下，會預設 end_time 為當前時間。
3. end_time 需要大於  start_time。
4. duration 至少為 30000 毫秒（30秒）。
5. 如果同時提供了 start_time, duration, end_time，duration 應該比 (end_time - start_time) 小或相等。

<br/>

### 解鎖成就條件

**方法名：**unlock_condition

**說明：**解鎖成就條件：需要外部API呼叫以解鎖

**示例：**

- 呼叫解鎖 id 為 2 的解鎖條件：[lifeup://api/unlock_condition?id=2](lifeup://api/unlock_condition?id=2)

| 引數 | 含義   | 取值          | 示例 | 是否必須 | 備註                                          |
| ---- | ------ | ------------- | ---- | -------- | --------------------------------------------- |
| id   | 條件id | 大於 0 的數字 | 2    | 是       | 獲取方式請檢視上文 「基礎知識 - 人升資料 ID」 |

<br/>

### 特殊介面

### 彈窗

**方法名：**confirm_dialog

**說明：**彈出一個選擇彈窗，可以自定義標題、文字、積極按鈕、消極按鈕。點選按鈕時也可以呼叫其他介面。

**示例：**

- [lifeup://api/confirm_dialog?title=你相信愛嗎&positive_action=lifeup:%2F%2Fapi%2Ftoast%3Ftext%3D相信&negative_action=lifeup:%2F%2Fapi%2Ftoast%3Ftext%3D不相信](lifeup://api/confirm_dialog?title=你相信愛嗎&positive_action=lifeup:%2F%2Fapi%2Ftoast%3Ftext%3D相信&negative_action=lifeup:%2F%2Fapi%2Ftoast%3Ftext%3D不相信)

- 其他使用場景：

  獎勵二選一

  分支選擇

| 引數            | 含義               | 取值            | 示例                                         | 是否必須 | 備註                                                         |
| --------------- | ------------------ | --------------- | -------------------------------------------- | -------- | ------------------------------------------------------------ |
| title           | 彈窗標題           | 任意文字        | 標題                                         | 是       |                                                              |
| message         | 彈窗詳細描述       | 任意文字        | 這是彈窗內容                                 | 否       |                                                              |
| positive_text   | 積極按鈕文案       | 任意文字        | 確定                                         | 否       |                                                              |
| negative_text   | 消極按鈕文案       | 任意文字        | 拒絕                                         | 否       |                                                              |
| positive_action | 積極按鈕的連結響應 | URL（其他介面） | lifeup:%2F%2Fapi%2Ftoast%3Ftext%3D你點了確定 | 否       | 實際上就是彈出訊息介面經過轉義的文字。轉義規則可參考`基礎知識-轉義`。 |
| negative_action | 消極按鈕的連結響應 | URL（其他介面） | 同上                                         | 否       |                                                              |
| cancel_action   | 取消彈窗的連結響應 | URL（其他介面） | 同上                                         | 否       |                                                              |

<br/>


#### 變數佔位符

「人升」提供了對引數的使用者介入處理手段。

| 佔位符           | 含義                               | 示例                   |
| ---------------- | ---------------------------------- | ---------------------- |
| [$text\|標題]    | 文字佔位符                         | [$text\|輸入任務名稱]  |
| [$number\|標題]  | 數字佔位符（不含小數點）           | [$number\|輸入價格]    |
| [$decimal\|標題] | 數字佔位符（含小數點）             | [$number\|輸入ATM利率] |
| [$item]          | 選擇商品，將被替換為商品id         | [$item]                |
| [$task_category] | 選擇任務清單，將被替換為任務清單id | [$task_category]       |

**示例1：使用時，選擇物品降價1金幣**

比如當你設定為某個商品降價的 api 後，**可能希望在呼叫的時候，再允許使用者選擇指定商品。**而非呼叫時就指定 id。

以下 api 只能讓 id 為 1 的商品降價 1 金幣：

```url
lifeup://api/item?id=1&set_price=-1&set_price_type=relative
```

只需要將商品 id 修改爲佔位符`[$item]`，就可以實現呼叫的時候，使用者能主動選擇想要降價的商品：

[lifeup://api/item?id=[$item|請選擇你想要降價1金幣的商品]&set_price=-1&set_price_type=relative](lifeup://api/item?id=[$item|請選擇你想要降價1金幣的商品]&set_price=-1&set_price_type=relative)



**示例2：任務模板，只需要輸入任務名稱和選擇清單，即可建立提前設定好的獎勵模板**

[lifeup://api/add_task?todo=[$text|輸入任務名稱]&notes=這是個任務的獎勵模板&coin=10&coin_var=10&exp=2048&skills=1&skills=2&skills=3&category=[$task_category]](lifeup://api/add_task?todo=[$text|輸入任務名稱]&notes=這是個任務的獎勵模板&coin=10&coin_var=10&exp=2048&skills=1&skills=2&skills=3&category=[$task_category])


<br/>

#### 結束回撥

所有介面你都可以加上`callback`引數，實現呼叫後回撥該`URL`的處理。

這也可以用於拼接多個介面，比如想要實現跳轉後提示激勵語：

lifeup://api/goto?page=lab + lifeup://api/toast?text=callback

可以使用`callback`引數，參考上文**基礎知識-轉義**，就可以寫出這種的處理：

[lifeup://api/goto?page=lab&callback=lifeup:%2F%2Fapi%2Ftoast%3Ftext%3D測試callback](lifeup://api/goto?page=lab&callback=lifeup:%2F%2Fapi%2Ftoast%3Ftext%3D測試callback)



當然，你也完全可以為一個商品新增多個連結來實現該效果。

該回調更多是用於：

A應用 -> 人升 -> A應用

或

A應用 -> 人升 -> B應用

<br/>

---

## 聯動

我們非常歡迎其他開發者任何形式的聯動。

### 需要更多 API？

API 功能目前僅經過了一個版本的迭代。

未來我們會持續加入更多的 API，以滿足更多的使用場景。

如果你有需要的 API 場景，可以在 [Github 留下 Issues](https://github.com/Ayagikei/LifeUp/issues/new/choose) 或者我們的 [QQ 頻道](https://ti.qq.com/open_qq/index.html?url=https%3A%2F%2Fqun.qq.com%2Fqqweb%2Fqunpro%2Fshare%3F_wv%3D3%26_wwv%3D128%26appChannel%3Dshare%26inviteCode%3D1W7IRQv%26businessType%3D9%26from%3D246610%26biz%3Dka%23%2Fout)進行留言。

<br/>


### 如何呼叫

#### Android

```kotlin
    /**
    * 定義一個方法處理 uri
    */
    private fun call(context: Context, uriString: String){
        try {
            val intent = Intent(Intent.ACTION_VIEW).apply {
                data = Uri.parse(uriString)
            }
            context.startActivity(intent)
        }catch (e: Exception) {
            e.printStackTrace()
        }
    }

	fun xxx() {
        ...
        // 然後在合適的地方呼叫即可
        call(context, "lifeup://api/toast?text=你學會了呼叫！&type=1&isLong=true")
        ...
    }
```

<br/>

#### 網頁

網頁呼叫的話，能否觸發也依賴於瀏覽器。常規的瀏覽器如夸克、Chrome、Edge都是可以的。但一些其他的系統內建的瀏覽器，可能會每次彈出時提醒使用者“是否開啟人升”。

如果你是自己開發的內嵌 WebView 應用，需要確保 WebView 能夠處理 lifeup scheme。

如果你想要保證體驗一致的話，可以使用「人升」裡的商品連結效果，並勾選“使用內建瀏覽器”開啟。但由於安全設定，這種方式僅支援 HTTPS 連結（不支援 HTTP）

**HTML**

直接超鏈接跳轉即可

```htm
<a href="lifeup://api/toast?text=你學會了呼叫！&amp;type=1&amp;isLong=true" target="_blank" rel="noopener">點選這裏呼叫</a>
```

**Javascript**

其實也是呼叫超鏈接

```javascript
location.href='lifeup://api/reward?type=coin&content=Wordle沒猜對，安慰獎&number=1'
```

<br/>


### 應用開發者

如果你是應用開發者，且支援與「人升」聯動，實現了有趣的功能和機制。

可以聯絡我們在應用內互相推薦應用。

> 如需 Google Play 上架等也可聯絡協助。

<br/>


### 網頁開發者

如果你是網頁開發者，開發了呼叫「人升」API 的網頁作品，歡迎在應用內透過商品的形式分享你的作品。

也可以聯絡我們進行互相推薦。

如果你的是靜態網頁，且不熟悉託管，也可以聯絡我們協助託管網頁。