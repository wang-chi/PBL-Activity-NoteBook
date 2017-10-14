### 從0開始做Android惡意程式分析

##### 分析惡意程式基本要素

1. Permission
2. Http Requests\(POST GET\)
3. Static Program Analysis\(\)

##### 環境準備

* 惡意程式樣本
* 裝置
* 封包擷取
* 逆向分析

##### APK架構

assets:png, 主程式載入檔

lib:用ntk寫的東西

META-INF: 簽名檔

res:icon

##### \(smack技術\)遠端遙控木法分析

smack底層是xmpp

安裝過程中會取得哪些權限

逆向會放到apk studio

隱藏icon讓使用者感受不到



攔截封包

###### Android Http

* HttpURLConnection
* HiipClient
* HttpProtocolParams
* OKHttp
* Volley
* AsyncHttpClient

從套件屬性了解

SO\(Share object, 公想褲\)

* 二進制
* 動態連結褲（類似windows, dll檔\)
* 


