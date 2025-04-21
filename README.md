# 📉 Sosyal Medya Kullanıcılarının PySpark ile Analizi

## 🔍 Amaç
Bu projede amacımız, `randomuser.me/api` adresinden elde edilen sahte sosyal medya kullanıcı verilerini analiz ederek:

- Kullanıcıların yaş ve kayıt bilgileri üzerinden istatistiksel bilgiler çıkarmak,
- Cinsiyet ve ülke bazlı gruplamalarla ortalama ve sıralama analizleri yapmak,
- PySpark kullanarak veri üzerinde çok boyutlu analizleri DataFrame API ve Spark SQL ile uygulamalı şekilde göstermek.

---

## 📄 Proje Dosyaları

| Dosya Adı                      | Açıklama                                                                 |
|-------------------------------|--------------------------------------------------------------------------|
| `Bitirme_Projesi.ipynb`       | 10 dakika boyunca 2 saniyelik aralıklarla API'den veri çekilir ve `.parquet` dosyası olarak kaydedilir. |
| `kullanici_verileri_last.parquet` | Çekilen verilerin `.parquet` formatındaki hali. Spark ile analiz için kullanılır.       |
| `pyspark_analiz.ipynb`        | Kayıtlı veriler PySpark ile analiz edilir, 3 soruya Spark SQL ve DataFrame API ile cevap verilir.       |

---

## 📊 Gerçekleştirilen Analizler

1. **Soru 1:** Kadın ve erkek kullanıcıların ortalama yaşı ve ortalama uygulama kullanım süreleri  
2. **Soru 2:** Cinsiyet ve ülkeye göre ortalama yaş ve uygulama kullanım süreleri  
3. **Soru 3:** Her ülke + cinsiyet grubu için en yaşlı ilk 3 kullanıcının belirlenmesi

---

## 🚀 Nasıl Çalıştırılır?

1. `Bitirme_Projesi.ipynb` dosyasını çalıştırarak API'den verileri alın ve `kullanici_verileri_last.parquet` dosyasını oluşturun.
2. `pyspark_analiz.ipynb` dosyasını PySpark destekli JupyterLab veya terminalde çalıştırarak analizleri gözlemleyin.

---

## 📁 Gereksinimler
- Python 3.8+
- Pandas
- PySpark
- pyarrow (Parquet yazma için)

---

## 📊 Teknolojiler
- **Veri Kaynağı:** `https://randomuser.me/api`
- **Veri Formatı:** JSON → Pandas DataFrame → Parquet
- **Veri Analizi:** PySpark DataFrame API & Spark SQL
- **Analiz Ortamı:** Jupyter Notebook
