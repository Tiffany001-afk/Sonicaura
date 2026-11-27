<div align="center">

# 🎵 SonicAura

**環境辨識、YouTube 完整播放與多語歌詞同步音樂播放器 ｜ Ambient Music Recognition, YouTube Full Playback & Synced Lyrics Player**

[![License: MIT](https://img.shields.io/badge/License-MIT-7c5cff.svg?style=for-the-badge)](./LICENSE)
[![PWA Ready](https://img.shields.io/badge/PWA-Installable-00d2ff.svg?style=for-the-badge&logo=pwa&logoColor=white)](./manifest.json)
[![Languages: 4](https://img.shields.io/badge/Languages-繁%20|%20简%20|%20EN%20|%20日本語-f59e0b.svg?style=for-the-badge)](#)
[![Zero CDN](https://img.shields.io/badge/Dependencies-Zero%20CDN-22c55e.svg?style=for-the-badge)](#)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-ff4da6.svg?style=for-the-badge&logo=github&logoColor=white)](https://YOUR_USERNAME.github.io/sonicaura/)

[繁體中文介紹](#-專案簡介) • [介面預覽](#-介面預覽--screenshots) • [使用方法](#-使用方法) • [English Version](#-english-version)

</div>

---

## 🖼️ 介面預覽 / Screenshots

> 💡 提示：將您的截圖上傳至專案內的 `screenshots/` 資料夾並依下列檔名命名，即可自動顯示。

| 🎵 整合式播放器、YouTube 完整播放與連續歌曲清單 | 🎙️ 環境聽歌識曲與歐美跨區分頁搜尋 |
| :---: | :---: |
| ![播放器與同步歌詞](./screenshots/player-lyrics.png) | ![環境聽歌識曲與跨平台搜尋](./screenshots/recognize-search.png) |
| *支援本地音訊與 YouTube 完整版混搭播放，固定高度歌詞同步捲動* | *純淨收音波形、分貝計、雙引擎辨識與分頁搜尋* |

| 🌐 AI 雙語同步歌詞與大字模式 | 🎨 四國語言、6 款主題與自訂背景設定 |
| :---: | :---: |
| ![AI 雙語同步歌詞](./screenshots/bilingual-fullscreen.png) | ![主題與背景設定](./screenshots/themes-settings.png) |
| *依介面語系自動翻譯並同步捲動，支援全螢幕大字檢視* | *支援四語系切換、炫光粉／寶寶藍／星空藍等主題與背景濃淡調整* |

---

## 📖 專案簡介

**SonicAura** 是一款純前端、零外部 CDN 依賴的漸進式網頁應用程式（PWA）音樂播放器。它整合了**YouTube 完整播放與歌詞同步**、**環境背景音樂辨識（聽歌識曲）**、**歐美與全球跨區分頁搜尋**、**五大串流平台快速跳轉**、**連續歌曲循環播放清單**以及**AI 雙語同步歌詞**，並內建**四國介面語言**與高度客製化的主題色彩及背景圖片設定。

### ✨ 核心功能

* **🎬 YouTube 完整播放 + 歌詞同步**：免 API Key！直接貼上 YouTube / YouTube Music 連結或 11 碼影片 ID，即可透過官方 IFrame Player API 播放完整歌曲，自動抓取歌名、歌手與高畫質封面，並即時驅動 LRCLIB 完整曲長同步歌詞、進度條、點擊歌詞跳轉與雙語翻譯。
* **🎵 播放器與精巧同步歌詞合一**：將播放控制與固定高度（僅容器內部捲動）的同步歌詞整合於同一張毛玻璃卡片中；播放器與歌詞區右上角皆配置**放大版「＋ 匯入本地音訊 / .lrc」與「🔍 搜尋歌詞」按鈕**，支援偏移微調（`-0.5s / -0.1s / +0.1s / +0.5s`）、一鍵對齊目前句與全螢幕大字模式。
* **🔁 連續歌曲清單 & 📂 歷史加入歌曲**：
  * **連續歌曲清單**：支援將本機 MP3、示範曲與 **YouTube 完整版** 混搭加入專屬播放佇列，提供「**▶ 開始連續播放**」依序循環不斷播放、單曲順序上下調整（`↑ / ↓`）、移除、清空，以及直接拖放音訊檔加入。
  * **歷史加入歌曲**：完整記錄所有匯入、YouTube 與試聽曲目，自動清洗檔名雜訊並智慧拆解「歌手 - 歌名」，每首皆可一鍵「**＋ 加入連續**」或「**＋ 全部加入**」。
* **🌐 四國介面語言 & AI 聯動歌詞翻譯**：內建 **繁體中文、简体中文、English、日本語** 四種介面語系即時切換；AI 同步歌詞翻譯會自動跟隨目前介面語系進行逐行翻譯並獨立快取。
* **🎙️ 環境背景音樂辨識**：採用關閉語音降噪與回音消除的純淨收音管線，內建即時頻譜、分貝計與錄音重聽功能，支援 **AudD 聲紋比對** 與 **Gemini AI 聽寫反查** 雙引擎。
* **🌍 歐美跨區擴充搜尋（含分頁瀏覽）與五大平台直達**：整合 iTunes 跨區（美、英、德、法、瑞、台、日）單區最多 50 筆、歐美跨區最多 75 筆去重搜尋，提供**上一頁／下一頁**分頁導覽與 `🎬 YT` 快捷跳轉，並可一鍵另開或批次開啟 **YouTube、YouTube Music、Apple Music、Spotify、KKBOX**。
* **🎨 外觀與背景自訂**：提供 **極致黑、炫光粉、烈焰橘、寶寶藍、星空藍、魔幻紫** 6 款主題，並可匯入自訂背景圖片，自由調整圖片濃淡度（0%～100%）與模糊度（0px～20px）。

---

## 🚀 使用方法

### 1. 使用「🎬 YouTube 完整播放」搭配同步歌詞
1. 複製任意 **YouTube / YouTube Music 網址**或 11 碼影片 ID，貼入播放器內的 `🎬` 輸入框並點擊 **「載入完整版」**。
2. 系統會自動帶入歌名、歌手與封面並展開內嵌視訊區開始播放。
3. 點擊歌詞區右上角 **「🔍 搜尋歌詞」**，LRCLIB 會自動依完整曲長優先列出最吻合的同步時間軸版本；套用後即可點擊歌詞跳轉影片進度、一鍵對齊或開啟 AI 雙語翻譯。

### 2. 匯入本地音樂與使用「🔁 連續歌曲清單」
1. 點擊播放器右上角 **「＋ 匯入本地音訊 / .lrc」**，或直接將電腦中的多首音樂檔拖放至下方 **「📂 歷史加入歌曲」** 或 **「🔁 連續歌曲清單」**。
2. 在「歷史加入歌曲」點擊 **「＋ 加入連續」**（或 **「＋ 全部加入」**），即可將本機音訊與 YouTube 完整曲目混搭排序。
3. 使用 `↑ / ↓` 調整順序後點擊 **「▶ 開始連續播放」**，播放器會顯示 **「連續播放中」** 徽章並依序循環不斷播放。

### 3. 環境聽歌識曲與歐美分頁搜尋
* 切換至 **「🎙️ 環境聽歌識曲 & 跨平台搜尋」** 分頁：
  * 點擊中央麥克風進行 8 / 10 / 15 秒純淨收音（需於 `HTTPS` 網址如 GitHub Pages 下使用），辨識後可直接試聽比對或微調聽寫歌詞重查。
  * 在「歐美與全球音樂搜尋」輸入關鍵字，可透過底部 **「◀ 上一頁 / 下一頁 ▶」** 瀏覽更多曲目，或點 `🎬 YT` 快速前往 YouTube 尋找完整版連結貼回播放器。

### 4. 切換多國語言、主題、背景與 API 設定
* 點擊畫面最右上方的 **⚙️ 齒輪圖示** 開啟程式設定：
  * **介面語言**：即時切換 繁體中文 / 简体中文 / English / 日本語。
  * **主題與背景**：切換 6 款主題色票、匯入背景圖並調整濃淡與模糊度。
  * **AudD / Gemini API**：選填個人 API 金鑰（僅保存於本機瀏覽器 `localStorage`，絕不上傳至伺服器）。

### 5. 安裝為手機／電腦 App（PWA）
* 使用 Chrome 或 Edge 開啟 GitHub Pages 網址，點擊瀏覽器選單中的 **「安裝應用程式」** 或 **「加到主畫面」**，即可享受全螢幕原生般體驗。

---

## 🌐 English Version

### 📖 Introduction

**SonicAura** is a lightweight, zero-CDN Progressive Web App (PWA) music player built entirely with vanilla HTML, CSS, and JavaScript. It combines **YouTube full-length playback with synced lyrics**, **ambient music recognition**, **paginated multi-region music discovery (US/UK/EU & Global)**, **cross-platform streaming shortcuts**, a **continuous sequential playlist**, **AI-powered bilingual synced lyrics**, and **4-language UI support** inside a customizable glassmorphism interface.

### ✨ Key Features

* **🎬 YouTube Full Playback + Synced Lyrics**: No API key required! Paste any YouTube / YouTube Music URL or 11-character video ID to play full-length tracks via the official IFrame Player API, automatically fetching title/artist metadata and syncing in real time with LRCLIB lyrics, click-to-seek, timing offset, and AI translation.
* **🎵 Unified Player & Compact Synced Lyrics**: Playback controls and a fixed-height, container-scoped scrollable lyrics pane live inside one seamless card. Features enlarged top-right **"＋ Import Audio / .lrc"** and **"🔍 Search Lyrics"** quick-action buttons, offset adjustments (`-0.5s / -0.1s / +0.1s / +0.5s`), one-click line alignment, and fullscreen lyrics mode.
* **🔁 Continuous Playlist & 📂 Added Songs History**:
  * **Continuous Playlist**: Mix local audio files, demo tracks, and YouTube full tracks into a looping sequential queue. Supports **"▶ Play Queue"**, **"＋ Add All"**, up/down reordering (`↑ / ↓`), item removal, clearing, and direct drag-and-drop audio import.
  * **Added Songs History**: Tracks all imported, YouTube, and preview songs with automatic filename cleanup (`Artist - Title`) and one-click **"＋ Queue"** buttons.
* **🌐 4-Language UI & Context-Aware AI Lyrics Translation**: Switch instantly between **Traditional Chinese (繁體中文), Simplified Chinese (简体中文), English, and Japanese (日本語)**. AI lyric translation automatically adapts to your chosen UI language and caches results per language.
* **🎙️ Ambient Music Recognition**: Captures clean audio with browser voice processing disabled (`echoCancellation`, `noiseSuppression`, and `autoGainControl` turned off). Includes a real-time spectrum visualizer, dB meter, clip replay, and a dual-engine pipeline (**AudD** audio fingerprinting + **Gemini AI** transcription & **LRCLIB** lookup).
* **🌍 Paginated Multi-Region Search & Cross-Platform Hub**: Search up to 50 tracks per region (or 75 deduplicated tracks across US/GB/DE) via iTunes Search API with **Prev / Next pagination**, quick `🎬 YT` shortcuts, and one-click or batch launching for **YouTube, YouTube Music, Apple Music, Spotify, and KKBOX**.
* **🎨 Themes & Custom Background**: Switch between 6 built-in themes (**Obsidian Dark, Neon Pink, Flame Orange, Baby Blue, Starry Blue, Magic Purple**) and upload a custom wallpaper with adjustable opacity (0–100%) and blur (0–20px).

### 🚀 How to Use

1. **YouTube Full Playback & Synced Lyrics**: Paste any YouTube / YouTube Music link or video ID into the `🎬` input bar and click **"Load Full"**. Then click **"🔍 Search Lyrics"** to pick duration-matched synced lyrics from LRCLIB.
2. **Local Files & Continuous Queue**: Click **"＋ Import Audio / .lrc"** (or drag & drop files). Click **"＋ Queue"** in **Added Songs History** to mix local tracks and YouTube songs into **Continuous Playlist**, reorder with `↑ / ↓`, and press **"▶ Play Queue"**.
3. **Recognize & Paginated Search**: Switch to **Recognize & Search** to identify ambient music via microphone *(requires `HTTPS`)*, browse multi-page iTunes results with **◀ Prev / Next ▶**, or jump to streaming platforms.
4. **Settings & PWA**: Click the top-right **⚙️ Gear icon** to switch between 4 languages, 6 themes, custom wallpaper sliders, and optional API tokens. Open your GitHub Pages URL in Chrome or Edge and choose **"Install App"** to install as a PWA.

---

## 📄 License

This project is licensed under the [MIT License](./LICENSE).