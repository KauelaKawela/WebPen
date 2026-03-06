# Web Pen 🖌️

Web Pen, tarayıcı üzerinden çalışan ve bilgisayar kamerası aracılığıyla el hareketlerinizi kullanarak ekrana çizim yapmanızı sağlayan yenilikçi bir web uygulamasıdır. Gücünü **MediaPipe Hands** kütüphanesinden alır ve gerçek zamanlı el takibi yaparak "havada çizim yapma" deneyimi sunar.

## Özellikler

- **Gerçek Zamanlı El Takibi**: Web kameranız aracılığıyla ellerinizi algılar ve işaret parmağınızın ucuyla çizim yapmanızı sağlar.
- **Geniş Renk Paleti**: Ekranın solundaki menüden veya klavye kısayollarını kullanarak farklı renkler seçebilirsiniz.
- **Ayarlanabilir Fırça Kalınlığı**: Çizimlerinizin fırça boyutunu klavye kısayollarıyla kolayca değiştirebilirsiniz.
- **Geri Al / İleri Al (Undo/Redo)**: Yaptığınız hatalı çizimleri kolayca geri veya ileri alabilirsiniz.
- **Silgi Modu**: İstemediğiniz çizgileri yakınından geçerek silebileceğiniz kullanışlı bir silgi aracı içerir.
- **Pürüzsüz Çizim (Smooth Curve)**: Çizim algoritması, noktaları birleştirirken kavisleri yumuşatarak çok daha profesyonel ve pürüzsüz çizgiler oluşturur.
- **Neon Işık Efekti (Glow)**: Çizgilerin etrafındaki hafif parlama (shadowBlur) efektiyle tasarıma şık bir hava katar.
- **İki El Desteği**: Uygulama ekranda iki eli birden algılayabilir (Ancak varsayılan olarak birincil elle çizim yapılır).

## Nasıl Çalıştırılır?

Proje tamamen istemci tarafında (tarayıcıda) çalışan tek bir HTML dosyası (`index.html`) formatındadır. Herhangi bir sunucu veya bağımlılık kurulumu gerektirmez.

1. Bu projeyi bilgisayarınıza indirin.
2. `index.html` dosyasını Google Chrome, Firefox veya Edge gibi modern bir web tarayıcısı ile açın.
3. Tarayıcınız **Kamera Erişimi** izni istediğinde **İzin Ver** seçeneğine tıklayın.
4. Kameranız açıldığında elinizi ekrana gösterin ve kısayolları kullanarak çizmeye başlayın!

*(Not: Tarayıcı güvenlik politikaları gereği yerel dosyalarda `file://` kamera erişimi bazen kısıtlanabilir. Böyle bir durumda VS Code için "Live Server" eklentisini kullanabilir veya yerel bir HTTP sunucusu başlatarak `http://localhost...` üzerinden projeyi açabilirsiniz.) ya da https://kauelakawela.github.io/WebPen adresinden deneyimleyebilirsiniz.*

## Klavye Kısayolları ve Kontroller

Çizim işlemlerini daha kolay ve hızlı yapabilmeniz için aşağıdaki klavye kısayollarını kullanabilirsiniz:

| Tuş / Kısayol | İşlev |
| :--- | :--- |
| **`Shift` (Basılı tutun)** | Ekrana çizim yapar (veya silgi modu açıksa siler) |
| **`Ctrl + Z`** | Son yapılan çizimi geri al (Undo) |
| **`Ctrl + Y`** | Geri alınan çizimi ileri al (Redo) |
| **`Space (Boşluk)`** | Tuvali (Tüm ekranı) tamamen temizle |
| **`E`** | Silgi modunu Aç / Kapat |
| **`+` (Artı)** | Fırça kalınlığını artır |
| **`-` (Eksi)** | Fırça kalınlığını azalt |
| **`1-9` ve `0`** | Hızlı renk seçimi |

## Kullanılan Teknolojiler

- **HTML5 & CSS3**: Sayfa yapısı, modern tasarım (Glassmorphism detaylar) ve animasyonlar.
- **JavaScript (Vanilla JS)**: Uygulamanın temel mantığı ve kullanıcı etkileşimleri.
- **HTML5 Canvas API**: Ekrana yüksek performanslı grafik ve çizgilerin çizilmesi.
- **[MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands.html)**: Google tarafından geliştirilen gerçek zamanlı makine öğrenimi tabanlı el takibi sistemi.
