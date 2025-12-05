# 小紅書 (Xiaohongshu/RedNote) 網域清單

此文件記錄小紅書相關的所有已知網域，供 DNS 過濾使用。

---

## 主要網域

| 網域 | 用途 |
| --- | --- |
| xiaohongshu.com | 主要網站 |
| xiaohongshu.cn | 中國域名 |
| xiaohongshu.net | 備用域名 |
| xiaohongshu.net.cn | 備用域名 |

## CDN 網域

| 網域 | 用途 |
| --- | --- |
| xhscdn.com | 主要 CDN |
| xhscdn.net | CDN 備用 |
| xhscdn.cn | CDN 中國域名 |

## 短網址 / 連結服務

| 網域 | 用途 |
| --- | --- |
| xhslink.com | 分享短連結 |
| xhslink.cn | 分享短連結（中國） |
| xhsurl.com | URL 服務 |
| xhsurl.cn | URL 服務（中國） |

## 系統與 DNS 網域

| 網域 | 用途 |
| --- | --- |
| xhsdns.com | DNS 服務 |
| xhsdns.net | DNS 服務 |
| xhsos.com | 作業系統/系統服務 |
| xhssys.cn | 系統服務 |
| xhssys.com | 系統服務 |
| xhssys.net | 系統服務 |

---

## 主要子網域（*.xiaohongshu.com）

### API 端點

| 子網域 | 用途 |
| --- | --- |
| edith.xiaohongshu.com | 主要 API（用戶資料、IM 即時通訊、系統服務、裝置資訊收集） |
| as.xiaohongshu.com | 安全工具/上傳端點 |
| t2.xiaohongshu.com | 日誌收集（每分鐘 30 秒標記發送） |
| lng.xiaohongshu.com | 日誌收集（每 1-5 分鐘發送） |
| apm-native.xiaohongshu.com | 原生 App 效能監控 |
| apm-fe.xiaohongshu.com | 前端效能監控 |
| modelportrait.xiaohongshu.com | CPU 監控與裝置評估（模擬器偵測） |
| spider-tracker.xiaohongshu.com | 反爬蟲追蹤 |
| crash.xiaohongshu.com | 當機回報 |
| gslb.xiaohongshu.com | 全域伺服器負載平衡 |
| live-room.xiaohongshu.com | 直播功能 |
| ros-upload-ali.xiaohongshu.com | 阿里雲圖片上傳（即使取消也會上傳） |

### 網頁/平台服務

| 子網域 | 用途 |
| --- | --- |
| www.xiaohongshu.com | 網頁版主站 |
| fe.xiaohongshu.com | 前端服務 |
| ark.xiaohongshu.com | 千帆平台（商家後台） |
| pro.xiaohongshu.com | 專業號平台 |
| school.xiaohongshu.com | 開放平台/開發者文件 |
| oia.xiaohongshu.com | App 開啟引導頁 |
| ci.xiaohongshu.com | 圖片 CDN |
| gaia.xiaohongshu.com | 服務端點 |
| picasso-static.xiaohongshu.com | 靜態資源 |

---

## CDN 子網域（*.xhscdn.com）

### 影片 CDN

| 子網域 | 雲端供應商 |
| --- | --- |
| sns-video-ak.xhscdn.com | Akamai |
| sns-video-al.xhscdn.com | 阿里雲 |
| sns-video-bd.xhscdn.com | 百度 |
| sns-video-cf.xhscdn.com | Cloudflare |
| sns-video-hw.xhscdn.com | 華為雲 |
| sns-video-qn.xhscdn.com | 七牛雲 |
| sns-video-exp5-qn.xhscdn.com | 七牛雲 |

### 圖片 CDN

| 子網域 | 雲端供應商 |
| --- | --- |
| sns-img-ak.xhscdn.com | Akamai |
| sns-img-bd.xhscdn.com | 百度 |
| sns-img-hw.xhscdn.com | 華為雲 |
| sns-webpic-qc.xhscdn.com | 青雲 |
| sns-avatar-qc.xhscdn.com | 青雲 |
| ov-sns-img-qc.xhscdn.com | 青雲 |
| sns-na-i8.xhscdn.com | - |
| sns-na-i9.xhscdn.com | - |

### 前端/靜態資源

| 子網域 | 用途 |
| --- | --- |
| fe-static.xhscdn.com | 前端靜態資源 |
| fe-video-qc.xhscdn.com | 前端影片 |

### 直播 CDN

| 子網域 | 用途 |
| --- | --- |
| xhslive-vod.xhscdn.com | 直播 VOD |

### 廣告 CDN

| 子網域 | 雲端供應商 |
| --- | --- |
| ads-video-al.xhscdn.com | 阿里雲 |
| ads-video-p1.xhscdn.com | - |
| ads-video-qn.xhscdn.com | 七牛雲 |

---

## 第三方追蹤服務

根據 SRLabs 報告，小紅書使用以下第三方追蹤服務：

| 網域 | 用途 |
| --- | --- |
| open.kuaishouzt.com | 快手追蹤 SDK（收集裝置與行為資料） |
| open.kwaizt.com | 快手追蹤 SDK |

---

## CDN 後綴對照表

| 後綴 | 雲端供應商 |
| --- | --- |
| ak | Akamai |
| al | 阿里雲 |
| bd | 百度 |
| cf | Cloudflare |
| hw | 華為雲 |
| qn | 七牛雲 |
| qc | 青雲 |

---

## App 識別碼

| 識別碼 | 平台 |
| --- | --- |
| com.xingin.xhs | Android Package Name |

---

## 聯絡信箱

| 信箱 | 用途 |
| --- | --- |
| brandaccount@xiaohongshu.com | 品牌帳號申請 |
| red.ad@xiaohongshu.com | 廣告合作 |

---

## 重要注意事項

1. **台灣封鎖措施**：台灣內政部於 2025 年 12 月 4 日下令封鎖小紅書一年，透過 DNS Response Policy Zone 協定執行封鎖。

2. **DNS 封鎖限制**：
   - 小紅書 App 使用多種方式繞過 DNS 封鎖，包括 DoH（DNS over HTTPS）、QUIC 協定、以及可能的硬編碼 IP 位址
   - 單純的 DNS 封鎖可能不完全有效，需要搭配 IP 封鎖或深度封包檢測

3. **隱私問題**：
   - App 會在使用者接受隱私政策前就開始傳送流量到 Facebook
   - 根據 EFF 的分析，小紅書會與騰訊、字節跳動、Facebook 和 Google 分享用戶資料
   - 部分流量使用明文 HTTP 傳輸而非 HTTPS

---

## 參考資料

- [Taipei Times - Taiwan bans Xiaohongshu](https://www.taipeitimes.com/News/front/archives/2025/12/05/2003848348)
- [SRLabs - Xiaohongshu Security Analysis](https://www.srlabs.de/blog-post/xiaohongshu-little-red-book-reads-you)
- [EFF - Crimson Memo: Analyzing Privacy Impact of Xiaohongshu](https://www.eff.org/deeplinks/2025/02/crimson-memo-analyzing-privacy-impact-xiaohongshu-aka-red-note)
- [Control D - Xiaohongshu Blocking](https://docs.controld.com/discuss/66b78f372b2376002bb0b50d)
