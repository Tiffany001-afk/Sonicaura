<div align="center">

# 🎵 SonicAura

**環境辨識與多語歌詞同步音樂播放器 ｜ Ambient Music Recognition & Synced Lyrics Player**

[![License: MIT](https://img.shields.io/badge/License-MIT-7c5cff.svg?style=for-the-badge)](./LICENSE)
[![PWA Ready](https://img.shields.io/badge/PWA-Installable-00d2ff.svg?style=for-the-badge&logo=pwa&logoColor=white)](./manifest.json)
[![i18n](https://img.shields.io/badge/Languages-繁中%20|%20简中%20|%20EN%20|%20日本語-f59e0b.svg?style=for-the-badge)](#)
[![Zero CDN](https://img.shields.io/badge/Dependencies-Zero%20CDN-22c55e.svg?style=for-the-badge)](#)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-ff4da6.svg?style=for-the-badge&logo=github&logoColor=white)](https://YOUR_USERNAME.github.io/sonicaura/)

[繁體中文介紹](#-專案簡介) • [介面預覽](#-介面預覽--screenshots) • [使用方法](#-使用方法) • [English Version](#-english-version)

</div>

---

## 🖼️ 介面預覽 / Screenshots

| 🎵 整合式播放器與同步歌詞 | 🎙️ 環境聽歌識曲與歐美跨區搜尋 |
| :---: | :---: |
| ![播放器與同步歌詞](./screenshots/player-lyrics.png) | ![環境聽歌識曲與跨平台搜尋](./screenshots/recognize-search.png) |
| *播放器與固定高度同步歌詞合一，右上角提供放大版匯入與搜尋歌詞按鈕* | *純淨收音波形、分貝計、雙引擎辨識與五大平台直達* |

| 🌐 AI 雙語同步歌詞與大字模式 | 🎨 四國語言、6 款主題與自訂背景設定 |
| :---: | :---: |
| ![AI 雙語同步歌詞](./screenshots/bilingual-fullscreen.png) | ![主題與背景設定](./screenshots/themes-settings.png) |
| *依介面語系自動翻譯並同步捲動，支援全螢幕大字檢視* | *支援四語系切換、炫光粉／寶寶藍／星空藍等主題與背景濃淡調整* |

---

## 📖 專案簡介

**SonicAura** 是一款純前端、零外部 CDN 依賴的漸進式網頁應用程式（PWA）音樂播放器。它整合了**環境背景音樂辨識（聽歌識曲）**、**歐美與全球跨區音樂搜尋**、**五大串流平台快速跳轉**以及**AI 雙語同步歌詞播放**，並內建**四國介面語言**與高度客製化的主題色彩及背景圖片設定。

### ✨ 核心功能
* **播放器與精巧同步歌詞合一**：將播放控制與固定高度（僅容器內部捲動）的同步歌詞整合於同一張毛玻璃卡片中；播放器與歌詞區右上角皆配置**放大版「＋ 匯入本地音訊 / .lrc」與「🔍 搜尋歌詞」按鈕**，並支援點擊歌詞跳轉、偏移微調（`-0.5s / -0.1s / +0.1s / +0.5s`）、一鍵對齊目前句與全螢幕大字模式。
* **🌐 四國介面語言 & AI 聯動歌詞翻譯**：內建 **繁體中文、简体中文、English、日本語** 四種介面語系即時切換；AI 同步歌詞翻譯會自動跟隨目前介面語系進行逐行翻譯並獨立快取。
* **🎙️ 環境背景音樂辨識**：採用關閉語音降噪與回音消除的純淨收音管線，內建即時頻譜、分貝計與錄音重聽功能，支援 **AudD 聲紋比對** 與 **Gemini AI 聽寫反查** 雙引擎。
* **🌍 歐美跨區搜尋與五大平台直達**：整合 iTunes 跨區（美、英、德、法、瑞、台、日）官方 30 秒試聽，並可一鍵另開或批次開啟 **YouTube、YouTube Music、Apple Music、Spotify、KKBOX** 搜尋頁面。
* **📂 本地匯入與開箱即播**：內建 3 首離線合成示範曲（英／日／中），支援拖放匯入本機音訊（MP3 / WAV / M4A / OGG / FLAC）與 `.lrc` 歌詞檔，自動清洗檔名雜訊並搭配 LRCLIB 時長比對搜尋歌詞。
* **🎨 外觀與背景自訂**：提供 **極致黑、炫光粉、烈焰橘、寶寶藍、星空藍、魔幻紫** 6 款主題，並可匯入自訂背景圖片，自由調整圖片濃淡度（0%～100%）與模糊度（0px～20px）。

---

## 🚀 使用方法

### 1. 開始播放、匯入音樂與同步歌詞
1. 開啟網頁即可直接播放內建示範曲，或點擊播放器右上角 **「＋ 匯入本地音訊 / .lrc」**（亦支援拖放至下方播放清單區）。
2. 若本地歌曲缺少歌詞，點擊歌詞區右上角 **「🔍 搜尋歌詞」**，系統會依歌曲時長從 LRCLIB 自動優先排序最吻合的同步版本供您套用。
3. 若發現歌詞快慢略有誤差，可使用下方偏移按鈕微調，或點選正在唱的那一句後按 **「📌 對齊目前時間」**。

### 2. 切換多國語言、主題與背景圖片
* 點擊畫面最右上方的 **⚙️ 齒輪圖示** 開啟程式設定：
  * **介面語言**：即時切換 繁體中文 / 简体中文 / English / 日本語，設定自動記憶於本機。
  * **主題與背景**：切換 6 款主題色票、匯入喜愛的背景圖片，並透過拉桿調整濃淡與模糊度。

### 3. 啟用 AI 歌詞翻譯與環境聽歌識曲
1. 在 **⚙️ 程式設定** 中填入您的 API 金鑰（僅安全保存於您本機瀏覽器的 `localStorage`，不會上傳至伺服器）：
   * **Gemini API Key**（可於 [Google AI Studio](https://aistudio.google.com/apikey) 免費取得）：啟用 AI 多語歌詞翻譯與 AI 環境音聽寫辨識。
   * **AudD API Token**（選填，可於 [AudD](https://audd.io/) 取得）：提供 Shazam 級聲紋比對，未填寫亦可開啟公開 `test` 測試模式。
2. 完成後即可點擊 **「🌐 翻譯中文」**（依語系自動顯示對應語言），或切換至 **「🎙️ 環境聽歌識曲 & 跨平台搜尋」** 分頁進行收音辨識（瀏覽器需在 `HTTPS` 網址下才會開放麥克風權限）。

### 4. 安裝為手機／電腦 App（PWA）
* 使用 Chrome 或 Edge 開啟 GitHub Pages 網址，點擊瀏覽器選單中的 **「安裝應用程式」** 或 **「加到主畫面」**，即可享受全螢幕原生般體驗。

---

## 🌐 English Version

### 📖 Introduction

**SonicAura** is a lightweight, zero-CDN Progressive Web App (PWA) music player built entirely with vanilla HTML, CSS, and JavaScript. It combines **ambient music recognition**, **multi-region music discovery (US/UK/EU & Global)**, **cross-platform streaming shortcuts**, **AI-powered bilingual synced lyrics**, and **4-language UI support** inside a customizable glassmorphism interface.

### ✨ Key Features
* **Unified Player & Compact Synced Lyrics**: Playback controls and a fixed-height, container-scoped scrollable lyrics pane live inside one seamless card. Features enlarged top-right **"＋ Import Audio / .lrc"** and **"🔍 Search Lyrics"** quick-action buttons, click-to-seek, timing offset controls (`-0.5s / -0.1s / +0.1s / +0.5s`), one-click line alignment, and fullscreen lyrics mode.
* **🌐 4-Language UI & Context-Aware AI Lyrics Translation**: Instantly switch the interface between **Traditional Chinese (繁體中文), Simplified Chinese (简体中文), English, and Japanese (日本語)**. AI lyric translation automatically adapts to your selected UI language and caches results per language.
* **🎙️ Ambient Music Recognition**: Captures clean audio with browser voice processing disabled (`echoCancellation`, `noiseSuppression`, and `autoGainControl` turned off). Includes a real-time spectrum visualizer, dB meter, clip replay, and a dual-engine pipeline (**AudD** audio fingerprinting + **Gemini AI** transcription & **LRCLIB** lookup).
* **🌍 Multi-Region Search & Cross-Platform Hub**: Search official 30-second previews across US, UK, DE, FR, SE, TW, and JP via iTunes Search API, and launch or batch-open search links on **YouTube, YouTube Music, Apple Music, Spotify, and KKBOX**.
* **📂 Local File Import & Offline Demos**: Ships with 3 offline Web Audio synthesized demos (EN/JP/ZH). Supports drag-and-drop import for local audio (`MP3 / WAV / M4A / OGG / FLAC`) and `.lrc` files with automatic filename cleanup and duration-matched LRCLIB search.
* **🎨 Themes & Custom Background**: Switch between 6 built-in themes (**Obsidian Dark, Neon Pink, Flame Orange, Baby Blue, Starry Blue, Magic Purple**) and upload a custom wallpaper with adjustable opacity (0–100%) and blur (0–20px).

### 🚀 How to Use
1. **Play, Import & Sync**: Play the built-in demos right away, or click the enlarged **"＋ Import Audio / .lrc"** button (or drag & drop files). Click **"🔍 Search Lyrics"** at the top-right of the lyrics pane to pick duration-matched synced lyrics from LRCLIB.
2. **Language & Appearance**: Click the top-right **⚙️ Gear icon** to switch between 4 interface languages, pick from 6 color themes, or upload a custom background image with opacity & blur sliders.
3. **AI Translation & Recognition**: In **⚙️ Settings**, configure your free **Gemini API Key** from [Google AI Studio](https://aistudio.google.com/apikey) *(stored locally in `localStorage`)* and optionally an [AudD](https://audd.io/) Token. Microphone recognition requires `HTTPS` (automatically provided by GitHub Pages).
4. **Install as PWA**: Open your deployed GitHub Pages URL in Chrome or Edge and select **"Install App"** or **"Add to Home Screen"**.

---

## 📄 License

This project is licensed under the [MIT License](./LICENSE).
