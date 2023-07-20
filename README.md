# Skyrnet



Manyetik Yapı görüntülerini sınıflandırma görevine özgü bir ESA modeli geliştirmeye karar verildi.
Modelin oluşturulmasında dikkate alınan önemli faktörler arasında loss değerleri, accuracy değerleri ve karmaşıklık matrisleri bulunmaktadır.
Bu metrikler, modelin performansını ölçmek ve doğrulamak için kullanılmaktadır.
Yüksek doğruluk(accuracy), düşük hata(loss) değerleri ve dengeli bir karmaşıklık matrisi, modelin sınıflandırma görevinde başarılı olduğunu göstermektedir.
Modelin son aşamasında, özel olarak geliştirilmiş ESA modeli, transfer öğrenme ile eğitilmiş ResNet-50, Inception-v3 ve VGG-16 modelleriyle karşılaştırıldı.
Özelleştirilmiş doğruluk metrikleri ve Skyrmion görüntülerinin özgün özelliklerini öğrenme yeteneğine dayanarak, geliştirilen model, ön eğitimli modellerden daha üstün bir performans sergiledi.

Skyr-Net mimarimiz, sıralı olarak dört konvolüsyon katmanı, ardışık her bir konvolüsyon katmanının hemen ardından gelen 3x3 boyutlarında maksimum havuzlama ve %10 düşme oranı (dropout) kullanılarak tasarlanmıştır.
Konvolüsyon katmanları, birinci katmanın 11x11 boyutunda 64 filtre, ikinci katmanın 5x5 boyutunda 64 filtre ve sonraki katmanların 3x3 boyutunda 64 filtre olacak şekilde düzenlenmiştir.

