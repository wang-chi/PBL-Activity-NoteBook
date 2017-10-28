### The Security of SDN

---

講者

心得

---



#### 什麼是SDN?

* Super-dope Network
* SDN的概念與運作原理

一般的Router都活在自己的世界

SDN-Software-defined Network

SDN的運作原理

1. Controller

一台switch不一定只有一張flow table

核心想法：把各個硬體需要計算的部分集中起來管理，只把實際執行

##### SDN的優點與缺點

* 優點
  * Centralized management  集中管理
  * Global View
  * NFV \(Network Functions Virtualization\)
  * Programmability, flexibility and innovation 
* 缺點
  * Single point of failure
  * New bottleneck for DDoS
  * Not scalable 不容易擴展網路架構
  * Dumb switch is not cheap\(at least for now\)

#### 保護SDN資料傳輸層的安全性

* 攻擊者可以做什麼 Threat Model

  * 任意傳送、丟棄或修改封包
  * 任意新增或刪除flow table規則
  * 同時控制多台switch串通執行攻擊
  * 回報假資料給controller

* 三個偵測與防禦的方法

  * Active Probing 主動探測
    * 核心想法：從controller送測試封包，看能否回來
    * 不用每條flow rule都送封包-&gt;否則網路上都是測試封包
    * Divide and conquer
    * 在準確度和效率取得平衡
  * Statistic Checking 數據檢查
    * 核心想法：檢查switch問相鄰的switch做了什麼
  * * 在不影響原本網路的情況下加上rule當作counter使用
    * 定期檢查switch的counter, 發現不吻合則降低所有相關的switch分數
      * 旁邊的switch可能會陷害
    * 檢查
      * forward相關的rule檢查
      * drop
  * Packet Obfuscation 封包模糊化

    * 核心想法：將封包header的部分加密，讓攻擊者無法達到特定目的
    * 新增flow table action: Encrypt and Decrypt
    * 僅留下routing需要留下的



