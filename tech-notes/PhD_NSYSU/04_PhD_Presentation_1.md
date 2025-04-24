from pptx.util import Inches, Pt
from pptx.enum.shapes import MSO_SHAPE
from pptx.dml.color import RGBColor

# 建立簡報

prs = Presentation()

# 1. 封面

slide1 = prs.slides.add_slide(prs.slide_layouts[0])
slide1.shapes.title.text = "博士班面試簡報"
slide1.placeholders[1].text = "洪希仁 / MAC-RAG 研究計劃簡介"

# 2. 自我介紹

slide2 = prs.slides.add_slide(prs.slide_layouts[1])
slide2.shapes.title.text = "自我介紹"
slide2.placeholders[1].text = (
"• 現任：薈智創新科技 執行長\n"
"• 經歷：Thales 創新總監 / Volvo 資深經理 / Accenture 顧問\n"
"• 專長：LLM, RAG, AutoML, 智慧製造與預測性維護\n"
"• 願景：融合產業實戰與學術研究，打造下一代智慧決策系統"
)

# 3. 研究動機與背景

slide3 = prs.slides.add_slide(prs.slide_layouts[1])
slide3.shapes.title.text = "研究動機與背景"
slide3.placeholders[1].text = (
"• 傳統 RAG 無法解決工業決策的三大問題：\n"
" - 缺乏反思修正能力\n"
" - 難以處理多模態資料（如 PDF/感測數據）\n"
" - 無法主動規劃任務與多步推理\n"
"• 我希望打造 MAC-RAG 系統作為突破方案"
)

# 4. MAC-RAG 架構總覽

slide4 = prs.slides.add_slide(prs.slide_layouts[1])
slide4.shapes.title.text = "MAC-RAG 系統架構總覽"
slide4.placeholders[1].text = (
"MAC-RAG = Multi-modal + Agentic + Corrective RAG\n\n"
"• CRAG：錯誤檢測與修正\n"
"• KAG：知識導向生成（Knowledge-Augmented Generation）\n"
"• Agent：任務規劃、工具調用、反思與記憶管理\n"
"• 多模態融合：時序、PDF、表格與自然語言"
)

# 5. 年度規劃

slide5 = prs.slides.add_slide(prs.slide_layouts[1])
slide5.shapes.title.text = "三年研究規劃"
slide5.placeholders[1].text = (
"Year 1: 強化 CRAG 與 KAG 結構 + 任務導向評估器\n"
"Year 2: 建立 Agentic 流程控制 + 任務規劃模組\n"
"Year 3: 多模態資料整合 + 智慧工廠應用場景驗證"
)

# 6. 應用場景與驗證計畫

slide6 = prs.slides.add_slide(prs.slide_layouts[1])
slide6.shapes.title.text = "應用場景與驗證計畫"
slide6.placeholders[1].text = (
"• PdM 預測性維護：結合感測數據 + 維修紀錄\n"
"• PDF 文件審查與報告生成：複雜結構理解\n"
"• 多模態交接班助手：壓縮機／泵浦狀態總結與建議\n"
"• 合規性建議產出：圖表 + 準則 + 關鍵詞搜尋"
)

# 7. Related Work

slide7 = prs.slides.add_slide(prs.slide_layouts[1])
slide7.shapes.title.text = "Related Work 對比"
slide7.placeholders[1].text = (
"• RAG: 檢索＋生成，不含反思與模態處理\n"
"• CRAG: 加入反思但無 Agent 能力\n"
"• ReAct: 可用工具但缺乏知識結構與回饋\n"
"• MAC-RAG: 三層融合 + 工業應用為導向的整合型架構"
)

# 8. 個人優勢與動機

slide8 = prs.slides.add_slide(prs.slide_layouts[1])
slide8.shapes.title.text = "Why Me？"
slide8.placeholders[1].text = (
"• 擁有完整產業落地經驗與跨國視野\n"
"• 熟悉 LLM / RAG / AutoML / MCP\n"
"• 已完成 PetroGPT / MiniGPT 實驗與開源經驗\n"
"• 願以博士研究整合實戰，回饋學術與中山系所"
)

# 9. Q&A 預備

slide9 = prs.slides.add_slide(prs.slide_layouts[1])
slide9.shapes.title.text = "常見問題與回應（FAQ）"
slide9.placeholders[1].text = (
"Q: 您年紀偏大，還能完成研究嗎？\n"
"A: 我的時間規劃與體力管理反而更成熟穩定，已有實證成果佐證。\n\n"
"Q: 工作與博士如何兼顧？\n"
"A: 公司已轉為技術顧問模式，博士研究與公司創新策略一致，可互相促進。"
)

# 10. 結語與展望

slide10 = prs.slides.add_slide(prs.slide_layouts[1])
slide10.shapes.title.text = "結語與展望"
slide10.placeholders[1].text = (
"MAC-RAG 是我希望留給中山與台灣 AI 社群的一個創新典範。\n"
"我願以三年時間，投入推動台灣智慧製造與多模態決策 AI 的學術突破與應用落地。"
)

# 儲存簡報

ppt*path = "/mnt/data/博士面試簡報*洪希仁\_MAC-RAG 研究提案.pptx"
prs.save(ppt_path)

ppt_path
