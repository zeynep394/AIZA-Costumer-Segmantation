# AIZA-Costumer-Segmantation
Costumer Segmantation homework using clustering

## Learn Clustering with Python and Pandas

Merhaba, bu ödevde costumer segmantation verisiyle çalışarak clusteringin mantığını öğreneceğiz. Clustering gerçekleştirmek için bir çok algoritma mevcut ancak biz bugün sadece bir tanesini ele alacağız: K-means clustering. Hazırsanız haydi başlayalım!

Takip edeceğimiz adımlar kabaca şu şekilde:

- Veri Ön Hazırlığı
- Benzerlik Matrisi Hazırlama
- K-means Algoritmasının Çalıştırılması
- Sonuçların İşlenmesi

### Veri Ön Hazırlığı
Kullanacağımız veri seti:

[recommendationdata.csv](https://github.com/zeynep394/AIZA-Costumer-Segmantation/blob/main/data.csv) - bir şirkete ait müşteri, ürün ve sipariş bilgilerini içeren csv formatındaki veri seti. 

Önce 

```python
import pandas as pd
```

kullanarak pandası import ediyoruz elimizde olan data.csv isimli excel dosyasını okuyabilmek için `df=pd.read_csv('data.csv')`

kullanıyoruz, ancak bu aşamada bir utf-8 hatası aldık bunu gidermek için encodingi değiştirmemiz gerekiyor ;

`df=pd.read_csv('data.csv',encoding='latin1')`

evet her şey yolunda gözüküyor!

Şimdi veri setimizi incelemeye başlayabiliriz.

