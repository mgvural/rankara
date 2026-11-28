# rankara
## Hasta ön anketi (sürüm 1.3)

- `onanket.html`: hastanın telefonda doldurduğu, sunucusuz ve çevrimdışı çalışan anket sayfası. Bağlantıyı iPad'deki **Ayarlar > Hasta ön anketi bağlantısı** verir.
- Cevaplar telefonda iPad'in genel anahtarıyla (ECDH P-256, HKDF-SHA256, AES-256-GCM) şifrelenir; hiçbir sunucuya gitmez. Özel anahtar yalnızca iPad'de, PIN anahtarıyla şifreli durur ve yedeğe girer.
- Hasta şifreli dosyayı paylaşım menüsüyle iletir (AirDrop, Quick Share, e-posta ya da randevuda elden). Hasta sayfasındaki **Ön anketi al** dosyayı açar, dosya numarası, doğum yılı ve cinsiyeti eşleştirir; hekim önizleyip onaylayınca kaydeder.
- Yeni kayıt açılırken yanıtlar formun kendi tanımına göre süzülüp ön doldurulur (boy ve kilo hariç). Genel anahtar herkesçe bilinebildiği için dosyanın kimden geldiği kanıtlanmaz; bu yüzden onay adımı vardır.
- Kliniğe özgü bilgiler (adres, ulaşım, telefon, e-posta, KVKK iletişim) `onanket.html` içindeki `CLINIC` nesnesinde doldurulur.

## Sürüm 1.4 (28.11.2026)

- Raporu Word (.docx) olarak kaydetme; PDF düğmesi yanında.
- Spor kardiyolojisi ilk değerlendirme: lisans gruplarının açıklaması, "Yerel" yarış seçeneği kaldırıldı, en son yarış (ad, km, süre), spora göre haftalık mesafe ve süre (koşu, bisiklet, yüzme), direnç egzersizi, EK-2 muayene ve EKG bulguları ayrı, ayrıntılı özgeçmiş, sigara paket-yıl, muayenede "Diğer", sporcu EKG'sinde renk kodu (normal sarı, sınırda gri, anormal kırmızı).
- Ön anket aynı sorulara göre güncellendi; metin cevaplar da kayda ön doldurulur.
- Yeni hasta ekranında Kaydet'in yanında eksik alanlar yazılıyor.
- Yedek ve güvenlik ekranında onaylı "Tüm kayıtları sil" (PIN ve ön anket anahtarı kalır).

## Sürüm 1.5 (28.11.2026)

- Görüntüleme Laboratuvarı'na **İleri EKO** modülü (dosya no IE-0001…): hekimin "İleri Ekokardiyografi Formu"ndaki tüm bölümler (sol ventrikül, diyastol ve sol atriyum, sağ kalp, pulmoner basınç, kapaklar ve aort, sonuç ve öneri).
- Formdaki referanslara göre kırmızı işaretleme (cinsiyete göre); BSA, RWT, LV kütle indeksi, geometri önerisi, E/A, ortalama E/e′, sPAP ve TAPSE/sPAP kendiliğinden hesaplanır.

## Sürüm 1.6 (28.11.2026)

- Tüm polikliniklerde ve Görüntüleme Laboratuvarı modüllerinde raporun yanında **Özet (Word)**: kayıttaki tüm bölümler bir hekime yazılmış gibi tek paragrafta. Spor kardiyolojisi ilk değerlendirmesi için ayrıntılı anlatım; diğer formlarda bölüm bölüm özet. Rapor ekranında özetin önizlemesi var.
- Yazım: "Nabzı saatle izleme".

## Sürüm 1.7 (28.11.2026)

- Spor kardiyolojisi hekime özeti: EK-1/EK-2/EK-3 ifadeleri kaldırıldı; bulgular "saptandı / tespit edildi / ölçüldü" diliyle; kardiyak MR, koroner BT ve karar cümleleri yeniden yazıldı.

## Sürüm 1.8 (28.11.2026)

- Özetin sonunda **ÖNERİLER**: büyük harfle, numaralı, her öneri ayrı satırda. Kaynakları: son adımdaki yeni "Öneriler" kutusu (her satıra bir öneri; ilaç, tetkik, kontrol), işaretlenen istenen tetkikler, yönlendirmeler ve sonraki kontrol. Aynı öneri iki kez yazılmaz.

## Sürüm 1.9 (28.11.2026)

- Toplu test (her poliklinik ve modülde 10 kurgusal hasta) sonrası düzeltmeler: İleri EKO'da TA ve nabız ortak anahtarlarla tutulur (eski kayıtlar açılışta taşınır); veri tablosunda modülde olmayan ortak sütunlar gösterilmez; hekime özette küçük yazım düzeltmeleri (HbA1c, "/dk", tekrar eden hesap adları, eksik veri uyarıları).
