# AIZA-Costumer-Segmantation
Costumer Segmantation homework using clustering

Merhaba, bu ödevde clustering kullanarak costumer segmantaion verisiyle çalışmayı öğreneceğiz. Haydi başlayalım!

Önce `import pandas as pd` kullanarak pandası import ediyoruz elimizde olandata.csv isimli excel dosyasını okuyabilmek için


`df=pd.read_csv('data.csv')`

kullanoyoruz ancak bu aşamada bir utf8 hatası aldık bunu gidermek için encodingi değiştirmemiz gerek;

`df=pd.read_csv('data.csv',encoding='latin1')`

evet her şey yolunda gözüküyor!


