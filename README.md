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

Önce kullanacağımız modülleri import ediyoruz: 

```python
import pandas as pd
```
**Not:** elimizde olan data.csv isimli excel dosyasını okuyabilmek için `df=pd.read_csv('data.csv')`

kullanıyoruz, ancak bu aşamada bir utf-8 hatası aldık bunu gidermek için encodingi değiştirmemiz gerekiyor ;

`df=pd.read_csv('data.csv',encoding='latin1')` Şimdi veri setimizi incelemeye başlayabiliriz.

**İstenilenler**
Bizden istenilenleri şu şekilde özetleyebiliriz:

- The first step for this project is to import the dataset and create three data
frames
  - Customer
  - Products
  - Orders
- Insert the three data frames in a SQLite database
- Import the tables from the database and merge them into a single data
frame
- Segment the customers using KMeans and highlight the characteristics
of the segments
- Selection of number of customers segments should be justified
- Create RFM table ( Recency, Frequency and Money)
