《个性化词云生成系统》软件开发文档\
软件开发：Duan Shoujian
2024年2月

一、系统概述
  该系统可以将任意长度的文本文档生成个性化的词云。用户可以方便地进行设置词云样式，包括词云尺寸、背景颜色、最多词语数、缩放比例。系统可以导入背景图，生成个性化图形的词云，还可以查看词频，将词云图保存为Jpg、Png格式以供其他场景使用。系统提供了将Word文档、Pdf文档、PowerPoint文档、Excel表格转换成文本文档的功能。系统界面友好、简洁易用，用户只需点击鼠标即可轻松生成个性化词云，经多次测试，系统状态稳定、安全可靠。

二、开发环境概述
  1．系统名称及版本：个性化词云生成系统 v1
  2．生成模式：单机模式\
  3．Python版本：Python 3.11
  4．开发环境：anaconda3+Pycharm 2022.2
  5. 程序运行环境：Win7、Win10、Win11

三、程序文件及功能
1. 主要文件和文件夹的功能说明
  文件夹或文件作用	作用
  /main.py	个性化词云生成主程序
  /resource	存放系统所需资源，包括背景图片、示例文本、词云、字体等文件 
  /resource/Mask	存放常用背景图片
  /resource/Text	存放示例文本
  /resource/cy.ico	系统图标文件
  /resource/temp.png	保存生成的原始词云图
  /resource/temp2.png	保存生成的用于在系统中显示的缩小的词云图
  /resource/msyh.ttc	支持中文显示的字体
  /resource/user_dict.txt	保存用户自定义分词词典
  /resource/stop_words.txt	保存用户自定义停用词词典
  /resource/word_frequency.txt	保存按降序排列的词频信息
2. 调用的主要Python库及作用说明
库名及作用
tkinter：tkintere用于生成GUI界面及控件。
jieba:jiebae用于中文分词。
wordcloud:wordcloud用于生成词云。
imageio:imageio读取和写入图像。
collections:collections用于处理词频排序。
PIL:PIL用于图像格式转换。
os:os用于处理文件路径及文件生成、删除。
docx:python-docx用于处理Word文档到文本文档的转换。
pdfplumber:pdfplumbe用于处理Pdf文档到文本文档的转换。
python-pptx:python-pptx用于处理PPT文档档到文本文档的转换。
openpyxl:openpyxl用于处理Excel电子表格到文本文档的转换。

