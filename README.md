# ÖDEV0501: Web Programlama Eğitimindeki Engellerin Analizi ve Çözüm Sistemi

Bu proje; Bilişim Teknolojileri öğrencilerinin PHP ve sunucu taraflı web programlama eğitiminde karşılaştıkları engelleri tespit etmek, dersteki başarı ve motivasyonu artırmak amacıyla geliştirilen kademeli rehberlik/kod çalıştırma platformunun gereksinim ve analiz dokümanıdır.

---

## 📌 Problem Tanımı

Bilişim Teknolojileri öğrencileri istekli olmalarına ve okul bünyesinde donanımlı bir bilgisayar laboratuvarı bulunmasına rağmen, PHP dersinde projeleri tamamlayamamakta ve sınavlardan ortalama 45 almaktadır. 

**Temel Nedenler:**
* Dersin ağırlıklı olarak teorik ve öğretici merkezli işlenmesi,
* Kodlama mantığının ve soyut kavramların tam oturmaması,
* Hata anında anında geri bildirim alamayan öğrencilerin çekinip pasif kalması,
* İlk hatada pes edilerek projenin yarım bırakılması ve yazılıma karşı mesleki motivasyonun kaybedilmesi.

---

## 🔍 Hızlı Analiz Planı

| Yöntem | Amaç / Gerekçe |
| :--- | :--- |
| **Öğrenci Görüşmeleri** | Öğrencilerin PHP öğrenirken zorlandıkları noktaları, dersteki pasiflik ve motivasyon düşüklüğünü doğrudan kendi ifadeleriyle belirlemek. |
| **Ders ve Laboratuvar Gözlemi** | Konu aktarımını, öğrencilerin dersten koptuğu aşamaları ve uygulamalarda en çok nerede tıkandıklarını doğrudan sınıfta izlemek. |
| **Ödev ve Sınav İncelemesi** | Düşük notların somut nedenlerini ve en sık yapılan hata türlerini net verilerle tespit etmek. |

---

## ⚖️ SWOT Analizi

### Güçlü Yönler (Strengths)
* Öğrencilerin yeni teknolojileri ve kodlamayı öğrenmeye yönelik temel isteği.
* Okulda ders saatlerinde aktif olarak kullanılabilecek donanımlı bilgisayar laboratuvarının bulunması.

### Zayıf Yönler (Weaknesses)
* Dersin teorik ağırlıklı kalması ve bireysel kodlama pratiğine yeterli alan açılmaması.
* Hata yapma çekincesi ve soyut kavramların oturmaması nedeniyle öğrencilerin pasif kalması.

### Fırsatlar (Opportunities)
* PHP'nin web geliştirme ve freelance pazarındaki güçlü iş ve staj potansiyeli.
* Öğrencilere anında Türkçe hata açıklaması sunabilecek yapay zekâ araçlarının (ChatGPT, Gemini vb.) varlığı.
* HackerRank ve LeetCode benzeri rozet/seviye tabanlı mikro alıştırma platformlarıyla ders içi rekabeti eğlenceli hale getirme imkânı.

### Tehditler (Threats)
* Sunucu taraflı kodlama ve veritabanı hatalarında anlık görsel sonuç alınamadığı için öğrencilerin ilk haftalarda dersten tamamen kopması.
* Başarısızlık hissiyle yazılıma yönelik mesleki inancın yitirilmesi.

---

## 🎯 SMART Hedefler

* **Katılım ve Tamamlama:** Önümüzdeki **6 hafta içinde** derslere entegre edilecek anında geri bildirimli mikro kod alıştırmaları ile öğrencilerin derse aktif katılım ve görev tamamlama oranını **%30'dan %80'e** yükseltmek.
* **Motivasyon ve Memnuniyet:** Seviye ve rozet tabanlı alıştırma sistemi ile **6 hafta sonunda** öğrencilerin derse yönelik memnuniyet ve motivasyon anket puanını 5 üzerinden **2.5'ten 4.2'ye** çıkarmak.

---

## 📐 Proje Kapsamı

* **Kapsam İçi (In-Scope):**
  * Öğrencinin yazdığı koddaki sözdizimi ve mantık hatalarını doğrudan düzeltmek yerine, öğrenciyi adım adım doğru koda yönlendiren Türkçe ve kural tabanlı ipucu/rehber arayüzü.
* **Kapsam Dışı (Out-of-Scope):**
  * Sistemin prodüksiyona (canlıya) alınması, alan adı (domain) yönlendirmeleri, SSL sertifikasyonu ve Linux sunucu yönetimi gibi ileri düzey ağ/sunucu operasyonları.

---

## ⚙️ Sistem Gereksinimleri

### Fonksiyonel Gereksinimler
1. **Kademeli İpucu Sistemi:** Sistem, hazır kod vermek yerine hatanın mantığını açıklayan ve soru sorarak düşündüren 3 kademeli yönlendirme sunmalıdır:
   * *1. İpucu:* Mantık hatırlatması
   * *2. İpucu:* Sözdizimi örneği
   * *3. İpucu:* Çözüm yolu
2. **Tek Ekranda Anlık Derleme:** Öğrencinin yazdığı PHP kodunu ve HTML form verilerini yerel bir sunucuya ihtiyaç duymadan tarayıcı üzerinde anlık olarak çalıştırmalı; dinamik çıktıyı yan panelde göstermelidir.

### Fonksiyonel Olmayan Gereksinimler
* **Sıfır Kurulum:** Sistem, okul laboratuvarındaki bilgisayarlara yerel sunucu (XAMPP, WAMP vb.), eklenti veya yönetici (admin) yetkisi gerektirmeden standart web tarayıcılarında doğrudan çalışabilmelidir.
