# Genetik Algoritma ile Akıllı Depo Raf Optimizasyonu

Bu proje, Genetik Algoritma (GA) kullanılarak bir akıllı depodaki raf yüksekliği ve derinliğinin optimize edilmesini amaçlamaktadır. Belirlenen kısıtlar altında depo verim puanını maksimize eden $x_1$ ve $x_2$ değerleri hesaplanmıştır.

## Öğrenci Bilgileri
- **Ad Soyad:** [Tunahan Ata]
- **Numara:** [2212721040]
- **Senaryo:** 0 (Akıllı Depoda Raf Yüksekliği ve Derinliği Ayarı)

## Problem Tanımı

**Amaç Fonksiyonu:**
$$y = 4x_1 + 3x_2 - 0.5x_1x_2$$

**Değişkenler:**
- $x_1$: Raf yüksekliği (m) $\in [2, 6]$
- $x_2$: Raf derinliği (m) $\in [1, 4]$

**Kısıtlar:**
1. $x_1 + x_2 \le 8$ (Alan sınırı)
2. $x_2 \ge 1.5$ (Minimum derinlik)

## Kullanılan Yöntemler
Projede Python dili ve `numpy` kütüphanesi kullanılarak bir genetik algoritma sıfırdan yazılmıştır.
- **Popülasyon:** Rastgele değerlerle başlatıldı.
- **Seçilim:** Fitness değerine göre sıralama ve en iyilerin seçilmesi (Elitizm dahil).
- **Çaprazlama (Crossover):** Aritmetik ortalama yöntemi.
- **Mutasyon:** Genlere rastgele Gaussian gürültü eklenmesi.
- **Ceza Yöntemi:** Kısıtları sağlamayan bireylere -9999 fitness değeri atanarak elenmeleri sağlandı.

## Kurulum ve Çalıştırma
1. Repoyu klonlayın.
2. `ipynb` dosyasını Jupyter Notebook veya Google Colab ile açın.
3. Hücreleri çalıştırarak optimizasyon sonucunu ve grafiği görüntüleyin.
