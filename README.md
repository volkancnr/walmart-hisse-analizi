(net görseller word dosyasında kayıtlı zip klasörünü indirerek ulaşabilirsiniz)

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

![image](https://github.com/user-attachments/assets/2de2873c-7332-4f3c-821a-882f3210f492)

Bu grafikte 2000 sonrası hisse fiyatlarının durumu grafiklenmiş grafikte dünya çapında yaşanan 2008 Finansal krizi ve covid-19 dönemleri işaretlenmiştir.

![image](https://github.com/user-attachments/assets/81cc0ac1-f1e3-48f9-a70f-ac6088944dc7)
![image](https://github.com/user-attachments/assets/5c8b5c12-3025-47a7-afd6-494f59e4e9bf)

Grafikten de görüldüğü üzere hisse yılların belirli zamanlarında inişe geçse de yükselen trende sahiptir. 2000-2016 arası daha durağan geçse de 2016 sonrası yükseliş trendi güçlenmiştir.
Mevsimselliğe bakıldığında yılın belirli dönemlerinde hisse fiyatı yükselip düşüyor. Bu yükselmeler kasım aylarında görülürken düşüşler yaz aylarında görülmekte. Artık bileşen grafiğine bakıldığında 2016 sonrası belirgin bir dalgalanma var ve bu 2020 sonrası devam etmekte yani hissenin fiyatını takip etmesi zor hale gelmiştir. Standart sapma grafiğinde de bu durum görülmekte.

![image](https://github.com/user-attachments/assets/bf7ebcbc-e0fe-4f29-9a3c-1f0980c3edd4)

![image](https://github.com/user-attachments/assets/c71dc0bd-1c95-4702-9d69-5e7aa4382635)

Bu grafikte ise2000 sonrası yılları yüzde kaç kar ve zararla kapattığını görmekteyiz.

Bu grafik yılların ilk ve son fiyatlarını baz alarak yapıldığı için yıl içerisinde iniş ve çıkışları göz önüne almadan uzun vadeli yatırımcılar için direkt yılı nasıl bir kar ve zararda kapatıldığını görmek için yapılmıştır.
Görüldüğü gibi genel olarak karda kapatıldığı gözlemlenmektedir bu da uzun vadeli yatırımcılar için pozitif bir çıkarımdır.

SONUÇLAR:
•	Yükseliş trendi mevcut olup, 2020 sonrası ve özellikle 2024 başında güçlü bir yükseliş yakalamıştır.
•	Risk faktörleri arasında ani fiyat hareketleri ve ekonomik kriz dönemlerindeki sert düşüşler öne çıkmaktadır.
•	2020 yılı sonrası en sert düşüşün görüldüğü 2022 Mayıs haziran aylarında gerçekleşmiştir.
•	Yakın zamanda en göze çarpan yükseliş 2024'te +%72.2 olarak gerçekleşirken
Yakın tarihte göze çarpan düşüşü 2015 yılını %26.7 lik zararla kapatması olarak görülmüştür
•	50 ve 200 günlük hareketli ortalamalar yukarı yönlü trend gösterirken, fiyat son dönemde bu ortalamaların üzerinde seyretmektedir.
•	Fiyat göstergeleri arasında yüksek, işlem hacmi ile fiyat arasında zayıf korelasyon bulunmaktadır.

Walmart hisse senedinde genel olarak bir yükseliş trendi bulunmaktadır yapılan görsel analizlere dayanarak bu trende göre uzun vadede yatırım olacağı sunulmakta ancak 2020 sonrası yüksek volatilite nedeniyle kısa vadeli yatırım risklidir. 
