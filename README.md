CLUEWSC2020: WSC Winograd模式挑战中文版，中文指代消解任务

Winograd Scheme Challenge（WSC）是一类代词消歧的任务。 

即判断句子中的代词指代的是哪个名词。题目以真假判别的方式出现，如：

句子：这时候放在床上枕头旁边的手机响了，我感到奇怪，因为欠费已被停机两个月，现在它突然响了。需要判断“它”指代的是“床”、“枕头”，还是“手机”？

数据来源：数据有CLUE benchmark提供，从中国现当代作家文学作品中抽取，再经语言专家人工挑选、标注。

数据形式：

 {"target": 
     {"span2_index": 37, 
     "span1_index": 5, 
     "span1_text": "床", 
     "span2_text": "它"}, 
 "idx": 261, 
 "label": "false", 
 "text": "这时候放在床上枕头旁边的手机响了，我感到奇怪，因为欠费已被停机两个月，现在它突然响了。"}
 "true"表示代词确实是指代span1_text中的名词的，"false"代表不是。
数据集大小：

训练集：1244

开发集：304

<a href='https://storage.googleapis.com/cluebenchmark/tasks/cluewsc2020_public.zip'>CLUEWSC2020数据集下载</a>