<h1 align="center">MangaApp Compose</h1>

<p align="center">
  En popüler mangaları Jikan API'den çekip listeleyen ve favorilere eklemeni sağlayan Android uygulaması.<br>
  Jetpack Compose ve API kullandığım ilk proje.
</p>

<p align="center">
  <a href="https://osmnnuri.github.io"><b>Ekran görüntüleri için siteme göz at</b></a>
</p>

---

## Proje hakkında

Uygulama, Jikan API (MyAnimeList verileri) üzerinden en popüler mangaları
çeker ve kapak görselleriyle ızgara halinde listeler. Beğendiklerini
favorilerine ekleyebilirsin; favoriler cihazdaki yerel veritabanına kaydedilir
ve kimseyle paylaşılmaz.

## Özellikler

| | |
|---|---|
| **Popüler mangalar** | Kapak görseli, ad ve puanla ızgara görünümünde listeleme |
| **Sonsuz kaydırma** | Listenin sonuna gelince sonraki sayfa kendiliğinden yüklenir |
| **Arama** | Yüklenen mangalar içinde ada göre anlık arama |
| **Favoriler** | Kalp simgesiyle ekleme / çıkarma ve ayrı favoriler ekranı |
| **Yerel kayıt** | Favoriler Room ile yalnızca cihazda saklanır |
| **Yükleme durumları** | İlk yükleme ve sayfa yükleme için ayrı göstergeler |

## Nasıl çalışıyor?

```
Compose ekranları  ◄──  HomeViewModel (StateFlow)
                              │
              ┌───────────────┴───────────────┐
        Retrofit + Gson                 FavoritesRepository
        (Jikan API: /top/manga)          (Room: favori mangalar)
```

## Kullanılan teknolojiler

| Katman | Teknoloji |
|---|---|
| Dil | Kotlin |
| Arayüz | Jetpack Compose, Material 3 |
| Mimari | MVVM, StateFlow, Coroutines |
| Ağ | Retrofit, Gson, OkHttp |
| Görseller | Coil |
| Veri kaynağı | Jikan API |
| Yerel veri | Room |
| Geliştirme ortamı | Android Studio |

## Neden yaptım?

Modern Android arayüz aracı Jetpack Compose üzerinde pratik yapmak, bir API'den
sayfalı veri çekmeyi ve yerel veritabanıyla birleştirmeyi öğrenmek için.

## Kaynak kod

Kaynak kod özel bir depoda tutuluyor; inceleme için talep üzerine paylaşılabilir.

## İletişim

**osmnnuri** · [Web sitesi](https://osmnnuri.github.io) · [GitHub](https://github.com/osmnnuri) · osmannuriyasar57@gmail.com
