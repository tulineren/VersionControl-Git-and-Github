### HEAD Nedir?
HEAD, Git’te şu anda üzerinde çalıştığın yeri gösteren işaretçidir (pointer). Hangi branch’te olduğunu ve o branch’in son commit’ini işaret eder.

### git branch
Mevcut branch’leri listeler.
* işareti, şu anda bulunduğun branch’i gösterir.

```bash
Örnek çıktı:
* main
  new_branch
```

### git branch new_branch
- new_branch adında yeni bir branch oluşturur.
- Branch değişimi yapmaz, sadece oluşturur.
- Hâlâ önceki branch’te (genelde main) kalırsın.

### git switch new_branch
- Çalışılan branch’i new_branch olarak değiştirir.
- HEAD, artık new_branch’i gösterir.

### git merge
Bir branch’te yapılan değişiklikleri başka bir branch’e birleştirir.

Genelde:
- Önce hedef branch’e geçilir
- Sonra merge yapılır

```bash
Örnek kullanım
git switch main
git merge new_branch
```
new_branch içindeki commit’ler main branch’ine eklenir.

### Fast-Forward Nedir? 
Fast-forward, Git’te yapılan bir merge türüdür. Hedef branch ile birleştirilecek branch ayrılmamışsa, Git sadece ileri sarar.

Yani:
- Yeni bir merge commit’i oluşturulmaz.
- Branch işaretçisi (pointer) ileri taşınır.

### Ne Zaman Olur?
- main branch’inde hiç yeni commit yoksa
- Diğer branch, main’in ilerisindeyse
- Ortak geçmiş bozulmamışsa

### Basit Senaryo
```bash
A---B   (main)
     \
      C---D   (feature)

A---B---C---D   (main)
```
