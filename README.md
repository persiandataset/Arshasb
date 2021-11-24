# Arshasb
Persian OCR dataset

In this repository, Arshaseb (ancient Iranian name) Persian OCR dataset  is located.
This datasets contains 33,000 pages of Persian text, of which 7,000 pages have been published for free.<br>

# Download
There are 100 samples of this dataset in Arshasb_samples.tar.gz </br>
You can download Arshasb dataset with 7k pages in this <a href="https://drive.google.com/file/d/1G9JEZY9MSzaND8ynnFodIXQvMMM1_6J3/view?usp=sharing">link</a> (~700M)</br>
Also, if you want a 33,000-page dataset, contact me [ hubare.ra[at]gamil.com ].

# Detail
For each page in this dataset, a subfolder with the same name as the page has been created.
Each subfolder contains 4 files, for example in subfolder 00001 we have:

    1.page_00001.png [ Page image ]
    2.label_00001.xlsx [ The exact location of each word on the page ]
    3.fulltext_00001.txt [ Full text in page ]
    4.line_00001.xlsx [ The exact location of each line on the page ]
    
    Introducing label_xxxx.xlsx columns:
    1.word
    2.line [show index-line word]
    3.point(1-2-3-4) [show location of each word]
<img src="https://github.com/persiandataset/Arshasb/blob/main/fig1.png"></img>
    
