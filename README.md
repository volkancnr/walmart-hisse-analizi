Bu projede Python kullanarak Walmart hisse senedi fiyatları üzerinde veri analizi ve zaman serisi modellemesi gerçekleştirilmiştir. Çalışmada yfinance API ile hisse senedi verileri çekilmiş, Pandas ve NumPy ile veri işleme yapılmış, Matplotlib ve Seaborn ile görselleştirme gerçekleştirilmiştir. Trend, mevsimsellik ve oynaklık analizleri için Statsmodels, SciPy ve TA-Lib gibi kütüphaneler kullanılmıştır. Veriler 2000 sonrası dönemi kapsamakta olup, trend analizi, mevsimsellik, artık bileşen analizi ve oynaklık (standart sapma) gibi önemli finansal göstergeler incelenmiştir.
 Walmart Hisse Senedi Fiyat Veri Seti ve Keşifsel Veri Analizi (EDA)

VERİ SETİ ÖZETİ:

 Walmart Hakkında
 
Walmart Inc., hipermarketler, indirimli mağazalar ve marketlerden oluşan bir zincir işleten çok uluslu bir perakende şirketidir. Gelir açısından dünyanın en büyük şirketlerinden biri ve perakende sektöründe önemli bir oyuncudur. Walmart'ın hisseleri büyük borsalarda aktif olarak işlem görmektedir ve bu da onu finansal analiz konu haline getirir.
 
 Veri Kümesi Genel Bakışı
 
Bu veri seti, Python API'sini kullanarak doğrudan Yahoo Finance'den alınan Walmart için tarihi hisse senedi fiyat verilerini içerir yfinance. Veriler günlük hisse senedi fiyatlarını kapsar ve birden fazla temel finansal gösterge içerir.
 
 Veri Setinde Bulunan Özellikler
 
•	Tarih  – Kaydedilen işlem günü.

•	Açılış Fiyatı  – Piyasa açılışındaki fiyat.

•	Yüksek Fiyat  – Günün en yüksek fiyatı.

•	Düşük Fiyat  – Günün en düşük fiyatı.

•	Kapanış Fiyatı  – Piyasanın kapanış fiyatı.

•	Düzeltilmiş Kapanış Fiyatı  – Bölünmeler ve temettüler için düzeltilmiş kapanış fiyatı.

•	İşlem Hacmi  – Toplam işlem gören hisse senedi sayısı.

•	Temettüler  – Hissedarlara yapılan nakit ödemeler.

•	Hisse Senedi Bölünmeleri  – Hisse senedi bölünme olaylarını kaydeder.

ANALİZ VE GÖRSELLEŞTİRMELER

![image](https://github.com/user-attachments/assets/90fe3604-d69a-4bdd-84a1-18e4256cb720)

Burada hissemizin açılış kapanış hacim değerlerinin başlangıçtan sonuna kadar minimum maksimum ortalama gibi betimsel istatistiklerini görmekteyiz. Hisse en az 0.002 dolar seviyelerine inmişken en fazla 105 dolar seviyesine kadar da çıkmıştır.

