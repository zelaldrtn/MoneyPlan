# Money Plan

### Finansını Yönet, Geleceğini Planla!

Money Plan, kullanıcıların kişisel finanslarını tek bir yerden yönetebilmelerini sağlayan, Flutter ve Supabase teknolojileri kullanılarak geliştirilmiş bir finans yönetimi uygulamasıdır.

Uygulama; gelir ve gider takibi, bütçe yönetimi, hesap ve kart takibi, birikim hedefleri ve finansal analiz gibi özellikleri bir araya getirerek kullanıcıların harcama alışkanlıklarını daha iyi anlamalarına ve finansal durumlarını kontrol altında tutmalarına yardımcı olur.

---

## Özellikler

### Ana Sayfa ve Finansal Özet
- Toplam varlık, borç ve kullanılabilir bakiye görüntüleme.
- Aylık gelir ve gider takibi.
- Son finansal işlemleri görüntüleme.
- Bütçe ve birikim hedeflerinin genel durumunu takip etme.
- Money Wrapped ile finansal alışkanlıkları özetleme.

### Hesap ve Kart Yönetimi
- Birden fazla finansal hesap oluşturma ve yönetme.
- Nakit ve banka bakiyelerini takip etme.
- Kredi ve banka kartlarını yönetme.
- Birden fazla para birimi desteği.

### Gelir ve Gider Takibi
- Gelir ve gider işlemleri ekleme.
- İşlemleri kategorilere ayırma.
- Finansal işlem geçmişini görüntüleme.
- Kredi kartı borç ödemelerini takip etme.

### Bütçe Yönetimi
- Aylık bütçeler oluşturma.
- Harcamaları belirlenen bütçe limitleriyle karşılaştırma.
- Bütçe kullanım oranlarını takip etme.

### Birikim Hedefleri
- Kişisel birikim hedefleri oluşturma.
- Birikim miktarını ve ilerlemeyi takip etme.
- Hedeflere ulaşma sürecini görselleştirme.

### Finansal Analiz ve Raporlama
- Gelir ve gider analizleri.
- Harcama alışkanlıklarını inceleme.
- Aylık finansal özetler.
- Finansal durum hakkında genel değerlendirmeler.

### Diğer Özellikler
- Düzenli ödeme takibi ve hatırlatmalar.
- Kullanıcı profili ve ayarlar.
- Açık ve koyu tema desteği.
- Çoklu para birimi desteği.
- Kullanıcıya özel veri yönetimi.

---

## Kullanılan Teknolojiler

| Teknoloji | Kullanım Amacı |
|---|---|
| Flutter | Çapraz platform uygulama geliştirme |
| Dart | Uygulama programlama dili |
| Supabase Auth | Kullanıcı kimlik doğrulama |
| PostgreSQL | İlişkisel veritabanı |
| Supabase RLS | Veritabanı erişim güvenliği |
| SharedPreferences | Yerel veri saklama ve önbellekleme |
| Material Design 3 | Modern kullanıcı arayüzü |

---

## Proje Yapısı

Proje, kodun daha düzenli, yönetilebilir ve geliştirilebilir olması amacıyla modüler bir yapıda oluşturulmuştur.

```text
lib/
├── main.dart
│
├── models/
│   └── ...
│
├── providers/
│   └── finance_state.dart
│
├── screens/
│   ├── home_screen.dart
│   └── tabs/
│       └── overview_tab.dart
│
├── services/
│   └── ...
│
├── theme/
│   └── app_theme.dart
│
├── utils/
│   └── ...
│
└── widgets/
    └── ...
```

---

## Veritabanı ve Backend

Money Plan, backend altyapısı olarak Supabase kullanmaktadır.

- **Supabase Authentication:** Kullanıcı kayıt ve giriş işlemleri.
- **PostgreSQL:** Kullanıcı ve finansal verilerin saklanması.
- **Row Level Security (RLS):** Kullanıcıların yalnızca yetkili oldukları verilere erişebilmesi.
- **Döviz Kurları:** Supabase üzerindeki `exchange_rates` tablosundan kur bilgilerinin alınması.
- **Yerel Önbellekleme:** Döviz kuru bilgilerinin SharedPreferences aracılığıyla yerel olarak saklanması ve gerektiğinde varsayılan değerlerin kullanılması.

---

## Kurulum

Projeyi kendi bilgisayarınızda çalıştırmak için aşağıdaki adımları takip edebilirsiniz.

### 1. Repoyu klonlayın

```bash
git clone https://github.com/zelaldrtn/MoneyPlan.git
```

### 2. Proje klasörüne gidin

```bash
cd MoneyPlan
```

### 3. Gerekli paketleri yükleyin

```bash
flutter pub get
```

### 4. Supabase yapılandırmasını yapın

Kendi Supabase projenizi oluşturun ve gerekli bağlantı bilgilerini uygulamanın yapılandırma dosyasına ekleyin.

Güvenlik açısından özel anahtarlarınızı ve servis rolü anahtarlarınızı GitHub üzerinde paylaşmayın.

### 5. Uygulamayı çalıştırın

```bash
flutter run -d chrome
```

## Geliştirme Hedefleri

- Daha kapsamlı finansal analiz ve grafikler.
- Detaylı finansal raporlama.
- Düzenli ödemeler için geliştirilmiş bildirim sistemi.
- Döviz kuru entegrasyonlarının geliştirilmesi.
- Kullanıcı deneyiminin iyileştirilmesi.
- Otomatik test kapsamının genişletilmesi.

---

## Projenin Amacı

Money Plan, Flutter ile çapraz platform uygulama geliştirme, Supabase entegrasyonu, veritabanı yönetimi, kullanıcı kimlik doğrulama ve kişisel finans yönetimi konularında pratik deneyim kazanmak amacıyla geliştirilmiştir.

Projenin temel amacı, kişisel finans yönetimini daha kolay, düzenli ve anlaşılır hâle getiren kullanıcı dostu bir uygulama sunmaktır.

---

**Flutter ve Supabase ile geliştirilmiştir.**
