# 🔬 國中自然科理化 互動語音解題動畫・數位學習題庫系統

本專案位於 `G:\AI測試\PageCrypt_網頁加密與GitHub託管專案`，已全面升級為**模組化多單元數位學習門戶**。
所有教材皆採用 **PageCrypt（AES-256-GCM 高強度加密演算法）** 保護，兼具版權安全、快速載入與清楚的差異化網址結構。

---

## 🌐 線上學習大廳與各單元專屬網址清單

* 🚪 **題庫首頁大廳**：**[https://chenhan12345.github.io/science-quiz/](https://chenhan12345.github.io/science-quiz/)**
* 🔑 **全站統一通關密碼**：`chenhan`
* 📦 **GitHub 儲存庫**：[https://github.com/chenhan12345/science-quiz](https://github.com/chenhan12345/science-quiz)

---

### 📋 完整 12 單元差異化網址對照表

| 版本 / 類別 | 回數 / 章節 | 單元教材名稱 | 專屬短網址 (Slug) | 主題標籤 |
| :--- | :--- | :--- | :--- | :--- |
| **南一版** | 第 6 回 | §3-1～§3-2 波動與聲音的世界 | [`/nani-ch3-waves.html`](https://chenhan12345.github.io/science-quiz/nani-ch3-waves.html) | 🌊 波速、縱波橫波、介質聲速 |
| **金安版** | 第 5 回 | §3-1～§3-2 波的傳播與聲音 | [`/jinan-ch3-waves.html`](https://chenhan12345.github.io/science-quiz/jinan-ch3-waves.html) | 🔊 週期波、振幅波長、聲音傳播 |
| **金安版** | 第 6 回 | §3-3～§3-4 回聲與多變的聲音 | [`/jinan-ch3-echo.html`](https://chenhan12345.github.io/science-quiz/jinan-ch3-echo.html) | ⛰️ 回聲測距、響度/音調/音色 |
| **金安版** | 第 7 回 | §4-1～§4-2 光的直線傳播與反射 | [`/jinan-ch4-light.html`](https://chenhan12345.github.io/science-quiz/jinan-ch4-light.html) | 💡 針孔成像、平面鏡虛像、反射定律 |
| **金安版** | 第 8 回 | §4-3～§4-5 光的折射與光學色光 | [`/jinan-ch4-refraction.html`](https://chenhan12345.github.io/science-quiz/jinan-ch4-refraction.html) | 🌈 透鏡成像作圖、顯微鏡、色光三原色 |
| **隨堂小考** | 第 4 章 | 4-1～4-2 光的傳播與面鏡成像 | [`/quiz-4-1-mirrors.html`](https://chenhan12345.github.io/science-quiz/quiz-4-1-mirrors.html) | 🪞 面鏡成像規律、光傳播實驗 |
| **隨堂小考** | 第 4 章 | 4-3 光的折射與透鏡 | [`/quiz-4-3-lens.html`](https://chenhan12345.github.io/science-quiz/quiz-4-3-lens.html) | 🔍 凸透鏡與凹透鏡焦距像距 |
| **隨堂小考** | 第 4 章 | 4-4～4-5 光學儀器與光色 | [`/quiz-4-4-optical.html`](https://chenhan12345.github.io/science-quiz/quiz-4-4-optical.html) | 🔬 複式顯微鏡、視力矯正、色光過濾 |
| **隨堂小考** | 第 5 章 | 5-1 溫度與溫度計 | [`/quiz-5-1-temperature.html`](https://chenhan12345.github.io/science-quiz/quiz-5-1-temperature.html) | 🌡️ 溫標換算、液體熱膨脹原理 |
| **隨堂小考** | 第 5 章 | 5-2 熱量與比熱 | [`/quiz-5-2-heat-capacity.html`](https://chenhan12345.github.io/science-quiz/quiz-5-2-heat-capacity.html) | 🔥 H=m·s·ΔT 計算、熱平衡與比熱曲線 |
| **隨堂小考** | 第 5 章 | 5-3 熱對物質影響 ＆ 5-4 熱傳播 | [`/quiz-5-3-heat-transfer.html`](https://chenhan12345.github.io/science-quiz/quiz-5-3-heat-transfer.html) | ☀️ 三態變化、傳導對流輻射實例 |
| **隨堂小考** | 第 6 章 | 6-1～6-2 元素與純物質 | [`/quiz-6-1-matter.html`](https://chenhan12345.github.io/science-quiz/quiz-6-1-matter.html) | 🧪 元素符號、金屬與非金屬特性 |

---

## 🛠️ 未來如何新增、更新並自動發布教材？

專案內建自動化管線，未來只要按照以下 2 步，就能輕鬆更新全站：

### 步驟 1：在 [`quiz_catalog.json`](file:///G:/AI%E6%B8%AC%E8%A9%A6/PageCrypt_%E7%B6%B2%E9%A0%81%E5%8A%A0%E5%AF%86%E8%88%87GitHub%E8%A8%97%E7%AE%A1%E5%B0%88%E6%A1%88/quiz_catalog.json) 新增單元
在清單陣列中加入新單元的設定，例如：
```json
{
  "id": "quiz-7-1",
  "slug": "quiz-7-1-chem.html",
  "version": "隨堂小考",
  "version_tag": "quiz",
  "badge_color": "#8b5cf6",
  "chapter": "ch7",
  "chapter_name": "第7章 化學反應",
  "round": "隨堂測驗",
  "title": "隨堂小考：7-1 化學反應式與質量守恆",
  "scope": "反應物生成物平衡、質量守恆定律計算",
  "icon": "⚗️",
  "src_path": "G:\\AI公文\\您的新檔案.html"
}
```

### 步驟 2：執行自動建置與推送指令
開啟 PowerShell 終端機，執行以下指令：
```powershell
# 1. 自動加密所有檔案並更新首頁導覽大廳
python G:\AI測試\PageCrypt_網頁加密與GitHub託管專案\build_system.py

# 2. 一秒推送到 GitHub Pages 上線！
python G:\AI測試\PageCrypt_網頁加密與GitHub託管專案\upload_to_github.py
```
執行完畢後，新單元就會自動出現在學習大廳首頁，且專屬短網址即刻生效！
