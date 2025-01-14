Sinema Müşteri Kayıt Sistemi - Java Console Uygulaması

Bu proje, bir sinema müşteri kayıt sistemi uygulamasıdır. Kullanıcılar filmleri, salonları ve müşterileri ekleyebilir, kayıt işlemleri gerçekleştirebilir ve verileri JSON formatında saklayıp okuyabilirler. Proje, temel OOP prensipleri (Encapsulation, Polymorphism, Inheritance) ile geliştirilmiş ve JSON veritabanı formatı kullanılmıştır.

Özellikler

Müşteri Kayıt İşlemi: Müşteriler sisteme kaydedilir ve her müşteri benzersiz bir numara ile kaydedilir.
Film ve Salon Yönetimi: Sinemada gösterilen filmler ve salonlar sisteme eklenebilir.
Kayıtlı Müşteriler: Salonlara kayıtlı müşteriler görüntülenebilir.
Veri Saklama: Sistem, filmler, salonlar ve müşterilerle ilgili verileri JSON formatında kaydeder ve okur.
Polymorphism: Temel sınıflar ve interface kullanılarak çok biçimlilik (polymorphism) uygulanmıştır.
JSON İşlemleri: Gson kütüphanesi kullanılarak JSON formatında dosyalarla veri işlemleri yapılır.

Kullanılan Teknolojiler ve Araçlar

Java 8+
Gson Kütüphanesi (JSON işleme için)
IDE: IntelliJ IDEA / Eclipse (Tercihinize göre)

Proje Yapısı

BaseEntity - Ortak özellikleri ve davranışları tutar. Diğer sınıflar bu sınıftan türetilir.
IKayit - Kayıt işlemi için kullanılan interface. Bu interface'i Musteri sınıfı implement eder.
Film - Filmlerle ilgili bilgileri tutar (ad, süre, tür).
Salon - Sinema salonlarının bilgilerini tutar. Aynı zamanda o salonda gösterilen filmleri ve kayıtlı müşterileri içerir.
Musteri - Müşterinin bilgilerini tutar (ad, soyad, müşteri numarası).
JsonHelper - JSON dosyalarına yazma ve okuma işlemleri yapılır. Veriler bu sınıf aracılığıyla saklanır.
SinemaSistemi - Sistemin ana sınıfı, burada işlem başlatılır ve kullanıcı etkileşimi sağlanır.
