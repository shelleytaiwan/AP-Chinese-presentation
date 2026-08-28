# AP 中文演說 AI 教練

本專案以 GitHub 保存原始碼，以 Vercel 執行網站與 `/api/ap-chinese-coach` Serverless Function。

## 部署
1. 將這個資料夾內的全部檔案上傳到 GitHub repository。
2. 在 Vercel Import Git Repository，選擇該 GitHub repository。
3. 在 Vercel → Project Settings → Environment Variables 新增：
   - `OPENAI_API_KEY` = 你的 OpenAI API Key
   - `OPENAI_MODEL` = `gpt-5.6-luna`（可省略，預設就是這個）
4. Redeploy。
5. 學生使用 Vercel 產生的正式網址。GitHub 是程式碼來源；不要用 GitHub Pages 作為正式網址，因為 GitHub Pages 不能執行後端 API。

不要把 OpenAI API Key 寫進 index.html，也不要提交 `.env`。
