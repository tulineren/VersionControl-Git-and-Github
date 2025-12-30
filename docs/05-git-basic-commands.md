## Git Temel Komutlar


### git init
- Bulunulan klasörü bir Git deposu haline getirir ve versiyon kontrolünü başlatır.
- Klasörün içine gizli bir .git dizini oluşturur. Bu .git klasörü, Git’in tüm geçmiş ve ayar bilgilerini tutar.
- Bu işlemden sonra Git, klasörde yapılan dosya değişikliklerini takip edebilir.
- Henüz dosyalar izlenmez; bunun için git add komutu kullanılır.

```bash
git init
```

### git status
Çalışma dizininin durumunu gösterir; hangi dosyaların değiştiğini, hangilerinin commit’e hazır olduğunu belirtir.
 
```bash
git status
```

### ls -la
Bulunulan dizindeki tüm dosya ve klasörleri (gizli dosyalar dahil) detaylı şekilde listeler.

```bash
ls -la
```

### git add
Yapılan değişiklikleri stage alanına ekler (commit’e hazırlık yapar).

```bash
git add
```

### git commit
Stage alanındaki değişiklikleri, verilen mesajla birlikte kalıcı olarak kaydeder.

```bash
git commit -m "İlk mesaj yazıldı"
```

### git log
Yapılan commit’lerin geçmişini listeler.

```bash
git log
```

**Commit hash’i:**
- git log çıktısında her commit’e ait bir hash (benzersiz kimlik) bulunur.
- Bu hash’ler birbirinden farklıdır ve her commit’i tekil olarak temsil eder.

### git commit -a
- Daha önce izlenen (tracked) dosyalardaki değişiklikleri otomatik olarak stage edip commit eder.
- Yeni dosyaları kapsamaz.

```bash
git commit -a -m "Mesaj"
```

### git add .
Bulunulan dizindeki tüm değişiklikleri (yeni dosyalar dahil) stage alanına ekler.

```bash
git add .
```

### .gitignore Nedir?
- .gitignore, Git’in hangi dosya ve klasörleri takip ETMEMESİ gerektiğini belirten dosyadır.
- İçine yazılan dosyalar commit edilmez ve Git geçmişine girmez.
- Genellikle: Geçici dosyalar, derleme çıktıları, IDE ayar dosyaları, gizli bilgiler (token, config vb.)için kullanılır.
- Projenin ana dizininde bulunur.
- Takip edilmeyen dosyalar git status çıktısında görünmez.

```bash
__pycache__/
node_modules/
.env
*.log
```

### GitHub’daki .gitignore Template (Şablon) Dosyaları
GitHub, farklı programlama dilleri ve araçlar için hazır .gitignore şablonları sunar.

Amaç:
- Gereksiz dosyaların yanlışlıkla repoya eklenmesini önlemek
- Standart ve temiz repo yapısı oluşturmak
- Yeni repo oluştururken “Add .gitignore” seçeneğiyle eklenebilir.

Şablonlar: O dile veya araca özel olarak yaygın ignore edilen dosyaları içerir.

### Popüler Template Örnekleri
Python → __pycache__/, .venv/ |
Node → node_modules/ |
Java → target/ |
Unity → Library/, Temp/ |
VisualStudio / JetBrains → .vs/, .idea/

### Neden Template Kullanılır?
- Her dosyayı tek tek düşünmek gerekmez.
- Sektör standardına uygundur.
- Yeni başlayanlar için hataları azaltır.
- Takım projelerinde düzen sağlar.
