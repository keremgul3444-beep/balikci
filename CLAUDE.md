# Kerem — Bağlam Dosyası

Bu dosya Claude'a beni ve çalışma şeklimi tanıtır. Oturum başında oku, çalışırken referans al.
Son güncelleme: 2 Ekim 2026.

> Bu depo herkese açık (public). Müşteri adları, iç fiyatlandırma ve maliyetler, ortaklık
> komisyonları, rezervasyon ve tahsilat verileri, altyapı güvenlik notları bilerek bu dosyaya
> konmadı. Bunlar yalnızca gizli bir depoda tutulmalı.

## 1. Ben kimim

- Adım Kerem, İstanbul'dayım. Elektrik-elektronik mühendisliği geçmişim var.
- Minoa Yachts (minoayachts.com) kurucusuyum: lüks katamaran tasarım ve üretim şirketi, 2022'de kuruldu.
- Minoa Experience (@minoaexperience, minoaexperience.com): aynı tekne üzerine kurulu premium Boğaz hospitality ve etkinlik markası.
- İki markada aynı anda creative director, operatör ve pazarlamacıyım.
- Windows kullanıyorum, Claude Code'u yerelde PowerShell'den çalıştırıyorum. Çalışma alanım `C:\AI_WORKSPACE`. Python 3.14 ve ffmpeg kurulu.
- PowerShell konsolu Türkçe kod sayfasında (cp1254): emoji basan Python scriptleri `UnicodeEncodeError` ile çöker, çözüm `PYTHONIOENCODING=utf-8`.

## 2. Nasıl çalışmak istiyorum

- Dil: Türkçe, direkt, samimi, hızlı tempo. Kısa geri bildirim döngüleri, somut çıktı. Uzun açıklama istemem.
- Marka içeriği: ünlem yok, emoji yok, klişe yok. Sofistike, kısa, duyusal, zamansız (quiet luxury). İçerik TR/EN çift dilli.
- Mevcut doküman düzenlerken orijinal format ve yerleşimi birebir koru, sadece isteneni değiştir. Kendiliğinden türetilmiş rakam veya ek yorum ekleme.
- Gerçekçilik: hoşuma gidecek değil, gerçekçi cevap ver. Düşük fiyatla büyüme önerme. Planlar tek kişi veya küçük ekiple uygulanabilir olmalı.
- Odak: konudan sapma, tek hedefe kilitli ilerle.
- Operasyon benim alanım: sahada denenmiş şeylere (ses sistemi, prova edilmiş akış, ekip kapasitesi) tekrar tekrar itiraz üretme.
- İş akışı: deploy öncesi mutlaka commit; Netlify'da önce draft, sonra `--prod`; oturum bağlamı için CLAUDE.md.

## 3. Minoa Yachts (üretici marka)

- Konumlandırma: "THE HOUSECAT – Designed for Life on Water". Yüzen ev, hafta sonu yatı değil.
- Modeller 135 ile 240 arası, amiral gemisi Minoa 170.
- Ortaklar: Volvo Penta, Franke, Bang & Olufsen, Lofrans. Teknede ses sistemi Wet Sounds.
- Marka sütunları: günlük yaşam, mühendislik, açık deniz bağımsızlığı, uzun vadeli değer.
- Marka hikâyesi: Minoa adı Minoslulardan geliyor; üretici kimliği ve yaptığımız şeyi insanlara yaşatma isteği. Üç perdeli anlatı: Minoans, builder, experience.
- Planlanan: Boğaz charter yapısı @minoacharter.
- İlk basın röportajım Klass Dergisi'nde çıktı (quiet luxury ton, EEM mühendisliğine çapalı anlatı).
- Minoa 170 teknik profil: 17,05 m boy (17 m LOA), 6,65–6,70 m en, 177 m² kullanılabilir alan, 77 m² flybridge, 2 güverte. Ticari kapasite her yerde 48 kişi olarak geçer.
- Minoa 170 dış tasarım: çift gövde, geniş dikdörtgen yaşam hacmi, koyu panoramik camlar, dış tik merdivenler, çapraz koyu destekler, geniş flybridge ve düz üst kanopi.

## 4. Minoa Experience (marka sistemi)

- Pozisyon: quiet luxury, davetle, "Reserve the Bosphorus", fiyat sadece talep üzerine. "Tekne kiralama" yerine "tahsis". Rakip dinner cruise operatörleri değil, yalı mekânları ve lüks otel alanları.
- Palet: Midnight Navy `#0d1f2d` / Warm Ivory `#f5ede0` / Champagne Gold `#c9a45a`.
- Tipografi: sitede Cormorant Garamond; teklif PDF'lerinde Lora + Poppins; içerik üretiminde EB Garamond.
- Logo: "MINOA" + altında harf aralıklı "EXPERIENCE".
- Dil repertuvarı: "Between Two Continents", "A private living room on the Bosphorus", "The view is served first", "Private dining. Open water.", "Davete açık, kalabalığa kapalı.", "Aynı su. Üç dünya.", "Bir gün. Üç ışık."
- Poster serisi: AURORA 09.30 "Şafak. Gün suda başlar.", VESPER 18.30 "Alacakaranlık. Gün altına döner.", NOX 22.00 "Gece. Sahne suyun üstünde." Üçlü poster: "İKİ KITA. ÜÇ DÜNYA."
- Program modülleri: AURORA (sabah / wellness), VESPER (sunset), NOX (gece), Privé (özel charter), MERIDIES (öğle / yüzme turu).
- İçerik kuralları: Vesper/Nox'un güncel satış durumu içerik yayınlanmadan önce benden teyit edilmeli. Tanınabilir misafirli gece partisi fotoğrafları kullanılamaz.

## 5. Dijital altyapı (genel)

- minoaexperience.com: Netlify, editoryal luxury tasarım, GSAP animasyonlar, TR/EN. Proje: `C:\AI_WORKSPACE\projects\minoa-reservation-system` (Supabase backend).
- Space deck: `C:\AI_WORKSPACE\projects\minoa-space-deck`, tek dosyalık `index.html`, m² ile anlatan animasyonlu SVG kat planı. Gerçek plan görseli altlık, render yok.
- İçerik üretim sistemi: `minoa-content/` (brand, assets, strategy, production, calendar, analytics). Hedef: profil ziyaretini rezervasyona çevirmek.
- CapCut otomasyonu: VectCutAPI, `C:\AI_WORKSPACE\VectCutAPI`. Windows notu: `claude mcp add-json` ters eğik çizgili path'leri reddediyor, düz `claude mcp add` ve `/` path kullan.

## 6. Yan projeler

- 50 m yolcu/etkinlik teknesi: değerlendirme aşamasında.
- HAVLU: arkadaşım için köpek yıkama randevu sistemi + online mağaza (Next.js + Supabase).
- The Swap File (theswapfile.com): içerik markası; Instagram, TikTok, YouTube Shorts, vidIQ.
