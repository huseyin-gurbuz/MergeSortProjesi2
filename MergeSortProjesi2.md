# Patika Veri Yapılar ve Algoritmalar Dersi Merge Sort Projesi



## **[16,21,11,8,12,22]** -> Merge Sort

* Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.

  Sayılar 1'er elemanlar şeklinde kalıncaya dek 2 tarafa bölünürler. Daha sonra bu tekli sayılar her adımda 2 tekli veya çoklu grubla soldan sağa küçükten büyüğe doğru sırayla birleşirilir. 

1. [16,21,11] ; [8,12,22] // ayırma işlemi başlar
1. [16,21] ; [11] ; [8,12] ; [22] // ayırma işlemi tek başlarına olana kadar devam eder
1. [16] ; [21] ; [11] ; [8] ; [12] ; [22]  // tek başlarına olana dek sayılar ayrıldı
1. [16,21] ; [8,11] ; [12,22] // burada 2'li gruplar halinde sıralı şekilde birleşir
1. [8,11,16,21] ; [12,22] // soldaki 2'li grup birleşir ve küçükten büyüğe sıralanır
1. [8,11,12,16,21,22] // son 2'li grup birleşir sıralınmış şekilde merge sort gerçekleşmiş olur.

---

- Big-O Notation

Sürekli sayı gruplarını 2'ye bölerek devam ettiğimiz için 2^x=n işleminden log(2)(n) elde ederiz ve her işlemin içinde n kere tarama yaptığımız için n*log(2)(n) bizim sonucumuzdur. 

Big-O Notation'da logaritmik olduğunu anlamamız yeterli olduğu için sonuç şudur:
$$
O(nlog(n))
$$
