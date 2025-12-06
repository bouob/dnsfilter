# 抖音/TikTok (ByteDance) DNS 封鎖清單

**更新日期**：2025-12-06
**資料來源**：v2fly/domain-list-community、GitHub 社群、網路研究

---

## 一、字節跳動產品線

| 產品 | 中國版 | 國際版 | 說明 |
|------|--------|--------|------|
| 短視頻 | 抖音 (Douyin) | TikTok | 核心產品 |
| 新聞資訊 | 今日頭條 | TopBuzz/BuzzVideo | 新聞聚合 |
| 長視頻 | 西瓜視頻 | - | 長視頻平台 |
| 直播 | 抖音火山版 | TikTok LIVE | 直播服務 |
| 影片編輯 | 剪映 | CapCut | 影片剪輯 App |
| 圖片社群 | - | Lemon8 | Pinterest 風格 |
| 問答 | 悟空問答 | - | 知識問答 |

---

## 二、萬用字元封鎖規則（建議使用）

### 抖音核心網域

| 封鎖規則 | 用途 |
|----------|------|
| `*.douyin.com` | 抖音主站 |
| `*.douyincdn.com` | 抖音 CDN |
| `*.douyinpic.com` | 抖音圖片 |
| `*.douyinstatic.com` | 抖音靜態資源 |
| `*.douyinvod.com` | 抖音影片點播 |
| `*.iesdouyin.com` | 抖音服務 |
| `*.amemv.com` | 抖音早期域名 |
| `*.douyinact.com` | 抖音活動 |
| `*.douyinact.net` | 抖音活動 |
| `*.douyinfe.com` | 抖音前端 |

### TikTok 核心網域

| 封鎖規則 | 用途 |
|----------|------|
| `*.tiktok.com` | TikTok 主站 |
| `*.tiktokv.com` | TikTok 影片服務 |
| `*.tiktokcdn.com` | TikTok CDN |
| `*.tiktokcdn-us.com` | TikTok CDN（美國） |
| `*.tiktokcdn-eu.com` | TikTok CDN（歐洲） |
| `*.tiktokd.net` | TikTok 服務 |
| `*.tiktokd.org` | TikTok 服務 |
| `*.tiktokv.eu` | TikTok（歐洲） |
| `*.tiktokv.us` | TikTok（美國） |
| `*.tiktokw.eu` | TikTok 網頁（歐洲） |
| `*.tiktokw.us` | TikTok 網頁（美國） |
| `*.tiktokeu-cdn.com` | TikTok 歐洲 CDN |
| `*.tiktokrow-cdn.com` | TikTok ROW CDN |
| `*.tik-tokapi.com` | TikTok API |
| `*.tiktok-row.net` | TikTok ROW |
| `*.tiktokglobalshopv.com` | TikTok Shop |
| `*.tiktokminis.us` | TikTok Minis |
| `*.ttlivecdn.com` | TikTok 直播 CDN |
| `*.ttoverseaus.net` | TikTok 海外美國 |
| `*.ttwstatic.com` | TikTok 靜態資源 |

### Musical.ly 遺留網域

| 封鎖規則 | 用途 |
|----------|------|
| `*.musical.ly` | Musical.ly 主站 |
| `*.muscdn.com` | Musical.ly CDN |
| `*.musemuse.cn` | Musical.ly 中國 |

### 字節跳動基礎設施

| 封鎖規則 | 用途 |
|----------|------|
| `*.bytedance.com` | 公司主站 |
| `*.bytedance.cn` | 公司中國站 |
| `*.bytedance.net` | 公司網路 |
| `*.bytedance.org` | 公司組織 |
| `*.bytecdn.cn` | CDN 服務 |
| `*.bytecdn.com` | CDN 服務 |
| `*.bytedns.net` | DNS 服務 |
| `*.bytednsdoc.com` | DNS 文件 |
| `*.byteimg.com` | 圖片服務 |
| `*.bytetos.com` | 對象存儲 |
| `*.bytescm.com` | 源碼管理 |
| `*.bytegoofy.com` | 內部服務 |
| `*.byted-static.com` | 靜態資源 |
| `*.bytexservice.com` | X 服務 |
| `*.byteoversea.com` | 字節海外 |
| `*.byteoversea.net` | 字節海外 |
| `*.bytefcdn-oversea.com` | 海外 CDN |
| `*.bytefcdn-ttpeu.com` | 歐洲 CDN |
| `*.byteintl.net` | 國際服務 |
| `*.bytelb.com` | 負載平衡 |
| `*.bytelb.net` | 負載平衡 |
| `*.bytemaimg.com` | 圖片服務 |
| `*.bytemastatic.com` | 靜態資源 |
| `*.bytetraffic.net` | 流量服務 |
| `*.bytetstatic.com` | 靜態資源 |
| `*.bytetstatic.net` | 靜態資源 |
| `*.bytevcloudvod.com` | 雲端影片 |
| `*.ibytedtos.com` | 國際對象存儲 |
| `*.ibyteimg.com` | 國際圖片服務 |
| `*.ibytedapm.com` | APM 監控 |

### 追蹤與日誌服務（高優先級）

| 封鎖規則 | 用途 |
|----------|------|
| `*.snssdk.com` | SDK 服務（關鍵追蹤域名） |
| `*.zijieapi.com` | 字節 API |
| `*.zijieimg.com` | 字節圖片 |
| `*.zjbyte.com` | 字節服務 |
| `*.zjcdn.com` | 字節 CDN |
| `*.pstatp.com` | 頭條靜態資源 |

### 今日頭條

| 封鎖規則 | 用途 |
|----------|------|
| `*.toutiao.com` | 今日頭條主站 |
| `*.toutiaoapi.com` | 頭條 API |
| `*.toutiaocdn.com` | 頭條 CDN |
| `*.toutiaocloud.com` | 頭條雲服務 |
| `*.toutiaopage.com` | 頭條頁面服務 |
| `*.toutiao13.com` | 頭條備用 |

### 西瓜視頻

| 封鎖規則 | 用途 |
|----------|------|
| `*.ixigua.com` | 西瓜視頻主站 |
| `*.ixiguavideo.com` | 西瓜視頻 |
| `*.xiguavideo.cn` | 西瓜視頻中國 |
| `*.xiguavideo.net` | 西瓜視頻 |
| `*.bdxiguaimg.com` | 西瓜圖片 |
| `*.bdxiguastatic.com` | 西瓜靜態資源 |

### 火山視頻

| 封鎖規則 | 用途 |
|----------|------|
| `*.huoshan.com` | 火山視頻 |
| `*.huoshanzhibo.com` | 火山直播 |
| `*.huoshancdn.com` | 火山 CDN |
| `*.huoshanimg.com` | 火山圖片 |
| `*.huoshanlive.com` | 火山直播 |

### DNS/負載平衡

| 封鎖規則 | 用途 |
|----------|------|
| `*.gslbdns.com` | 全域負載平衡 |
| `*.gslbdns.net` | 全域負載平衡 |
| `*.fedlearner.net` | 聯邦學習 |

### 其他字節跳動產品

| 封鎖規則 | 用途 |
|----------|------|
| `*.capcut.com` | CapCut 剪映 |
| `*.capcut.net` | CapCut 服務 |
| `*.lemon8-app.com` | Lemon8 |
| `*.feelgood.cn` | 社交服務 |
| `*.feiliao.com` | 飛聊（即時通訊） |
| `*.wukong.com` | 悟空問答 |
| `*.wukongwenda.com` | 悟空問答 |
| `*.gogokid.com.cn` | GoGoKid 教育 |
| `*.pipix.com` | 皮皮蝦 |
| `*.ppximg.com` | 皮皮蝦圖片 |
| `*.gifshow.com` | GIF 服務 |
| `*.kspkg.com` | 快手相關 |

---

## 三、已確認子網域詳細清單

### 追蹤與日誌子網域（高優先級）

| 子網域 | 用途 | 優先級 |
|--------|------|--------|
| `log.snssdk.com` | 日誌收集 | 🔴 高 |
| `xlog.snssdk.com` | 擴展日誌 | 🔴 高 |
| `mon.snssdk.com` | 監控服務 | 🔴 高 |
| `i.snssdk.com` | SDK 服務 | 🔴 高 |
| `effect.snssdk.com` | 效果追蹤 | 🔴 高 |
| `applog.zijieapi.com` | App 日誌 | 🔴 高 |
| `log.tiktokv.com` | TikTok 日誌 | 🔴 高 |

**重要**：封鎖 `log.snssdk.com`、`xlog.snssdk.com`、`i.snssdk.com` 後，抖音 App 會直接顯示載入失敗。

### TikTok API 子網域

| 子網域 | 用途 | 優先級 |
|--------|------|--------|
| `api.tiktokv.com` | TikTok API | 🔴 高 |
| `api-h2.tiktokv.com` | TikTok API H2 | 🔴 高 |
| `ib.tiktokv.com` | TikTok 服務 | 🔴 高 |
| `api2.musical.ly` | Musical.ly API | 🔴 高 |
| `api2-16-h2.musical.ly` | Musical.ly API | 🔴 高 |
| `api2-21-h2.musical.ly` | Musical.ly API | 🔴 高 |
| `log2.musical.ly` | Musical.ly 日誌 | 🔴 高 |
| `mon.musical.ly` | Musical.ly 監控 | 🔴 高 |

### TikTok CDN 子網域

| 子網域 | 用途 | 優先級 |
|--------|------|--------|
| `v16a.tiktokcdn.com` | 影片 CDN | 🔴 高 |
| `v16m.tiktokcdn.com` | 影片 CDN | 🔴 高 |
| `v19.tiktokcdn.com` | 影片 CDN | 🔴 高 |
| `p16-tiktokcdn-com.akamaized.net` | Akamai CDN | 🟡 中 |

### 抖音 API 子網域

| 子網域 | 用途 | 優先級 |
|--------|------|--------|
| `aweme.snssdk.com` | 抖音核心 API | 🔴 高 |
| `api.amemv.com` | 抖音 API | 🔴 高 |

### 海外測試子網域

| 子網域 | 用途 | 優先級 |
|--------|------|--------|
| `abtest-sg-tiktok.byteoversea.com` | 新加坡 A/B 測試 | 🟢 低 |
| `abtest-va-tiktok.byteoversea.com` | 維吉尼亞 A/B 測試 | 🟢 低 |

---

## 四、第三方 CDN 網域

TikTok/抖音使用多個第三方 CDN 服務：

| 網域 | CDN 供應商 |
|------|-----------|
| `p16-tiktokcdn-com.akamaized.net` | Akamai |
| `bytedance.map.fastly.net` | Fastly |
| `worldfcdn.com` | Zenlayer |

---

## 五、App 識別碼

| 平台 | 識別碼 | 說明 |
|------|--------|------|
| Android | `com.ss.android.ugc.aweme` | 抖音 |
| Android | `com.zhiliaoapp.musically` | TikTok |
| Android | `com.ss.android.ugc.trill` | TikTok Lite |
| iOS | `com.zhiliaoapp.musically` | TikTok |
| iOS | `aweme` | 抖音 |

---

## 六、封鎖限制說明

1. **DoH/DoT 繞過**：TikTok/抖音使用 DNS over HTTPS 和 DNS over TLS 繞過傳統 DNS 封鎖，需同時封鎖 DoH/DoT
2. **動態 CDN**：CDN 子網域包含動態生成的數字組合，難以完全列舉
3. **硬編碼 IP**：App 可能內建 IP 位址直接連線
4. **第三方 CDN**：使用 Akamai、Fastly、Zenlayer 等第三方 CDN
5. **Port 53 封鎖**：建議封鎖所有出站 TCP/UDP 53 流量，防止使用替代 DNS

---

## 七、重要注意事項

1. **美國禁令**：2025 年 1 月 18 日，TikTok、CapCut、Lemon8、Gauth、Hypic 在美國被禁止

2. **隱私問題**：
   - TikTok 的 iOS App 被發現注入可監控鍵盤輸入的程式碼
   - 即使不使用 TikTok，網站也可能透過 TikTok 追蹤技術追蹤用戶

3. **關鍵封鎖網域**：封鎖以下網域可使抖音無法載入：
   - `log.snssdk.com`
   - `xlog.snssdk.com`
   - `i.snssdk.com`

---

## 八、資料來源

- [v2fly/domain-list-community - TikTok](https://github.com/v2fly/domain-list-community/blob/master/data/tiktok)
- [v2ray/domain-list-community - ByteDance](https://github.com/v2ray/domain-list-community/blob/master/data/bytedance)
- [M4jx/TikTokBlockList](https://github.com/M4jx/TikTokBlockList)
- [krombopulosM/TikTok-blocklist](https://github.com/krombopulosM/TikTok-blocklist)
- [GitHub Gist - 抖音分流域名](https://gist.github.com/eallion/1ed7f6cc46554c9adcc9edd125d468e5)
- [GitHub Gist - 屏蔽短視頻域名](https://gist.github.com/eallion/bd83ce76ad88ccd6eed113cd5176ec2c)
- [GitHub Gist - 抖音快手 DNS 污染](https://gist.github.com/JamesHopbourn/b5cf9219bdacfa8b6dbb3414276c149b)
- [字節系 DNS 討論](https://github.com/VirgilClyne/GetSomeFries/issues/12)
- [WhoTracks.Me - TikTok Analytics](https://whotracks.me/trackers/tiktok_analytics.html)
- [Axios - ByteDance Apps](https://www.axios.com/2024/04/23/tiktok-ban-bytedance-apps-capcut-lemon8)

---

## 九、更新記錄

| 日期 | 更新內容 |
|------|----------|
| 2025-12-06 | 初始版本，整合多來源資料 |
| 2025-12-06 | 包含抖音、TikTok、今日頭條、西瓜視頻、火山視頻等產品 |
| 2025-12-06 | 新增 CapCut、Lemon8 等新產品網域 |
| 2025-12-06 | 新增追蹤與日誌服務詳細說明 |
| 2025-12-06 | 新增 App 識別碼（Android/iOS） |
