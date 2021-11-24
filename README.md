# Arshasb
Persian OCR dataset

In this repository, Arshaseb (ancient Iranian name) Persian OCR dataset  is located.
This datasets contains 33,000 pages of Persian text, of which 7,000 pages have been published for free.
For each page in this dataset, a subfolder with the same name as the page has been created.

Each subfolder contains 4 files, for example in subfolder 00001 we have:</br>

    1.page_00001.png [ Page image ]
    2.label_00001.xlsx [ The exact location of each word on the page ]
    3.fulltext_00001.txt [ Full text in page ]
    4.line_00001.xlsx [ The exact location of each line on the page ]
    
Introducing label_xxxx.xlsx columns:</br>
    1.word</br>
    2.line [show index-line word]</br>
    3.point(1-2-3-4) [show location of each word]</br>
    <img src="https://github.com/persiandataset/Arshasb/blob/main/fig1.png"></img>
    
