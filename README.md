# Sesli-Geri-Bildirim-Veren-Masa-st-Asistan-Robotu
🔧 Proje Tanımı

Bu proje, ESP32 mikrodenetleyici kullanılarak geliştirilen dinamik bir alarm sistemidir. Sistem; gerçek zamanlı saat takibi, OLED ekran ile görsel bildirim, buzzer ve ISD1820 ses modülü ile sesli uyarı verme yeteneklerine sahiptir. Kullanıcı, çalışma sırasında istediği kadar alarm kurabilmekte ve sistem her alarm için tek seferlik sesli/görsel bildirim sağlamaktadır.

🧰 Kullanılan Donanım Bileşenleri

ESP32 Development Board

RTC DS3231 Modülü (Gerçek Zamanlı Saat)

OLED Ekran (128x64, I2C)

Buzzer (3x kısa bip)

ISD1820 Ses Modülü (3 saniyelik ses çalar)

Breadboard ve Jumper Kablolar

🛠️ Özellikler

Gerçek zamanlı saat takibi (RTC modülü ile)

Seri port üzerinden istenildiği kadar alarm eklenebilir (örnek: 13:45)

Her alarm yalnızca bir kez tetiklenir

Alarm sırasında OLED ekranda saat görüntülenir

3x bip sesi (buzzer)

Önceden kaydedilmiş 3 saniyelik ses çalma (ISD1820)

Enerji tasarrufu: OLED ekran sadece alarm sırasında aktif

🚀 Kurulum

Arduino IDE'yi indirip kurun

Aşağıdaki kütüphaneleri yükleyin:

RTClib by Adafruit

Adafruit SSD1306

Adafruit GFX

Bağlantıları yapın:

OLED -> SDA: D21, SCL: D22, VCC: 3.3V, GND

RTC -> SDA: D21, SCL: D22, VCC: 3.3V, GND

Buzzer -> D13

ISD1820 PlayE -> D12, VCC -> 5V, GND

Kodu ESP32'ye yükleyin

Seri monitörü açın (115200 baud)

Alarm saati girin (örnek: 14:30)

🧪 Nasıl Çalışır?

RTC modülü üzerinden saat sürekli izlenir

Kullanıcıdan girilen alarmlar hafızaya alınır

Saat eşleşirse:

OLED ekranda saat görünür

Buzzer 3 bip sesi verir

ISD1820 modülü 3 saniyelik ses çalar

OLED kapanır, sistem tekrar alarm beklemeye geçer

📌 Notlar

Aynı alarm bir daha tetiklenmez

Sistem çalışırken yeni alarm eklenebilir

Sistemde buton kullanılmamıştır, tüm işlemler seri monitör ile yapılır

👩‍💻 Yazar

Demet ToyAnkara Üniversitesi, Bilgisayar ve Öğretim Teknolojileri Eğitimi📧 toydemet49@gmail.com

📄 Lisans

Bu proje açık kaynaklıdır. Dilediğiniz gibi geliştirip kullanabilirsiniz. 
