Docker Taipei

日期：2017.10.21 Sat.

地點：國立臺中科技大學 資訊樓 2701

內容：

透過Web介面使用Docker：[http://labs.play-with-docker.com/](http://labs.play-with-docker.com/)

#### \# 虛擬化技術的歷史

* IBM zOS
* 虛擬化軟體－VMware, KVM, Xen, VirtualBox
* Hardware-assisted virtualization 硬體加速
* Paravirtualiztion半虛擬化
* 作業系統層虛擬化
  * OpenVZ
  * LXC
  * Docker
* IaaS, PaaS, Saas - Snapshot, Migration

container目前沒有snapshot

#### \# 容器與虛擬化架構差異

1. 一個虛擬機的單位叫做**instance**
2. VM和Container差異在於共用Host OS少掉Gust OS，效能上提升較多
3. VM和Container在於VM會完全隔離，VM有Gust OS，病毒不會互相感染，Container僅有安全隔離
4. Container在啟動速度、性能（接近原生）、

#### \# The Matrix of Hell

只要可以運作Docker的環境都可以移植映像檔

#### \# Docker Engine

Client端可以透過REST API去控制server\(Docker daemon\)

一個容器跑起來在運作就叫做container

容器跟容器之間運作就可以叫做docker network

#### \# Docker Compose

* 一鍵完成多個容器
* docker-compose.yml
* 支援Docker Network
* 支援Docker Volume
* 建構完整軟體服務
  * 如：3-tier
* 快速建置測試模擬環境

#### \# Docker Machine

* 在多種平上建立VM
* 一套工具適用所有雲端平台、虛擬化平台
* 內建Dokcer Engine
* 具備SSH功能

#### \# Docker Swarm

* 容器叢集系統
* 內建分散式鍵值儲存功能

北榮有導入Docker

簡報連結：

相關照片：

