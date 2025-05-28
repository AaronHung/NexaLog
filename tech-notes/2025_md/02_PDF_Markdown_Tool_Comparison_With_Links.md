
# 工具比較概覽（含超連結）

| 工具       | 轉換精度與結構保留 | OCR能力 | 適用場景 |
|------------|--------------------|---------|----------|
| **Marker** | 轉換準確，支援標題、段落、程式碼、公式等結構。詳見 [Marker 專案](https://github.com/VikParuchuri/marker) | 內建OCR（支援Tesseract） | 適合技術書籍，開源可自架 |
| **MinerU** | 高保真轉換，支援LaTeX、表格結構化處理，參見 [MinerU](https://github.com/opendatalab/MinerU) | 支援84種語言OCR，自動判斷是否需啟用 | 適合學術文檔，表格與圖像保留完整 |
| **MarkItDown** | 轉換快速，輸出簡潔Markdown。來源 [MarkItDown](https://github.com/microsoft/markitdown) | 支援影像OCR，能搭配LLM生成圖像描述 | 適合LLM摘要任務的預處理 |
| **pdf2md** | 基於GPT-4 Vision，自動產出Markdown格式。參考 [pdf2md](https://github.com/zyocum/pdf2md1) | 高品質視覺OCR | 適合精緻格式轉換與圖像理解 |
