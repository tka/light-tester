# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 專案概述

崁燈洗牆效果模擬器 - 使用 Three.js 模擬室內崁燈的洗牆照明效果，可調整光束角度、傾斜角度、離牆距離等參數。

## 技術架構

- **無建置工具**：純 HTML 單頁應用，透過 CDN 載入所有相依套件
- **React 18**：透過 Babel Standalone 在瀏覽器端編譯 JSX
- **Three.js r128**：3D 場景渲染（使用舊版以相容 OrbitControls 全域附加方式）
- **Tailwind CSS**：透過 CDN 載入樣式

## 執行方式

直接用瀏覽器開啟 `index.html` 或使用任意靜態伺服器：

```bash
npx serve .
# 或
python -m http.server 8000
```

## 檔案結構

- `index.html` - 主要應用程式，包含完整的 React 元件與 Three.js 場景
- `remixed-e8403d6f.tsx` - 備用/匯出版本的 React 元件（使用 ES module import）

## 程式碼慣例

- 使用 arrow function 定義函式
- 不使用 React.FC 型別定義
- 以台灣中文撰寫 UI 與註解
