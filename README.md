# FinRepProcessor
上市企业年报文本计算套件（FinRepProcessor）： 

**1. CustSplitTxts.exe**

即定制化文本分词批处理工具。通过自定义主题词典，对数以千计的文本文件（UTF-8-BOM编码）实施过滤分词，导出结果。 

在Windows命令行下使用：_CustSplitTxt.exe -d [你的定制词典] [待处理文本文件目录]_

输出各个待处理的文本文件的分词结果，并保存为文本文件。

**2. CalcTxts.exe**

计算CustSplitTxts导出的分词结果，输出各企业年报的词频和TF-IDF值、汇总词频及TF-IDF值。

在Windows命令行下使用：_CalcTxts.exe [待处理分词文件所在目录]_

输入由CustSplitTxts产生的分词文本所在目录。输出对所有分词文件的文本计算结果，包括对应于各分词文件的词频和TF-IDF计算结果，以及汇总的词频和TF-IDF值。

**3. SplitTxts.exe**

功能与CustSplitTxts相同，但输入的是文件列表，而不是目录路径。

在Windows命令行下使用：_SplitTxts.exe [待分词文本文件列表]_

**4. CountWords.exe**

简单计算文本文件的字数（中文：按字计算；英文：按字母计算，不计入空格）。

在Windows命令行下使用：_CountWords.exe [待计算文本文件目录]_
