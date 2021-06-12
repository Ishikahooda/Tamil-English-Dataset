# Abstract
The Tamil language is spoken by 80 million people around the world. The translation between Tamil and English leads to a signiﬁcant impact by helping in the understanding of Tamil scripts, which otherwise would be a tedious, costly, and time-consuming process. Thus, developing an automated system to perform Tamil to English translation would save human time and effort. We publicly release a new high-quality corpus for standard training, evaluation, and report results experiments with two different architectures based on Encoder-Decoder to translate Tamil to English. We further tried to improve it by experimenting with pre- trained word embeddings and tuning hyperparameters. Although Google-Translator also provides Tamil to English and vice versa, our implemented architectures, along with the new dataset, completely outperformed the Google Translator with a margin of 7.5 BLEU score. Moreover, our proposed model solves out of vocabulary and polysemy problems up to a greater extent.

## Paper Preview:
Feel free to download our paper using this [link](https://drive.google.com/file/d/11AvwDVFWOYZb1ZT1S-sGeYBIgnJzqBvb/view?usp=sharing)

## Tamil-English-Dataset (Update: 12th June 2021)
In our experimentation we used 236,427 parallel English - Tamil Sentences, further we add more sentences and to the dataset. The final dataset is divided into six English <--> Tamil parallelly translated files for ease of distribution, please check the dataset folder. If you want to test our latest trained model and other languages we covered, please visit [TranslateMe Network](https://translateme.network/)

## Authors

If you still face an issue, feel free to contact the authors:
1. [Ravneet Punia](https://www.linkedin.com/in/ravneetpunia/)
2. [Ishika Hooda](https://www.linkedin.com/in/ishikahooda/)

## Results
All the evaluated methodologies for Tamil-to-English translations were done using the same dataset for both the architectures. We compared our results with Google translator . The transformer translator outperforms the proposed Tamil translator and the Google translator, which is known to be the best-reported model for machine translation. While experimenting with Tamil translator, it became clear that pre-trained embeddings performing better than trained from Corpus, hence for transformer translator, only tested with pre-trained embeddings.

### Qualitative Evaluation
Apart from BLEU Score evaluation, human evaluation was done by 3 Tamil scholars, given 100 randomly chosen translation from each other, using the following rating scheme:

* good [5]: interpretable in the correct meaning by a native speaker of Tamil; no incorrectly translated content word.
* helpful [3]: partially distorted, but interpretable with some context information (tolerant against errors in word order and against incorrect function words).
* incorrect [1]: contains incorrectly translated content words and/or is uninterpretable.

Final scores user rating is calculated as an average of all ratings given by scholars to each model, which is shown in below table.


|     Model Architecture                               | BLEU  | User Rating |
|    --------------------                              | ----- | ----------- |	
|1. Google Translator                                  | 8.6   |	  2.6      |
|2. Tamil Translator                                   | 21.6  |    14.6     |
|3. Tamil Translator + pretrained Embeddings           | 14.9  |    3.1      |      	       			    
|4. Transformer Translator + pre-trained Embeddings    | 16.1  |    3.8      |


## Citation
If you use our dataset or any other part of the paper, don't forget to cite us using

```bibtex
@article{jain2020neural,
  title={Neural machine translation for Tamil to English},
  author={Jain, Minni and Punia, Ravneet and Hooda, Ishika},
  journal={Journal of Statistics and Management Systems},
  volume={23},
  number={7},
  pages={1251--1264},
  year={2020},
  publisher={Taylor \& Francis}
}
```