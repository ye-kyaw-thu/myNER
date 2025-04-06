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

## Corpus 

Under myNER/7-tags/corpus_ver.1.0/ folder,

myNER-7tags_ver.1.0.conll: myNER (7 tags) version 1.0, UTF-8 text, CONLL format  
train_v5.conll: Training data, UTF-8 text, CONLL format  
val_v5.conll: Validation data, UTF-8 text, CONLL format  
test_v5.conll: Test data, UTF-8 text, CONLL format  

## Publication

The myNER 7 Tags corpus (version 1.0) is being used for The International Conference on Cybernetics and Innovations (ICCI 2025) Conference paper.  

## Citation

If you use the **myNER (7-tag)** corpus in your research, we would appreciate it if you cite the following reference:  

Kaung Lwin Thant, Kwankamol Nongpong, Ye Kyaw Thu, Thura Aung, Khaing Hsu Wai, Thazin Myint Oo , "myNER: Contextualized Burmese Named Entity  Recognition with Bidirectional LSTM and fastText  Embeddings via Joint Training with POS Tagging ", the International Conference on Cybernetics and Innovations (ICCI 2025), April 2-4, Pattaya Chonburi, Thailand pp.xx-xx \[to Appear\] 

