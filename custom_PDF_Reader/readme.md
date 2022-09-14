# 一種基於ML和Tesseract框架的PDF提取文字方式
### 動機
- 現有PDF套件在讀取文字上，無法對圖片中的文字進一步地做提取
- PDF每一頁的文字分布，能夠讓人知道要如何按順序閱讀段落
### 方法
- 使用Tesseract先獲取每個字母的位置
- 利用DBscan來對位置進行cluster形成paragraph
- 輸出資料除了有圖片中的文本資訊外，也有paragraph的相對位置
- 未來: 我們可以再利用其他ML/DL方法，讓模型判斷這頁PDF文本，是要做橫式還是直式來進行閱讀
### 方法圖示
![image](https://github.com/B0544218/Introduction_resume/blob/main/custom_PDF_Reader/figure1.JPG)
![image](https://github.com/B0544218/Introduction_resume/blob/main/custom_PDF_Reader/figure2.JPG)
![image](https://github.com/B0544218/Introduction_resume/blob/main/custom_PDF_Reader/figure3.JPG)
![image](https://github.com/B0544218/Introduction_resume/blob/main/custom_PDF_Reader/figure4.JPG)
![image](https://github.com/B0544218/Introduction_resume/blob/main/custom_PDF_Reader/figure5.JPG)
![image](https://github.com/B0544218/Introduction_resume/blob/main/custom_PDF_Reader/figure6.JPG)

