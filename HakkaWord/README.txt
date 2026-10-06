客語句子學習 v2.0（GitHub Pages）

檔案：
- index.html：主學習網站
- data.json：目前 20 筆公開客語短句與來源資訊
- about.html：資料來源、授權、AI 發音、隱私與準確度說明
- LICENSE_SITE_CODE.txt：本站自行程式碼 MIT 授權範圍

部署：
把四個檔案放到 GitHub repository 根目錄並啟用 GitHub Pages 即可。
網站是純前端，不需要自己的伺服器。

TTS：
- 使用者按「取得拼音／發音」時才呼叫 ivanusto/tw-hakka-tts。
- 目前固定模型 yourtts-htia-240704。
- FormoSpeech 模型為非商業授權，因此本網站含 TTS 時應維持非商業用途。
- 如果第三方 TTS 暫停，文字學習功能仍可使用。

擴充資料：
只需新增 data.json 的 items：
{
  "id": 21,
  "dialect": "sixian",
  "dialectLabel": "四縣",
  "text": "...",
  "sourcePerson": "...",
  "sourceType": "...",
  "sourceUrl": "..."
}

重要：
目前 v2.0 內建 20 筆句子，不是完整語料庫。
若要大規模擴充，應優先從已確認可再利用的政府開放資料集匯入，
不要直接抓取授權不明或另有限制的教材。
