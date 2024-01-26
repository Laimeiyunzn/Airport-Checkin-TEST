# 機場自動簽到
**使用Github Actions自動簽到是違反了Github Actions條款的，如果仍需使用請fork後添加刪除的兩個yml自行使用**

做這個專案主要是看到最近冒出來許多機場註冊就能白嫖，簽到就送流量。然後又順便拿這個專案學習一下Github Actions。
請注意，本項目不討論跟fq有關的話題，僅僅是技術討論，不要詢問白嫖jc等內容！！！
## 功能

廢話，肯定就是機場自動簽到啊。
## 部署

https://xcao.top/post-278.html 水了個博文，操作更詳細

1. Fork此倉庫
2. 到`Settings`→`Secrets`→`Actions` 添加以下參數：

| 參數  | 是否必須  | 內容  | 示例  |
| ------------ | ------------ | ------------ | ------------ |
| EMAIL  | 是  | 註冊機場所用郵箱  | a@example.com  |
| PASSWORD  | 是  | 註冊機場所用密碼  | password1  |
| BASE_URL  | 是  | 機場地址  | https://examplea.com  |
| SCKEY  | 否  | Sever醬秘鑰  | SCTxxxxxxxxxxxxxx  |
| TGBOT  | 否  | Telegram推送bot  | 5xxxxxxx:xxxxxxxxx  |
| TGUSERID  | 否  | Telegram推送人id  | 8xxxxxxxxx  |

3. 轉到`Actions`創建一個workflow，運行一次，以後每天專案都會自動運行。最後，可以到Run sign查看簽到情況，同時也會通過Sever醬發送出去。
## 參考
1. https://github.com/zhjc1124/ssr_autocheckin 用了他的機場簽到代碼。
2. https://github.com/sirodeneko/genshin-sign 參考其Actions的yml。
~~（兩個倉庫均無許可證，讓我有點蒙）~~
最近倉庫https://github.com/sirodeneko/genshin-sign 增加了GPL許可證，在徵求作者同意後，本倉庫依舊保持使用MIT許可證進行開源，以下為與作者通信郵件
[![](https://raw.githubusercontent.com/xiaocao666tzh/imghosting/main/image.png)](https://raw.githubusercontent.com/xiaocao666tzh/imghosting/main/image.png)
