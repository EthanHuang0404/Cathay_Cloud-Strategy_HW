這個為作業二的答案，我一次把兩個方案都實現出來，過程中皆有使用 chatgpt 進行協助生成程式碼，程式碼檔案為「國泰_雲端架構工程師實習生_作業.ipynb」。


1. 將新聞稿以爬蟲方式抓取內文，並存為 txt 檔
使用 BeautifulSoup 套件從 https://www.ithome.com.tw/news/152373 上將新聞內文爬下來，並存成 news_article.txt。

2. 將新聞稿的內文輸入給 ChatGPT API，並請 ChatGPT 總結新聞稿內容
透過 OpenAI 官方網站上（ https://platform.openai.com/docs/api-reference/chat/create ） 的 Create chat completion API 進行新聞內容透過 ’gpt-3.5-turbo’ 模型進行摘要的生成，並將結果存成 news_summary.txt。其中將 temperature 設定為 0.7 來控制生成文本的隨機性，max_tokens 設定為 1000, 來指定生成的文本最大長度 top_p 設定為 1 來控制生成過程中的token選擇範圍。

下圖為api使用證明。
<img width="1224" alt="image" src="https://github.com/EthanHuang0404/Cathay_Cloud-Strategy_HW/assets/52795694/285d73a5-99cd-415a-a391-be90ad54dd7e">
