# PDF 轉 JPG 工具（Streamlit）

這是一個可直接放到 GitHub，並部署到 Streamlit Community Cloud 的 PDF 轉 JPG 小工具。

## 功能

- 支援上傳多個 PDF
- 每一頁轉成 JPG
- 可調整輸出清晰度
- 可下載全部 ZIP
- 可預覽並下載單頁 JPG
- 不需要安裝 Poppler，較適合部署到 Streamlit

## 專案結構

```text
pdf_to_jpg_streamlit/
├─ app.py
├─ requirements.txt
├─ README.md
└─ .streamlit/
   └─ config.toml
```

## 本機執行

```bash
pip install -r requirements.txt
streamlit run app.py
```

## 部署到 GitHub + Streamlit Community Cloud

1. 新增一個 GitHub repository
2. 把這些檔案上傳到 repo 根目錄
3. 到 Streamlit Community Cloud 建立新 app
4. 選你的 GitHub repo
5. Main file path 填入 `app.py`
6. Deploy

## 注意事項

- 如果你要上傳比較大的 PDF，可調整 `.streamlit/config.toml`
- 建議 Python 版本使用 3.11 或 3.12
