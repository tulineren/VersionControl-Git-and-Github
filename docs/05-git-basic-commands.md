## Git Temel Komutlar

### git status
Çalışma dizininin durumunu gösterir; hangi dosyaların değiştiğini, hangilerinin commit’e hazır olduğunu belirtir.
 
```bash
git status
```

### git init
Bulunulan klasörü bir Git deposu haline getirir ve versiyon kontrolünü başlatır.

```bash
git init
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
