# AKER Proje Premium Website

GitHub -> Vercel deployment icin hazir statik web sitesi.

## Dosya yapisi

- `index.html` - Ana sayfa / TR-EN icerik
- `styles.css` - Premium responsive tasarim
- `script.js` - Dil gecisi, menu ve interaktif davranislar
- `public/assets/` - Briolight ve sayfa gorselleri
- `vercel.json` - Vercel ayarlari ve security headers
- `robots.txt`, `sitemap.xml` - SEO

## GitHub'a yukleme

```bash
git init
git add .
git commit -m "Initial AKER premium website"
git branch -M main
git remote add origin https://github.com/KULLANICI_ADI/akerproje-web.git
git push -u origin main
```

## Vercel ile yayinlama

1. Vercel Dashboard -> Add New -> Project
2. GitHub hesabini bagla.
3. `akerproje-web` reposunu sec.
4. Framework Preset: `Other`
5. Root Directory: `./`
6. Build Command: bos birak
7. Output Directory: bos birak
8. Deploy

Sonraki her `git push` otomatik deployment olusturur.

## Domain

Vercel Dashboard -> Project -> Settings -> Domains altindan:
- `akerproje.com.tr`
- `www.akerproje.com.tr`

ekleyin ve Vercel'in gosterdigi DNS kayitlarini DNS saglayicinizda uygulayin.

## Not

Mevcut AKER logo ve bazi kurumsal gorselleri mevcut AKER web sitesindeki CDN kaynagindan kullanilmaktadir. Briolight gorselleri sunumdan optimize edilerek repository icindeki `public/assets/` klasorune eklenmistir.
