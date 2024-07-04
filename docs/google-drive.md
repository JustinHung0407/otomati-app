# Google Drive API

我們透過 Google Drive API 來存取 Google Drive 上的檔案。
並進一步透過 LangChain 的 pipe 達到 load document 與 retrieval 的功能。

設定步驟請參考 [建立 Google API 服務帳戶憑證教學](https://notes.fism.app/Area/Company/Google/Google+API+%26+Services/%E5%BB%BA%E7%AB%8B+Google+API+%E6%9C%8D%E5%8B%99%E5%B8%B3%E6%88%B6%E6%86%91%E8%AD%89%E6%95%99%E5%AD%B8)

## SCOPES

Google Drive API 有許多不同的 SCOPES，用途為控制應用程式對 Google Drive 的存取權限，請根據需求選擇適合的 SCOPES。

請參考：
- [選擇 Google Drive API 範圍](https://developers.google.com/drive/api/guides/api-specific-auth?hl=zh-tw)
- 常用 SCOPES：
  - `https://www.googleapis.com/auth/drive.file`
  - `https://www.googleapis.com/auth/drive.metadata.readonly`
  - `https://www.googleapis.com/auth/drive.readonly`


## 參考資料
- [Google Drive API](https://developers.google.com/drive/api/v3/about-sdk)
- [Using OAuth 2.0 for Installed Applications](https://github.com/googleapis/google-api-python-client/blob/main/docs/oauth-installed.md)
- [選擇 Google Drive API 範圍](https://developers.google.com/drive/api/guides/choosing-auth?hl=zh-tw)