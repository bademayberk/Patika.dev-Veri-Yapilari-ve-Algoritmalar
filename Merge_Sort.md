## Soru:
***[16,21,11,8,12,22] -> Merge Sort***
***1- Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.***
***2- Big-O gösterimini yazınız.***

Merge sort türünde sıralama şu kurala göre yapılır: Dizi, ikiye bölünerek gruplara ayrılır. İkiye ayırma işlemi elemanlar tek kalana kadar devam eder. Elemanlar ayrıldıkları gruplardaki elemanlarla küçükten büyüğe doğru sıralanır. En küçük gruplar sıralandıktan sonra sıra daha büyük gruplara gelir. En sonunda dizi küçükten büyüğe doğru sıralanır. Bu soruda dizinin bu kurala göre dizilmesi ve adımların açıklanması istenmiştir.
1. adım: Dizi ikiye ayrılır.
[16, 21, 11, 8, 12, 22] --> [16, 21, 11], [8, 12, 22]
2. adım: Yeni oluşan gruplar ikiye ayrılır.
[16, 21, 11] --> [16, 21], [11]
[8, 12, 22] --> [8, 12], [22]
3. adım: Elementler tek kalana ayırma işlemi devam eder.
[16, 21] --> [16] [21]
[8, 12] --> [8] [12]
4. adım: Elementler, daha önce dahil oldukları gruplardaki elementlerle küçükten büyüğe doğru sıralanır.
[16, 21, 11] grubu [16, 21] ve [11] şeklinde ayrılıp daha sonrasında ikili olan son grup da elementlerine ayrılmıştı. Önce [16, 21] grubundaki elementler birbiri arasında sıralanır, daha sonra 11 sayısı sıralamaya dahil edilir. Aynı adımlar diğer gruplar için de geçerlidir.
Yeni sıralama adımları: [16] ve [21] --> [16, 21]. [11] dahil edildiğinde --> [11, 16, 21]
[8] ve [12] --> [8, 12]. [22] dahil edildiğinde --> [8, 12, 22]
5. adım: Gruplar birleştirilirken sıralama şu ilkeye dayanarak yapılır: Her iki grup da küçükten büyüğe sıralandığına göre dizinin en küçük elemanı, iki grubun en küçük elemanlarından biridir. Böylelikle fazladan işlem yapmaya gerek kalmaz. En küçük eleman belirlenir. Diğer elemanlar belirlenirken yine grupların en küçük elemanları sorgulanır ve dizinin elemanlarının sıralanması yapılır.
Sonuç:
```
[11, 16, 21] [8, 12, 22]
      |___________|
            |
  [8, 11, 12, 16, 21, 22]
```
Big-O Gösterimi: O(n*log2(n))