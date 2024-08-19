# Laptop Fiyat Tahmin Projesi

Bu proje, ürün fiyatlarını tahmin etmek için bir makine öğrenmesi modeli kullanmaktadır. Özellikle, RandomForestRegressor kullanarak ürünlerin fiyatlarını tahmin etmek amacıyla geliştirilmiştir. Bu proje, kategorik verilerin sayısal verilere dönüştürülmesi, verilerin eğitim ve test setlerine ayrılması ve model performansının değerlendirilmesini içerir.

## İçerik

- [Proje Hakkında](#proje-hakkında)
- [Kurulum](#kurulum)
- [Kullanım](#kullanım)
- [Sonuçlar](#sonuçlar)
- [Veri](#veri)
- [Lisans](#lisans)

## Proje Hakkında

Bu proje, ürün fiyatlarını tahmin etmek için bir RandomForestRegressor modeli kullanmaktadır. Veri kümesindeki kategorik özellikler sayısal verilere dönüştürülmüştür ve modelin başarısını değerlendirmek için R² skoru ve Ortalama Kare Hata (MSE) hesaplanmıştır. Ayrıca, tahmin edilen ve gerçek fiyatlar Hindistan Rupisi (INR) ile Türk Lirası (TRY) arasında dönüştürülmüştür.

## Kurulum

Gerekli kütüphaneleri yüklemek için aşağıdaki komutu kullanabilirsiniz:

```bash
pip install pandas scikit-learn
```

## Kullanım

1. Veriyi `data/data_preprocessed.csv` dosyasına yerleştirin.
2. Python scriptini çalıştırarak modeli eğitin ve tahminler yapın:

```bash
python model.ipynb
```

## Sonuçlar

Modelin performansı aşağıdaki metriklerle değerlendirilmiştir:

- **Ortalama Kare Hata (MSE)**: Modelin tahminlerinin gerçek değerlerden ne kadar uzak olduğunu gösterir.
- **R² Skoru**: Modelin veri kümesindeki varyansı ne kadar iyi açıkladığını ölçer.

Örnek tahmin sonuçları:

- **Tahmin Edilen Fiyat (ilk test örneği, TRY olarak)**: (Örnek değer)
- **Gerçek Fiyat (ilk test örneği, TRY olarak)**: (Örnek değer)

Aşağıdaki tabloda gerçek ve tahmin edilen fiyatlar karşılaştırılmaktadır:

| Gerçek Fiyat (INR) | Tahmin Edilen Fiyat (INR) | Gerçek Fiyat (TRY) | Tahmin Edilen Fiyat (TRY) |
|--------------------|---------------------------|--------------------|---------------------------|
| ...                | ...                       | ...                | ...                       |

## Veri

Veri kümesi, `data/data_preprocessed.csv` dosyasında bulunmaktadır. Bu dosya, modelin eğitimi ve test edilmesi için gerekli olan işlenmiş verileri içermektedir.

## Lisans

Bu proje [MIT Lisansı](LICENSE) altında lisanslanmıştır.
