# Kişisel Site Taslağı — Kurulum

Bu taslak, academicpages şablonu (MIT lisanslı) üzerine ekremekc.github.io ile
aynı yapıda hazırlandı: Feed / Bio / Research / Publications / Talks / Teaching / Useful.

## 1. Repoyu oluştur
1. GitHub'da yeni repo aç, adı tam olarak: `KULLANICIADIN.github.io` (public)
2. Bu klasördeki tüm dosyaları repoya yükle (web arayüzünden sürükle-bırak
   veya `git init` + `git add .` + `git commit` + `git push`)
3. Repo > Settings > Pages > Source: **Deploy from a branch** > Branch: `master` (veya `main`), klasör `/ (root)` > Save
4. Birkaç dakika içinde site `https://KULLANICIADIN.github.io` adresinde yayında.

## 2. Doldurulacak yerler (arama yaparak bul)
- `KULLANICIADI` → GitHub kullanıcı adın (_config.yml içinde 3 yerde)
- `AD SOYAD` → görünecek ismin (_config.yml)
- `_config.yml` içinde: bio, employer (KURUM ADI), email, Google Scholar, ORCID linkleri
- `images/profile.png` → kendi fotoğrafınla değiştir (aynı isimle)

## 3. İçerik dosyaları
- Ana sayfa metni: `_pages/about.md` (TODO işaretli)
- Research sayfası üst metni: `_pages/portfolio.md`
- Useful sayfası: `_pages/useful.md`
- CV: `_pages/cv.md`
- Yayınlar: `_publications/` — içindeki örnek dosyayı kopyalayıp çoğalt
  (kategoriler: manuscripts, conferences, books, trdizin)
- Konuşmalar: `_talks/`, Dersler: `_teaching/`, Araştırma temaları: `_portfolio/`,
  Blog yazıları (Feed): `_posts/` — hepsinde format örneği olarak 1'er dosya bırakıldı.

## 4. Yerelde önizleme (isteğe bağlı)
Ruby kuruluysa: `bundle install && bundle exec jekyll serve` → http://localhost:4000
Kurulum uğraştırıyorsa gerek yok; her push sonrası GitHub otomatik derler.
