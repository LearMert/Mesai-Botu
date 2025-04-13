# Discord Mesai Botu Altyapısı

Bu proje, Discord sunucularında kullanılan, buton tabanlı bir **mesai takip botunun** altyapısını içerir. Özelleştirilebilir ve kolayca geliştirilebilir yapısıyla Discord yönetiminde etkin bir mesai kontrol sistemi sunar.

## 🔧 Özellikler

- 🎯 **Giriş Butonu**: Kullanıcıların mesaiye başlamasını sağlar.
- 🛑 **Çıkış Butonu**: Kullanıcıların mesaiyi sonlandırmasını sağlar.
- 👥 **Mesai Butonu**: Aktif olarak mesaide bulunan kullanıcıları listeler.
- 📊 **Bilgilerim Butonu**: Kullanıcının geçmiş mesai verilerini gösterir.
- 🔁 **Sunucudan çıkınca otomatik mesai kapatma**: Kullanıcı sunucudan çıktığında mesaisi otomatik olarak sonlandırılır.
- 💾 **Otomatik veritabanı yedeği**: Her gün sistem tarafından veritabanı otomatik olarak yedeklenir.
- 🌐 **Sunucu bağlantısı ile kontrol**: Belirtilen FiveM sunucusuna bağlı kullanıcılar, sadece online olduklarında mesaiye giriş yapabilir.

```js
const servers = [
  {
    url: "https://servers-frontend.fivem.net/api/servers/single/977mp9",
    name: "xxx",
  },
];
```

Bu yapı, kullanıcının hedef sunucuda çevrim içi olup olmadığını doğrulamak için kullanılır.

## ⚙️ Komutlar

| Komut | Açıklama |
|-------|----------|
| `/kapat <oyuncu> <sebep>` | Belirtilen kullanıcının mesaisini sonlandırır. |
| `/kontrol` | Kullanıcıların toplam mesai sürelerini görüntüler. |
| `/mesaiekle <kullanıcı> <süre> <kanıt>` | Belirtilen kullanıcıya manuel olarak mesai süresi ekler. |
| `/mesaisil <kullanıcı> <süre>` | Kullanıcının mesai süresinden belirtilen kadarını siler. |
| `/sıfırla` | Tüm mesai kayıtlarını sıfırlar. |
| `/tümünükapat <sebep>` | Tüm kullanıcıların mesaisini belirtilen sebeple kapatır. |

## 📁 Kurulum

1. Bu projeyi bilgisayarınıza klonlayın:
   ```bash
   git clone https://github.com/LearMert/Mesai-Botu.git
   ```
2. Gerekli bağımlılıkları yükleyin:
   ```bash
   npm install
   ```
3. `config.json` veya `.env` gibi yapılandırma dosyalarını düzenleyin.
4. Botu başlatın:
   ```bash
   node index.js
   ```

## 📝 Lisans

Bu proje [MIT Lisansı](LICENSE) ile lisanslanmıştır. Detaylar için `LICENSE` dosyasına göz atabilirsiniz.

---

💬 Her türlü geri bildirim veya katkı için pull request göndermekten çekinmeyin!
