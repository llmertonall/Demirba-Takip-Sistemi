# İnönü Üniversitesi Demirbaş Kontrol Sistemi

Bu sistem, İnönü Üniversitesi'nde demirbaş kayıtlarının dijital ortamda takip edilmesi için geliştirilmiştir.

## 🚀 Teknoloji Stack

### Backend

- **PHP 7.4+** - Server-side scripting
- **MySQL/MariaDB** - Database management
- **PDO** - Database abstraction layer

### Frontend

- **Bootstrap 5.3.3** - Responsive UI framework
- **FontAwesome 6.4.0** - Icon library
- **JavaScript (ES6+)** - Client-side interactions
- **CSS3** - Modern styling with gradients and animations

### Güvenlik & Performans

- **bcrypt** - Password hashing
- **PDO Prepared Statements** - SQL injection prevention
- **Input validation** - XSS protection
- **File upload security** - Secure file handling

## 📸 Sistem Görüntüleri

### Modern Login Ekranı

- Gradient arka plan tasarımı
- Responsive ve kullanıcı dostu arayüz
- İnönü Üniversitesi branding'i

### Gelişmiş Dashboard

- Collapsible sidebar navigation
- Real-time istatistikler
- Modern kart tasarımları
- Hover animasyonları

### Akıllı Demirbaş Yönetimi

- Drag & drop file upload
- Gelişmiş filtreleme sistemi
- Çoklu resim desteği
- Manuel model girişi

### Kapsamlı Log Sistemi

- Detaylı audit trail
- Filtrelenebilir log kayıtları
- Color-coded log seviyeleri

## Özellikler

### Temel Özellikler

- ✅ Kullanıcı kimlik doğrulama sistemi
- ✅ Rol tabanlı yetkilendirme (Admin/User)
- ✅ Demirbaş kayıt ekleme/düzenleme
- ✅ Gelişmiş filtreleme ve arama
- ✅ Çoklu resim yükleme
- ✅ Yazdırma ve raporlama
- ✅ İşlem geçmişi takibi
- ✅ Birim/marka/model yönetimi

### Güvenlik Özellikleri

- ✅ Şifre hashleme (bcrypt)
- ✅ SQL injection koruması (PDO)
- ✅ XSS koruması
- ✅ Dosya yükleme güvenliği
- ✅ Oturum güvenliği

## Kurulum

### Gereksinimler

- PHP 7.4 veya üstü
- MySQL/MariaDB 5.7 veya üstü
- Apache/Nginx web sunucusu
- XAMPP (yerel geliştirme için)

### Kurulum Adımları

1. **Projeyi Web Sunucusuna Kopyalayın**

   ```bash
   # XAMPP için
   C:\xampp\htdocs\DBTKınonu\
   ```

2. **Veritabanını Oluşturun**
   - phpMyAdmin'e gidin
   - `demirbas` adında veritabanı oluşturun
   - `config/db_schema.sql` dosyasını içe aktarın

3. **Başlangıç Verilerini Ekleyin**
   - `config/initial_data.sql` dosyasını çalıştırın

4. **Klasör İzinlerini Ayarlayın**

   ```bash
   chmod 755 public/uploads/
   ```

5. **Veritabanı Bağlantısını Yapılandırın**
   - `public/config.php` dosyasını kontrol edin
   - Gerekirse ayarları güncelleyin

## Kullanım

### Giriş Bilgileri

- **Yönetici:** admin / 123456
- **Kullanıcı:** user / 123456

### Ana URL

**Yerel Test Ortamı:**

```text
http://localhost/DBTKınonu/public/
```

## Dosya Yapısı

```text
DBTKınonu/
├── config/
│   └── db_schema.sql      # Veritabanı şeması
├── public/
│   ├── admin_tabs/        # Yönetici panel sekmeleri
│   ├── assets/           # CSS/JS kütüphaneleri
│   ├── css/              # Özel stiller
│   ├── img/              # Resim dosyaları
│   ├── js/               # JavaScript dosyaları
│   ├── uploads/          # Yüklenen dosyalar
│   ├── admin_panel.php   # Yönetici paneli
│   ├── asset_add.php     # Demirbaş ekleme
│   ├── assets_list.php   # Demirbaş listesi
│   ├── config.php        # Veritabanı ayarları
│   ├── dashboard.php     # Ana panel
│   ├── index.php         # Giriş yönlendirmesi
│   ├── login.php         # Giriş sayfası
│   └── logout.php        # Çıkış
└── README.md
```

## Veritabanı Tabloları

- `users` - Kullanıcı bilgileri
- `roles` - Kullanıcı rolleri
- `units` - Fakülte/Daire/Birimler
- `brands` - Markalar
- `models` - Modeller
- `asset_types` - Demirbaş türleri
- `assets` - Demirbaş kayıtları
- `asset_images` - Demirbaş resimleri
- `logs` - İşlem geçmişi

## Önemli Notlar

### Güvenlik

- Üretim ortamında güçlü şifreler kullanın
- `config.php` dosyasını web erişiminden koruyun
- Düzenli yedekleme yapın
- Güncellemeleri takip edin

### Performans

- Büyük veritabanları için indexleme yapın
- Resim dosyalarını optimize edin
- Cache mekanizması ekleyin

## Destek

Teknik destek için: [admin@inonu.edu.tr](mailto:admin@inonu.edu.tr)

## 👨‍💻 Geliştirici

### Mert Reşit ÖNAL · Embiya KIZRAK

## İLETİŞİM

- 📧 E-posta: [onalm8312@gmail.com](mailto:onalm8312@gmail.com)

- 🎓 İnönü Üniversitesi için özel olarak geliştirdi
- 💻 Full-Stack PHP Developer
- 🛠️ Modern web teknolojileri uzmanı
- 📧 İletişim: [admin@inonu.edu.tr](mailto:admin@inonu.edu.tr)

### Geliştirme Sürecinde Kullanılan Teknolojiler

- **IDE:** Visual Studio Code
- **Version Control:** Git
- **Database Design:** phpMyAdmin
- **Testing:** XAMPP Local Server
- **UI/UX:** Bootstrap 5 + Custom CSS
- **Security:** Modern PHP best practices

## 🌟 Proje Özellikleri

### ✨ Modern UI/UX

- Gradient tasarımlar ve smooth animasyonlar
- Fully responsive design (Mobile-first)
- Intuitive user interface
- Professional color scheme

### 🔐 Enterprise Security

- Role-based access control
- Secure file upload handling
- Session management
- Input validation & sanitization

### ⚡ Performance Optimized

- Optimized database queries
- Efficient file handling
- Minimal HTTP requests
- Fast loading times

## Lisans

Bu sistem İnönü Üniversitesi için özel olarak geliştirilmiştir.

### 📝 Geliştirme Notları

- **Proje Süresi:** 1 gün (yoğun geliştirme)
- **Kod Satırı:** 2000+ satır
- **Dosya Sayısı:** 15+ PHP dosyası
- **Database Tables:** 9 tablo
- **Modern Features:** Drag&Drop, Responsive Design, Real-time Stats

### 🎯 Gelecek Geliştirmeler

- [ ] QR Kod sistemi (isteğe bağlı)
- [ ] PDF raporlama (CSV yeterli şimdilik)
- [ ] Email bildirimleri (gelecekte)
- [ ] PWA özellikleri (gelecekte)

---

### © 2025 İnönü Üniversitesi - Mert Reşit ÖNAL tarafından geliştirildi

*Tüm hakları saklıdır. Bu sistem professional iş başvurusu için geliştirilmiştir.*
