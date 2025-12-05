# 小紅書 (Xiaohongshu/RedNote) DNS 封鎖清單

**更新日期**：2025-12-05
**資料來源**：urlscan.io、SRLabs 安全報告、ControlD、網路研究

---

## 一、萬用字元封鎖規則（建議使用）

### 主要網域

| 封鎖規則 | 用途 |
|----------|------|
| `*.xiaohongshu.com` | 主站與所有子網域 |
| `*.xiaohongshu.cn` | 中國網域 |
| `*.xiaohongshu.net` | 備用網域 |
| `*.xiaohongshu.net.cn` | 備用網域 |

### CDN 網域

| 封鎖規則 | 用途 |
|----------|------|
| `*.xhscdn.com` | 主要 CDN |
| `*.xhscdn.net` | CDN 備用 |
| `*.xhscdn.cn` | CDN 中國 |
| `*.xhsredcdn.com` | RED CDN |
| `*.cdnxhs.com` | CDN 備用 |

### 短網址服務

| 封鎖規則 | 用途 |
|----------|------|
| `*.xhslink.com` | 分享短連結 |
| `*.xhslink.cn` | 分享短連結（中國） |
| `*.xhsurl.com` | URL 服務 |
| `*.xhsurl.cn` | URL 服務（中國） |

### 系統服務

| 封鎖規則 | 用途 |
|----------|------|
| `*.xhsdns.com` | DNS 服務 |
| `*.xhsdns.net` | DNS 服務 |
| `*.xhsos.com` | 作業系統服務 |
| `*.xhssys.cn` | 系統服務 |
| `*.xhssys.com` | 系統服務 |
| `*.xhssys.net` | 系統服務 |

### 新發現網域

| 封鎖規則 | 用途 |
|----------|------|
| `*.redelight.info` | RedElight 服務 |
| `*.redelight.com.cn` | RedElight 中國 |
| `*.yuukoo.com.cn` | 關聯服務 |
| `*.hongyunlogistics.com` | 物流服務（紅雲物流） |
| `*.xingin.com` | 公司技術網域（行吟） |

### 第三方追蹤服務（必須額外封鎖）

| 封鎖規則 | 用途 |
|----------|------|
| `*.kuaishouzt.com` | 快手追蹤 SDK |
| `*.kwaizt.com` | 快手追蹤 SDK |

---

## 二、已確認子網域詳細清單

### API 與核心服務（*.xiaohongshu.com）

#### 用戶資料與 API

| 子網域 | 用途 | 優先級 |
|--------|------|--------|
| `edith.xiaohongshu.com` | 主要 API（用戶資料、IM、裝置資訊） | 🔴 高 |
| `as.xiaohongshu.com` | 安全工具/上傳端點 | 🔴 高 |
| `gaia.xiaohongshu.com` | 服務端點 | 🔴 高 |
| `gslb.xiaohongshu.com` | 全域伺服器負載平衡 | 🟡 中 |

#### 日誌收集與監控

| 子網域 | 用途 | 優先級 |
|--------|------|--------|
| `t2.xiaohongshu.com` | 日誌收集（每分鐘 30 秒標記） | 🔴 高 |
| `lng.xiaohongshu.com` | 日誌收集（1-5 分鐘間隔） | 🔴 高 |
| `apm-fe.xiaohongshu.com` | 前端效能監控 | 🔴 高 |
| `apm-native.xiaohongshu.com` | 原生 App 效能監控 | 🔴 高 |
| `modelportrait.xiaohongshu.com` | CPU 監控/模擬器偵測 | 🔴 高 |
| `spider-tracker.xiaohongshu.com` | 反爬蟲追蹤 | 🟡 中 |
| `crash.xiaohongshu.com` | 當機回報 | 🟡 中 |

#### 內容上傳

| 子網域 | 用途 | 優先級 |
|--------|------|--------|
| `ros-upload-ali.xiaohongshu.com` | 阿里雲圖片上傳 | 🔴 高 |
| `ci.xiaohongshu.com` | 圖片 CDN | 🔴 高 |
| `live-room.xiaohongshu.com` | 直播功能 | 🟡 中 |

#### 網頁/平台服務

| 子網域 | 用途 | 優先級 |
|--------|------|--------|
| `www.xiaohongshu.com` | 網頁版主站 | 🔴 高 |
| `fe.xiaohongshu.com` | 前端服務 | 🔴 高 |
| `cdn.xiaohongshu.com` | CDN 服務 | 🔴 高 |
| `ark.xiaohongshu.com` | 千帆平台（商家後台） | 🟡 中 |
| `pro.xiaohongshu.com` | 專業號平台 | 🟡 中 |
| `school.xiaohongshu.com` | 開放平台/開發者 | 🟡 中 |
| `oia.xiaohongshu.com` | App 開啟引導頁 | 🟡 中 |
| `picasso-static.xiaohongshu.com` | 靜態資源 | 🔴 高 |

#### 新發現子網域（來自 Certificate Transparency）

| 子網域 | 用途 | 優先級 |
|--------|------|--------|
| `beta.xiaohongshu.com` | 測試版 | 🟢 低 |
| `test.xiaohongshu.com` | 測試環境 | 🟢 低 |
| `sit.xiaohongshu.com` | 整合測試 | 🟢 低 |
| `flssandbox.xiaohongshu.com` | 沙盒環境 | 🟢 低 |
| `devops.xiaohongshu.com` | DevOps 服務 | 🟢 低 |
| `mojito.devops.xiaohongshu.com` | DevOps 工具 | 🟢 低 |
| `portal.databus.xiaohongshu.com` | 資料匯流排 | 🟡 中 |
| `feishu.xiaohongshu.com` | 飛書整合 | 🟢 低 |
| `dingding.xiaohongshu.com` | 釘釘整合 | 🟢 低 |
| `workweixin.xiaohongshu.com` | 企業微信整合 | 🟢 低 |
| `redacademy.xiaohongshu.com` | 紅學院 | 🟢 低 |
| `xue.xiaohongshu.com` | 學習平台 | 🟢 低 |
| `pgy.xiaohongshu.com` | 蒲公英/內測分發 | 🟢 低 |
| `seedawards.xiaohongshu.com` | 活動獎項 | 🟢 低 |

---

### CDN 子網域（*.xhscdn.com）

#### 影片 CDN

| 子網域 | 雲端供應商 |
|--------|-----------|
| `sns-video-ak.xhscdn.com` | Akamai |
| `sns-video-al.xhscdn.com` | 阿里雲 |
| `sns-video-bd.xhscdn.com` | 百度 |
| `sns-video-cf.xhscdn.com` | Cloudflare |
| `sns-video-hw.xhscdn.com` | 華為雲 |
| `sns-video-qn.xhscdn.com` | 七牛雲 |
| `sns-video-qc.xhscdn.com` | 青雲 |
| `sns-video-exp5-qn.xhscdn.com` | 七牛雲（實驗） |

#### 圖片 CDN

| 子網域 | 雲端供應商 |
|--------|-----------|
| `sns-img-ak.xhscdn.com` | Akamai |
| `sns-img-bd.xhscdn.com` | 百度 |
| `sns-img-hw.xhscdn.com` | 華為雲 |
| `sns-img-qn.xhscdn.com` | 七牛雲 |
| `sns-img-qc.xhscdn.com` | 青雲 |
| `sns-webpic-qc.xhscdn.com` | 青雲（網頁圖片） |
| `sns-avatar-qc.xhscdn.com` | 青雲（頭像） |
| `ov-sns-img-qc.xhscdn.com` | 青雲（海外） |
| `sns-na-i8.xhscdn.com` | 北美節點 |
| `sns-na-i9.xhscdn.com` | 北美節點 |

#### 廣告 CDN

| 子網域 | 雲端供應商 |
|--------|-----------|
| `ads-video-al.xhscdn.com` | 阿里雲 |
| `ads-video-p1.xhscdn.com` | 通用節點 |
| `ads-video-qn.xhscdn.com` | 七牛雲 |
| `ads-video-qc.xhscdn.com` | 青雲 |

#### 其他 CDN

| 子網域 | 用途 |
|--------|------|
| `fe-static.xhscdn.com` | 前端靜態資源 |
| `fe-video-qc.xhscdn.com` | 前端影片 |
| `xhslive-vod.xhscdn.com` | 直播 VOD |

---

## 三、第三方追蹤服務詳細說明

根據 [SRLabs 安全研究報告](https://srlabs.de/blog/xiaohongshu-little-red-book-reads-you)：

| 網域 | 用途 | 收集資料 |
|------|------|----------|
| `open.kuaishouzt.com` | 快手追蹤 SDK | 裝置 ID、行為資料 |
| `open.kwaizt.com` | 快手追蹤 SDK 配置 | 配置請求 |

**重要發現**：
- 小紅書 App 與 78 個不同網域通訊，向 28 個網域發送資料
- 收集的敏感資訊包括：ANDROID_ID、GAID、裝置型號、CPU 頻率、溫度
- 資料透過 gzip 壓縮傳輸以混淆內容
- 即使用戶取消上傳，圖片仍會被發送到 `ros-upload-ali.xiaohongshu.com`

---

## 四、CDN 後綴對照表

| 後綴 | 雲端供應商 |
|------|-----------|
| ak | Akamai |
| al | 阿里雲 |
| bd | 百度 |
| cf | Cloudflare |
| hw | 華為雲 |
| qn | 七牛雲 |
| qc | 青雲 |

---

## 五、App 識別碼

| 平台 | 識別碼 |
|------|--------|
| Android Package | `com.xingin.xhs` |
| iOS Bundle ID | `com.xingin.discover` |

---

## 六、聯絡信箱

| 信箱 | 用途 |
|------|------|
| brandaccount@xiaohongshu.com | 品牌帳號申請 |
| red.ad@xiaohongshu.com | 廣告合作 |

---

## 七、封鎖限制說明

1. **硬編碼 IP 位址**：小紅書 App 可能使用硬編碼的 IP 位址直接連線，繞過 DNS 封鎖
2. **IP 位址數量**：小紅書擁有超過 1,000 個 IP 位址
3. **CDN 動態性**：CDN 子網域可能會新增，建議定期更新
4. **加密 DNS**：需配合封鎖 DoH/DoT 以防繞過

---

## 八、重要注意事項

1. **台灣封鎖措施**：台灣內政部於 2025 年 12 月 4 日下令封鎖小紅書一年，透過 DNS Response Policy Zone 協定執行封鎖。

2. **DNS 封鎖限制**：
   - 小紅書 App 使用多種方式繞過 DNS 封鎖，包括 DoH（DNS over HTTPS）、QUIC 協定、以及可能的硬編碼 IP 位址
   - 單純的 DNS 封鎖可能不完全有效，需要搭配 IP 封鎖或深度封包檢測

3. **隱私問題**：
   - App 會在使用者接受隱私政策前就開始傳送流量到 Facebook
   - 根據 EFF 的分析，小紅書會與騰訊、字節跳動、Facebook 和 Google 分享用戶資料
   - 部分流量使用明文 HTTP 傳輸而非 HTTPS

---

## 九、資料來源

- [SRLabs - Xiaohongshu Security Analysis](https://srlabs.de/blog/xiaohongshu-little-red-book-reads-you)
- [urlscan.io - xhscdn.com](https://urlscan.io/domain/xhscdn.com)
- [urlscan.io - xiaohongshu.com](https://urlscan.io/domain/xiaohongshu.com)
- [ControlD 社群討論](https://docs.controld.com/discuss/678b52149f7acd002add0202)
- [Taipei Times - ISPs ordered to block China's Xiaohongshu](https://www.taipeitimes.com/News/front/archives/2025/12/05/2003848348)
- [裕笠科技 - DNS 封鎖指南](https://www.ublink.org/index.php/service/tech-know/vigor-tech/vigor-lan-dns-block-douyin)
- [EFF - Crimson Memo: Analyzing Privacy Impact of Xiaohongshu](https://www.eff.org/deeplinks/2025/02/crimson-memo-analyzing-privacy-impact-xiaohongshu-aka-red-note)

---

## 十、更新記錄

| 日期 | 更新內容 |
|------|----------|
| 2025-12-05 | 初始版本，整合多來源資料 |
| 2025-12-05 | 新增 Certificate Transparency 發現的子網域 |
| 2025-12-05 | 新增 ControlD 來源的網域（redelight, yuukoo, hongyunlogistics） |
| 2025-12-05 | 新增第三方追蹤服務（kuaishouzt, kwaizt） |
| 2025-12-05 | 新增 xhsredcdn.com, cdnxhs.com CDN 網域 |
| 2025-12-05 | 新增 xingin.com 公司技術網域 |
| 2025-12-05 | 新增 iOS Bundle ID (com.xingin.discover) |
