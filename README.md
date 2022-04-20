# doc_similiarty


## Similarity method compare
1. levenshtein & normalized_levenshtein
2. LongestCommonSubsequence & metric_lcs
3. Jaccard coefficient
4. Dice coefficient
5. Overlap coefficient
6. cosine similarity

## Method descrition
1. 首先我們有兩件文件，文件A以及文件B，將這兩個文件進行斷詞斷句。 *** 任務目標:檢測文件A 是否抄襲 (目前database 僅有一件文件B)
2. 將斷詞結果的list套入距離/相似度的演算法進行文件A的句子(7句)以及文件B的句子(六句)兩兩比較。
3. 將相似程度最高的句子內容以及相似分數/距離列出來(以文件A為基準，找到文件B當中相似度最高的句子)。
4. 將一樣的文字敘述透過顏色標註(疑問點:目前的作法是將文件B token內容直接丟進去，看是否有無在文件A token裡面，不考慮順序)
