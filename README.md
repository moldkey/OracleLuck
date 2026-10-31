# 🔮 OracleLuck — 天啟好運

**AI 玄學工具與知識庫 | AI Metaphysics Tools & Knowledge Base**

[🌐 網站 Website](https://www.oracleluck.com) · [📚 知識庫](https://www.oracleluck.com/library/) · [🔮 AI 問事](https://www.oracleluck.com/chat/) · [💬 塔羅拍照解讀](https://www.oracleluck.com/tarot/photo/)

---

## ✨ 這是什麼

OracleLuck 是 AI 驅動的**東西方玄學工具與知識庫**。所有解讀由真實曆法／排盤引擎計算，AI 依傳統框架說明，屬文化參考。

OracleLuck is an AI-powered platform for **Eastern and Western metaphysics** — all readings are computed by real calendrical/astrological engines and explained by AI.

---

## 🀄 知識體系 Systems Covered

### 東方命理 Eastern

| 系統 | 頁數 | 連結 |
|---|---:|---|
| 紫微斗數（14 主星 / 12 宮位） | 26 | [查看 →](https://www.oracleluck.com/ziwei/star/) |
| 八字命理（十神 / 干支 / 五行） | 97 | [查看 →](https://www.oracleluck.com/bazi/god/) |
| 易經六十四卦 | 64 | [查看 →](https://www.oracleluck.com/iching/) |
| 觀音靈籤 100 支 | 100 | [查看 →](https://www.oracleluck.com/qian/) |
| 二十四節氣 | 24 | [查看 →](https://www.oracleluck.com/solar-terms/) |
| 二十八星宿 | 28 | [查看 →](https://www.oracleluck.com/mansions/) |

### 西方與其他 Western & More

| 系統 | 頁數 | 連結 |
|---|---:|---|
| 塔羅 78 張完整牌義 | 78 | [查看 →](https://www.oracleluck.com/tarot/) |
| 塔羅牌陣 | 12 | [查看 →](https://www.oracleluck.com/tarot/spreads/) |
| 周公解夢 | 150 | [查看 →](https://www.oracleluck.com/dream/) |
| 西洋十二星座 | 12 | [查看 →](https://www.oracleluck.com/astrology/) |
| 十二生肖 | 12 | [查看 →](https://www.oracleluck.com/zodiac/) |

---

## 🤖 AI 工具 AI Tools

| 功能 | 說明 | 連結 |
|---|---|---|
| 🔮 **AI 問事** | 20 個神明角色的對話，先問診再給建議，每則附依據與合規聲明 | [開始 →](https://www.oracleluck.com/chat/) |
| 📚 **學科助教** | 12 個玄學學科的 AI 家教，四步教學法（拆解→示範→出題→批改） | [開始 →](https://www.oracleluck.com/chat/?mode=learn) |
| 📷 **塔羅拍照解讀** | 拍下牌面 → AI 辨識（含正逆位）→ 結合站內牌義解讀 | [試試 →](https://www.oracleluck.com/tarot/photo/) |
| 🏠 **風水照片問診** | 上傳住宅/商辦/學校/地皮照片，AI 先確認類型再給可逆建議 | [試試 →](https://www.oracleluck.com/fengshui/photo/) |
| 📜 **命盤報告** | 八字／紫微真排盤 + 十節完整分析，可列印 PDF | [查看 →](https://www.oracleluck.com/report/bazi/) |

---

## 📊 開源資料集 Open Datasets

這個 repo 也開源了排盤引擎用的**結構化資料層**：

| 檔案 | 內容 | 筆數 |
|---|---|---:|
| [`data/tarot-78.json`](data/tarot-78.json) | 塔羅 78 張完整牌義（中英、正逆位、愛情、事業、建議） | 78 |
| [`data/ganzhi60.json`](data/ganzhi60.json) | 六十甲子 + 五行 + 納音 | 60 |
| [`data/year_ganzhi.json`](data/year_ganzhi.json) | 年干支生肖表 1900–2100 | 201 |
| [`data/calendar_2026_2028.json`](data/calendar_2026_2028.json) | 逐日黃曆：農曆、干支、節氣、六曜 | 1,096 天 |
| [`data/solar-terms.json`](data/solar-terms.json) | 二十四節氣精確日期 | 72 |
| [`data/rokuyo_table.json`](data/rokuyo_table.json) | 六曜對照表（日本） | 360 |
| [`data/kyusei9.json`](data/kyusei9.json) | 九星気学（日本） | 9 |
| [`data/nakshatra27.json`](data/nakshatra27.json) | 印度二十七宿 | 27 |
| [`data/western-astrology.json`](data/western-astrology.json) | 西洋占星對照（行星/星座/宮/相位） | — |

**授權 License**：資料 CC BY-NC 4.0（需標註來源、不得商業使用）

### 免 key 公開 API

```
https://www.oracleluck.com/data/rules/                        規則表索引
https://www.oracleluck.com/data/rules/calendar_2026_2028.json
https://www.oracleluck.com/data/rules/ganzhi60.json
https://www.oracleluck.com/data/rules/rokuyo_table.json
https://www.oracleluck.com/data/kg.json                       知識圖譜
```

---

## 🧩 免費黃曆 Widget（可嵌入任何網站）

一行 iframe，就能在你的網站顯示今日黃曆（干支、農曆、六曜、建除、沖煞）：

```html
<iframe src="https://www.oracleluck.com/embed/almanac/"
        width="320" height="200" frameborder="0"
        style="border-radius:12px"></iframe>
```

指定日期：

```html
<iframe src="https://www.oracleluck.com/embed/almanac/?date=2027-01-01"
        width="320" height="200" frameborder="0"></iframe>
```

- 免費、免註冊、自動更新
- 純 HTML 2KB，無外部字體、無追蹤腳本
- 底部固定帶署名連結（使用條件）

**線上工具**：[黃曆查詢](https://www.oracleluck.com/tools/almanac/) · [八字排盤](https://www.oracleluck.com/tools/bazi/)

---

## 🔌 免費 JSON API

免 API key、免註冊，直接 GET：

```bash
# 單日黃曆
curl "https://www.oracleluck.com/api/tools/almanac/?date=2026-10-31"

# 八字排盤
curl "https://www.oracleluck.com/api/tools/bazi/?date=1993-05-16&time=12:00"

# 全量日曆（1,096 天）
curl "https://www.oracleluck.com/data/rules/calendar_2026_2028.json"
```

回應範例：

```json
{
  "date": "2026-10-31",
  "lunar": "九月廿二",
  "year_gz": "丙午",
  "month_gz": "戊戌",
  "day_gz": "戊寅",
  "rokuyo": "赤口",
  "jianchu": "定",
  "chong": "申",
  "chong_zodiac": "猴"
}
```

- 限流 240 次/分鐘/IP
- 可商業使用（標註來源）
- **完整文檔**：[www.oracleluck.com/docs/api/](https://www.oracleluck.com/docs/api/)
- **教學文章**：[免費黃曆 API 使用教學](https://www.oracleluck.com/insight/free-almanac-api-tutorial/) · [如何嵌入黃曆 Widget](https://www.oracleluck.com/insight/embed-free-almanac-widget/)


---

## 🛠 技術架構 Tech Stack

- **CMS**: Django 5.2 + PostgreSQL（自建，非 Next.js）
- **前端**: 預編譯 Tailwind CSS（無 CDN 依賴）
- **AI**: DeepSeek-V4.1-Flash（支援視覺）
- **部署**: Ubuntu + Nginx + Gunicorn
- **SEO**: 動態 sitemap（753 URL）+ IndexNow + 結構化數據

---

## 🌏 多語言 Languages

繁體中文 · 简体中文 · English · **日本語**（166 頁已翻譯）

---

## ⚖️ 合規 Compliance

- 所有解讀標明「依據」與「非宗教啟示」
- 不預言生死、疾病、災禍
- 不做醫療、法律、投資建議
- 風水只給可逆建議，施工／結構／水電一律轉介專業
- 完整免責聲明：[www.oracleluck.com/terms/](https://www.oracleluck.com/terms/)

---

## 🔗 相關連結 Links

- 🌐 網站：[www.oracleluck.com](https://www.oracleluck.com)
- 📚 知識庫總覽：[www.oracleluck.com/library/](https://www.oracleluck.com/library/)
- 💬 AI 對話：[www.oracleluck.com/chat/](https://www.oracleluck.com/chat/)
- 📷 塔羅拍照：[www.oracleluck.com/tarot/photo/](https://www.oracleluck.com/tarot/photo/)
- 🏠 風水問診：[www.oracleluck.com/fengshui/](https://www.oracleluck.com/fengshui/)
- ⚖️ 免責聲明：[www.oracleluck.com/terms/](https://www.oracleluck.com/terms/)

---

## 📄 License

資料檔案 CC BY-NC 4.0 · 範例程式碼 MIT · Copyright (c) 2026 OracleLuck
