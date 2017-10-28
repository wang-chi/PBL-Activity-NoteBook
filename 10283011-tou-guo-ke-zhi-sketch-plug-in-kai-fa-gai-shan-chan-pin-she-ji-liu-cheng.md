# 透過客製Sketch Plug-in 開發改善產品設計流程

---

講者：楊維中

介紹：UI設計是產品開發過程中的重要一環，但是在實務上，有太多與設計工作相關，但不應該由設計師負責、反而讓設計師分心的工作。我們嘗試改進設計師使用的工具，讓原本需要人力的工作自動化，解放設計師的生產力。

---

### 多國語系服務

* 版權結構的差異
* 法規不同
  * 稅收差異
  * 金流服務
* 中文是字串長度最短的
* 設計初期就先套用多國語文

痛點：翻譯完自傳才發現過長，往往影響開發流程

解法：初期就能夠預覽多國語言字串，而且可以自動化

## Sketch Plugins

URL:[https://www.sketchapp.com/extensions/plugins/](https://www.sketchapp.com/extensions/plugins/)

Google Translation API

## 主題面板

通點：人工手動打包過程不但費時，而且容易出錯

解法：除了上傳過程需要加上驗證機制外，打包過程也應該自動化

* Sketch Plugin開發/CocoaScript

1.  CocoaScript,前身為JSTalk,缺乏IDE/Editor支援，可以使用Objective-J Syntax Hightlight.
2.  錯誤訊息意味不明, 混用JavaScript 與 Objective-C 物件，有時不容易分辨是屬於哪一種類型的物件
3.  因為呼叫macOS系統JavaScript Core直譯器，不同版本OS可以支援的JS與法不同
4.  可呼叫所有Cocoa framework及sketch app中頭所有的class
5.  要用setCOSJSTargetFunction:實作Target/Action
6.  無法實作Delegate/Block，無法呼叫非同步的API
7.  缺少API文件，基本上只能參考github上人家classdump出來的header files.
8.  每一代Sketch能呼叫的API都不太一樣，所以在Sketch升級後，之前寫的Plug-in可能無法使用（Sketch改版不會通知已改版）
9. 




