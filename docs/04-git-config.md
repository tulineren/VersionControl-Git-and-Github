## Git Config Komutları
### Kullanıcı Bilgileri

```bash
git config --global user.name "Ad Soyad"
```
- Git’te yapılan commit’lerde görünen adını ayarlar.

```bash
git config --global user.email "email@example.com"
```
- Commit’leri GitHub hesabınla eşleştiren e-posta adresini ayarlar.

```bash
git config user.name
```
- Ayarlı olan kullanıcı adını görüntüler.

```bash
git config user.email
```
- Ayarlı olan e-posta adresini görüntüler.

**Commit**, Git’te projede yapılan değişikliklerin belirli bir açıklama (commit mesajı) ile kaydedilmesini sağlayan bir işlemdir. İlk bakışta önemsiz gibi görünse de,
özellikle büyük projelerde ne kadar kritik olduğu anlaşılır. Her commit projenin o anki durumunu saklar ve gerektiğinde önceki sürümlere geri dönülmesine imkân tanır.
