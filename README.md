# Arshasb
Persian OCR dataset

* In this repository, Arshaseb (ancient Iranian name[ اَرشاسب ]) Persian OCR dataset  is located.
* This dataset contains 33,000 pages of Persian text, of which 7,000 pages have been published for free.<br>
* The words that are placed next to each other are interdependent and represent one subject. <br>
* More precisely, the placement of the words is meaningful, and this helps to use NLP models in the OCR process.<br>
* In this datasets, the position of each word is precisely labeled. Look at this sample:</br>
<img src="https://github.com/persiandataset/Arshasb/blob/main/page_08734.png"></img>
    
# Download
* There are 100 samples of this dataset in Arshasb_samples.tar.gz </br>
* You can download Arshasb dataset with 7k pages in this <a href="https://drive.google.com/file/d/1G9JEZY9MSzaND8ynnFodIXQvMMM1_6J3/view?usp=sharing">link</a> (~730M)</br>
* Also, if you want a 33,000-page dataset, contact me by hubare.ra[at]gmail.com .

# Detail
* The number of unique words with the removal of numbers and punctuation is 97498. In the 7k version, this number is reduced to 40911 unique words.</br>
* The content of this dataset includes public and news texts.</br>
* This dataset uses Far_ketab font. [<a href="https://www.fontyab.com/3247/far_ketab.html">website</a>]</br>

* For each page in this dataset, a subfolder with the same name as the page has been created.
* Each subfolder contains 4 files, for example in subfolder 00001 we have:</br>

    - 1.page_00001.png [ Page image ]
    - 2.label_00001.xlsx [ The exact location of each word on the page ]
    - 3.fulltext_00001.txt [ Full text in page ]
    - 4.line_00001.xlsx [ The exact location of each line on the page ]
    
    - Introducing label_xxxx.xlsx columns:
      - 1.word
      - 2.line [show index-line word]
      - 3.point(1-2-3-4) [show location of each word]

<img src="https://github.com/persiandataset/Arshasb/blob/main/fig1.png"></img>
    
# Sample code for read label_xxxx.xlsx
```python

label = pd.read_excel('Arshasb_7k/00001/label_00001.xlsx')
data = []
for j in range(len(label)):
    #read word
    word = label['word'][j]
    #read index_line word
    index_line = label['line'][j]
    #read points
    point1 = eval(label['point1'][j])
    point2 = eval(label['point2'][j])
    point3 = eval(label['point3'][j])
    point4 = eval(label['point4'][j])
    data.append({'number':j , 'word':word, 'line':index_line ,'point1':point1,'point2':point2,'point3':point3,'point4':point4})
```
# Donation
I try to publish free Persian datasets in github. Your financial support will encourage me. Donation link : https://www.patreon.com/persiandataset
