## Git Config Komutları
### Kullanıcı Bilgileri

Git’te yapılan commit’lerde görünen adını ayarlar.
```bash
git config --global user.name "Ad Soyad"
```

Commit’leri GitHub hesabınla eşleştiren e-posta adresini ayarlar.
```bash
git config --global user.email "email@example.com"
```

Ayarlı olan kullanıcı adını görüntüler.
```bash
git config user.name
Ad Soyad
```

Ayarlı olan e-posta adresini görüntüler.
```bash
git config user.email
email@example.com
```

**Commit**, Git’te projede yapılan değişikliklerin belirli bir açıklama (commit mesajı) ile kaydedilmesini sağlayan bir işlemdir. İlk bakışta önemsiz gibi görünse de,
özellikle büyük projelerde ne kadar kritik olduğu anlaşılır. Her commit projenin o anki durumunu saklar ve gerektiğinde önceki sürümlere geri dönülmesine imkân tanır.
