# Metro Ağı Rota Bulma Sistemi

Bu proje, şehir içi metro ağında istasyonlar arası en optimal rotaları bulan gelişmiş bir Python uygulamasıdır.

## Proje Özellikleri
- Metro hatlarının ve istasyonların dinamik modellemesi
- İstasyonlar arası bağlantıların yönetimi
- En az aktarmalı rota hesaplama (BFS Algoritması)
- En hızlı rota hesaplama (Dijkstra Algoritması)
- Kapsamlı test senaryoları

## Test Senaryoları
Uygulama aşağıdaki örnek rotaları test eder:

1. AŞTİ - OSB Rotası
   - En az aktarmalı güzergah
   - En hızlı ulaşım süresi

2. Batıkent - Keçiören Rotası
   - Alternatif hat seçenekleri
   - Aktarma noktaları analizi

3. Keçiören - AŞTİ Rotası
   - Çoklu hat kullanımı
   - Optimal süre hesaplaması

## Kullanılan Algoritmalar

### En Az Aktarmalı Rota (BFS - Breadth First Search)
BFS algoritması, bir ağaç veya graf yapısında en geniş şekilde arama yapan bir algoritmadır. Bu projede şöyle çalışır:

1. Başlangıç istasyonundan başlar
2. Önce bir adım uzaklıktaki tüm istasyonları kontrol eder
3. Sonra iki adım uzaklıktaki istasyonları kontrol eder
4. Bu şekilde hedef istasyona ulaşana kadar devam eder

Avantajları:
- En kısa yolu (aktarma sayısı açısından) bulur
- Basit ve anlaşılır bir mantığı vardır
- Her zaman en az aktarmalı rotayı bulur

### En Hızlı Rota (Dijkstra Algoritması)
Dijkstra algoritması, ağırlıklı graflarda en kısa yolu bulan bir algoritmadır. Bu projede şöyle çalışır:

1. Her istasyona ulaşmak için gereken minimum süreyi hesaplar
2. Her adımda en kısa sürede ulaşılabilecek istasyonu seçer
3. Seçilen istasyondan diğer istasyonlara olan süreleri günceller


Avantajları:
- En kısa sürede ulaşımı sağlar
- Aktarma sürelerini de hesaba katar
- Alternatif rotaları değerlendirir


Çıktı:
![Ekran Görüntüsü (19)](https://github.com/user-attachments/assets/839e4075-c5cd-4af5-b09e-03eb0388b333)

