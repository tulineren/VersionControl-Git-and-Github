# Version Control: Git and Github #
## Git Nedir?
- Yazılım projelerinde kullanılan bir versiyon kontrol sistemidir.
- Dosyalarda yapılan değişiklikleri kaydeder(örneğin oyun geliştirirken arayüzde yaptığım değişiklikleri düzenli olarak kaydediyordum).
- Değişikliklerin ne zaman ve kim tarafından yapıldığını takip eder.
- Hatalı veya yanlış işlemler yapıldığında önceki sürümlere geri dönülebilir.
- Birden fazla kişinin aynı proje üzerinde düzenli şekilde çalışmasına imkân tanır.

## Terminal Kullanımı (Temel Komutlar)

pwd    : Bulunulan dizinin tam yolunu gösterir  
ls     : Dizindeki dosya ve klasörleri listeler  
cd     : Dizin değiştirmek için kullanılır  
cd ..  : Bir üst dizine geçer  
clear  : Terminal ekranını temizler  



### Dosya ve Klasör İşlemleri

mkdir  : Yeni bir klasör oluşturur.
 Örnek : mkdir GitKursu
touch  : Yeni bir dosya oluşturur.
 Örnek : touch not.txt
- Terminal kullanarak dosya ve klasör oluşturabiliriz.

### Dosya Silme Komutları

rm     : Dosya siler  
 Örnek : rm not.txt
rm -rf : Klasör ve içeriğini geri dönüşsüz siler
 Örnek : rm -rf GitKursu

#### rm ve rm -rf Arasındaki Fark

rm     : Tekil dosyalar için kullanılır
rm -rf : Klasörleri ve içindeki her şeyi siler
- rm -rf daha tehlikelidir, yanlış kullanılırsa önemli dosyalar silinebilir
