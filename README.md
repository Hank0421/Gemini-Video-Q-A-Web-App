# Gemini AI Video Q&A System

## Introduction

This project is a web application based on Flask and Google Gemini API, allowing users to upload video files and interact with AI for video content Q&A.  
The frontend uses HTML, CSS, and JavaScript (jQuery), while the backend is implemented with Python Flask and integrates Gemini generative AI services.

## Features

- Upload video files (supports mp4, mov, avi, webm, wmv, 3gp, flv, mpg, mpeg formats)
- Automatically upload videos to Gemini for processing
- After processing, interact with AI about the video content
- Supports Traditional Chinese interaction

## Installation & Usage

1. **Install dependencies**

   ```sh
   pip install -r requirements.txt
   ```

2. **Set API Key**

   - Edit `config.ini` and set your Google Gemini API key under the `[Gemini]` section.

3. **Start the server**

   ```sh
   flask run --port=5001
   ```

   Or use the VS Code debugger.

4. **How to use**

   - Open [http://127.0.0.1:5001/](http://127.0.0.1:5001/) in your browser.
   - Upload a video file. After processing, you can chat with the AI about the video.

## Project Structure

```
app.py
config.ini
requirements.txt
static/
    css/
        style.css
    data/
        # uploaded video files
    js/
        main.js
templates/
    index.html
.vscode/
    launch.json
```

## Notes

- Make sure the `static/data/` directory exists and is writable.
- Google Gemini API access is required for video upload and analysis.

# Gemini AI 影片問答系統

## 簡介

本專案是一個基於 Flask 與 Google Gemini API 的網頁應用，讓使用者可以上傳影片檔案，並與 AI 進行影片內容相關的問答互動。  
前端採用 HTML、CSS、JavaScript（jQuery），後端則以 Python Flask 實作，並整合 Gemini 生成式 AI 服務。

## 功能

- 上傳影片檔案（支援 mp4、mov、avi、webm、wmv、3gp、flv、mpg、mpeg 格式）
- 影片上傳後自動傳送至 Gemini 處理
- 影片處理完成後，可與 AI 進行影片內容相關的對話
- 支援繁體中文互動

## 安裝與執行

1. **安裝相依套件**

   ```sh
   pip install -r requirements.txt
   ```

2. **設定 API 金鑰**

   - 編輯 `config.ini`，將 `[Gemini]` 區塊下的 `API_KEY` 設為你的 Google Gemini API 金鑰。

3. **啟動伺服器**

   ```sh
   flask run --port=5001
   ```

   或使用 VS Code 的偵錯工具啟動。

4. **使用方式**

   - 於瀏覽器開啟 [http://127.0.0.1:5001/](http://127.0.0.1:5001/)
   - 上傳影片檔案，待處理完成後即可與 AI 互動。

## 專案結構

```
app.py
config.ini
requirements.txt
static/
    css/
        style.css
    data/
        # 上傳的影片檔案
    js/
        main.js
templates/
    index.html
.vscode/
    launch.json
```

## 注意事項

- 請確保 `static/data/` 目錄存在且有寫入權限。
- Google Gemini API 需有權限上傳與分析影片檔案。

