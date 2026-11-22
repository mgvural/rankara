# rankara
## Hasta ön anketi (sürüm 1.3)

- `onanket.html`: hastanın telefonda doldurduğu, sunucusuz ve çevrimdışı çalışan anket sayfası. Bağlantıyı iPad'deki **Ayarlar > Hasta ön anketi bağlantısı** verir.
- Cevaplar telefonda iPad'in genel anahtarıyla (ECDH P-256, HKDF-SHA256, AES-256-GCM) şifrelenir; hiçbir sunucuya gitmez. Özel anahtar yalnızca iPad'de, PIN anahtarıyla şifreli durur ve yedeğe girer.
- Hasta şifreli dosyayı paylaşım menüsüyle iletir (AirDrop, Quick Share, e-posta ya da randevuda elden). Hasta sayfasındaki **Ön anketi al** dosyayı açar, dosya numarası, doğum yılı ve cinsiyeti eşleştirir; hekim önizleyip onaylayınca kaydeder.
- Yeni kayıt açılırken yanıtlar formun kendi tanımına göre süzülüp ön doldurulur (boy ve kilo hariç). Genel anahtar herkesçe bilinebildiği için dosyanın kimden geldiği kanıtlanmaz; bu yüzden onay adımı vardır.
- Kliniğe özgü bilgiler (adres, ulaşım, telefon, e-posta, KVKK iletişim) `onanket.html` içindeki `CLINIC` nesnesinde doldurulur.
