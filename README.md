# Versiyon Kontrolleri: Git ve Github Kullanımı #
## Git Nedir?
- Yazılım projelerinde kullanılan bir versiyon kontrol sistemidir.
- Dosyalarda yapılan değişiklikleri kaydeder(örneğin oyun geliştirirken arayüzde yaptığım değişiklikleri düzenli olarak kaydediyordum).
- Değişikliklerin ne zaman ve kim tarafından yapıldığını takip eder.
- Hatalı veya yanlış işlemler yapıldığında önceki sürümlere geri dönülebilir.
- Birden fazla kişinin aynı proje üzerinde düzenli şekilde çalışmasına imkân tanır.

## Terminal Kullanımı (Temel Komutlar)

pwd    : Bulunulan dizinin tam yolunu gösterir. 
ls     : Dizindeki dosya ve klasörleri listeler.  
cd     : Dizin değiştirmek için kullanılır.  
cd ..  : Bir üst dizine geçer.
clear  : Terminal ekranını temizler.  



### Dosya ve Klasör İşlemleri

mkdir  : Yeni bir klasör oluşturur.
 Örnek : mkdir GitKursu
touch  : Yeni bir dosya oluşturur.
 Örnek : touch not.txt
- Terminal kullanarak dosya ve klasör oluşturabiliriz.

### Dosya Silme Komutları

rm     : Dosya siler.  
 Örnek : rm not.txt
rm -rf : Klasör ve içeriğini geri dönüşsüz siler.
 Örnek : rm -rf GitKursu

#### rm ve rm -rf Arasındaki Fark

rm     : Tekil dosyalar için kullanılır.
rm -rf : Klasörleri ve içindeki her şeyi siler.
- rm -rf daha tehlikelidir, yanlış kullanılırsa önemli dosyalar silinebilir.

## Git Config Komutları

git config --global user.name "Ad Soyad"
- Git’te yapılan commit’lerde görünen adını ayarlar.

git config --global user.email "email@example.com"
- Commit’leri GitHub hesabınla eşleştiren e-posta adresini ayarlar.

git config user.name
- Ayarlı olan kullanıcı adını görüntüler.

git config user.email
- Ayarlı olan e-posta adresini görüntüler.

**Commit**, Git’te projede yapılan değişikliklerin belirli bir açıklama (commit mesajı) ile kaydedilmesini sağlayan bir işlemdir; her commit projenin o anki durumunu saklar ve gerektiğinde önceki sürümlere geri dönülmesine imkân tanır.
## Git Görselleştirme

![Git branch ve merge yapısı](git-visual.png)

 **git status**: Çalışma dizininin durumunu gösterir; hangi dosyaların değiştiğini, hangilerinin commit’e hazır olduğunu belirtir.
 **git init**: Bulunulan klasörü bir Git deposu haline getirir ve versiyon kontrolünü başlatır.
 **ls -la**: Bulunulan dizindeki tüm dosya ve klasörleri (gizli dosyalar dahil) detaylı şekilde listeler.

