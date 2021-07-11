# 新版QuantumultX解鎖tiktok規則

註釋：舊版的tiktok只能顯示作者的ID，升級後原先的的規則失效特更新新版的規則，測試tiktok：v20.0.0

------

>（1）添加下方的規則：

- (?<=_region=)CN(?=&) url 307 TW

- (?<=&mcc_mnc=)4 url 307 2

- ^(https?:\/\/(tnc|dm)[\w-]+\.\w+\.com\/.+)(\?)(.+) url 302  $1$3

- (?<=\d\/\?\w{7}_\w{4}=)1[6-9]..(?=.?.?&) url 307 17

>（2）添加下方的主機名：

- *.tiktokv.com
- *.byteoversea.com
- *.tik-tokapi.com

----

- 安裝MitM證書 👉「生成證書」 👉「安裝證書」
- 第一次信任證書👉 「設置」👉「描述文件」
- 第二次信任 👉 「關於本機」 👉 最下方的「證書列表」信任QuantumultX的證書
- 開啟重寫功能
- 配置節點
- 長按右下方藍色圖標 👉 流量設置為 「規則分流」
- 開啟開關即可正常觀看tiktok

------------------

- [Telegram](https://t.me/xwring) 
- [個人telegram](https://t.me/kwaong)
- [我的博客](https://kwaon.wordpress.com/)
- [Facebook粉專](https://www.facebook.com/jsrwon)
- 微信公眾號 

![image](https://github.com/hkjswong/shadowsocksR-setup/blob/master/%E5%BE%AE%E4%BF%A1%E5%85%AC%E7%9C%BE%E8%99%9F.jpg)
