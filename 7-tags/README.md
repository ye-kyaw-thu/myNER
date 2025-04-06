# myNER (7 Tags)


## License

Creative Commons Attribution-NonCommercial-Share Alike 4.0 International (CC BY-NC-SA 4.0) License  
[Details Info of License](https://creativecommons.org/licenses/by-nc-sa/4.0/)  

## NER Tags

myNER corpus containing 16, 605 sentences, originally sourced from data taken from the [myPOS](https://github.com/ye-kyaw-thu/myPOS/) version 3 corpus, is manually annotated NER corpus for our experiments. In our corpus, we used the BIOES (B-Begin, I-Inside, O-Outside, E-End, S-Single) tagging scheme with a total of seven tag categories as shown in Table 1.  

<div align="center">  
  
**Table 1. Tag Names, Descriptions, and Examples of myNER Corpus**  

| **Tag** | **Description**                       | **Examples**                                                                 |
|--------|---------------------------------------|------------------------------------------------------------------------------|
| DATE   | Date                                  | ၁ ရက် ၅ လ ၁၉၉၆ (01-05-1996), ကဆုန်လပြည့် (full moon day of Kasone)          |
| TIME   | Time                                  | မနက် ၆ နာရီ ၁၀ မိနစ် (06:10 AM)                                            |
| NUM    | Numbers                               | ၁ (1), ၁သန်း (1 Million)                                                    |
| PER    | Person Names                          | အန်တိုနီယို (Antonio), ကောင်းလွင်သန့် (Kaung Lwin Thant)                    |
| ORG    | Organizations and Institutions        | မိုက်ခရိုဆော့ (Microsoft Inc), ဟားဗတ်တက္ကသိုလ် (Harvard University)         |
| LOC    | Locations and Geographic Features     | အာရှတိုက် (Asia), ထိုင်းနိုင်ငံ (Thailand)                                 |
| O      | Outside                               | Nonspecific entities which do not match the above tags                      |

</div>

## Tag Distribution

The following figure shows the distribution of named entity (NE) categories in the **myNER (7-tags)** corpus, excluding the non-entity tag `O`. The count includes tokens from the training, validation, and test sets.

This visualization helps users understand the balance and representation of each NE tag in the dataset. As shown, `LOC` (location) entities are the most frequent, followed by `NUM`, `PER`, and `DATE`, while `ORG` and `TIME` are relatively less frequent.

<div align="center">

<img src="https://github.com/ye-kyaw-thu/myNER/blob/main/7-tags/doc/datatags_2.png" alt="Tag Distribution in myNER Corpus" width="600"/>

<br/>

**Figure 1: Distribution of NER tag categories in the myNER corpus (excluding the 'O' tag).**  

</div>

## Corpus

The corpus files are available under the [myNER/7-tags/corpus_ver.1.0/](https://github.com/ye-kyaw-thu/myNER/tree/main/7-tags/corpus_ver.1.0) folder.  
Each file uses a **CoNLL-style format** with **three columns**: word, part-of-speech (POS), and named entity (NER) tag, separated by tabs.

- [myNER-7tags_ver.1.0.conll](https://github.com/ye-kyaw-thu/myNER/blob/main/7-tags/corpus_ver.1.0/myNER-7tags_ver.1.0.conll): Full corpus (version 1.0), UTF-8 encoded  
- [train_v5.conll](https://github.com/ye-kyaw-thu/myNER/blob/main/7-tags/corpus_ver.1.0/train_v5.conll): Training set  
- [val_v5.conll](https://github.com/ye-kyaw-thu/myNER/blob/main/7-tags/corpus_ver.1.0/val_v5.conll): Validation set  
- [test_v5.conll](https://github.com/ye-kyaw-thu/myNER/blob/main/7-tags/corpus_ver.1.0/test_v5.conll): Test set

## Format

Each line in the corpus follows a **CoNLL-style tab-separated format** with three columns:  
**Word**, **Part-of-Speech (POS) Tag**, and **Named Entity (NER) Tag**.

Sentences are separated by blank lines.

Below are three example sentences taken from the **top of the test set** (`test_v5.conll`). These examples illustrate different types of named entities:

```
ရွာ	n	O
နေရာ	n	O
ကုတ်	n	O
မှာ	ppm	O
၂၁၃၉၈၃	num	S-NUM
ဖြစ်	v	O
သည်	ppm	O
။	punc	O

ကျောက်ဖြူတိုင်	n	B-LOC
ရွာ	n	E-LOC
သည်	ppm	O
စစ်ကိုင်း	n	B-LOC
တိုင်း	part	I-LOC
ဒေသကြီး	n	E-LOC
၊	punc	O
ယင်းမာပင်	n	B-LOC
ခရိုင်	n	E-LOC
၊	punc	O
ဆားလင်းကြီး	n	B-LOC
မြို့နယ်	n	E-LOC
၊	punc	O
ဖောင်းကတာ	n	B-LOC
ကျေးရွာ	n	I-LOC
အုပ်စု	n	E-LOC
၌	ppm	O
တည်ရှိ	v	O
သည်	ppm	O
။	punc	O

ကြက်ခြေနီ	n	S-ORG
မှ	ppm	O
ပြောရေးဆိုခွင့်ရှိသူ	n	O
MattCochrane	fw	S-PER
မော့တ်ကော့ချရင်း	n	S-PER
က	ppm	O
ထို	adj	O
ဆိုင်ကလုန်း	n	O
ကြောင့်	ppm	O
သေကံမရောက်သက်မပျောက်	v	O
ဘဲ	part	O
ကျန်ရစ်	n	O
များ	part	O
သည်	ppm	O
အလုံးစုံ	n	O
လိုအပ်	v	O
သည်	ppm	O
ဟု	part	O
ပြော	v	O
ခဲ့	part	O
သည်	ppm	O
။	punc	O
```

## Previous Works on Myanmar Language NER

1. Hsu Myat Mo et al., "CRF-Based Named Entity Recognition for Myanmar Language,"  
   in *Genetic and Evolutionary Computing (ICGEC 2016)*, J. S. Pan et al., Eds.,  
   *Advances in Intelligent Systems and Computing*, vol. 536. Cham: Springer, 2017.  
   [https://link.springer.com/chapter/10.1007/978-3-319-48490-7_24](https://link.springer.com/chapter/10.1007/978-3-319-48490-7_24)   

2. Hsu Myat Mo and Khin Mar Soe, "Named Entity Recognition for Myanmar Language,"  
   in *Proceedings of the 2022 International Conference on Communication and Computer Research (ICCR 2022)*,  
   Sookmyung Women’s University, Seoul, Korea, 2022.  
   [https://www.researchgate.net/publication/379828999_Named_Entity_Recognition_for_Myanmar_Language](https://www.researchgate.net/publication/379828999_Named_Entity_Recognition_for_Myanmar_Language)   


## Publication

The myNER 7 Tags corpus (version 1.0) is being used for The International Conference on Cybernetics and Innovations (ICCI 2025) Conference paper.  

## Citation

If you use the **myNER (7-tag)** corpus in your research, we would appreciate it if you cite the following reference:  

Kaung Lwin Thant, Kwankamol Nongpong, Ye Kyaw Thu, Thura Aung, Khaing Hsu Wai, Thazin Myint Oo , "myNER: Contextualized Burmese Named Entity  Recognition with Bidirectional LSTM and fastText  Embeddings via Joint Training with POS Tagging", the International Conference on Cybernetics and Innovations (ICCI 2025), April 2-4, Pattaya Chonburi, Thailand pp.xx-xx \[to Appear\] 

