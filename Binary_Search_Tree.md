## Soru:
***[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.***
1. İlk olarak kök (root) değerini bularak başlayalım. Kök, 7 sayısıdır.
2. Binary-Search-Tree'de dizilim yapmanın kuralı şu şekildedir: Kök sayısını en üste yerleştirdikten sonra, eğer sıradaki sayı kök sayısından büyükse sayı sağ alt tarafa yerleştirilir. Eğer sayı, kök sayısından küçükse sol alt tarafa yerleştirilir. Bu kural diğer sayılar için de geçerlidir. Diyelim ki ikinci sıradaki sayı kök sayısından büyük. O zaman sayı sağ alt tarafa yerleştirilir. Üçüncü sırada gelen sayı kök sayısından büyük ancak diğer sayıdan küçükse sayı, ikinci sayının sol alt tarafına yerleştirilir. Dizilim bu şekilde devam eder. Bu dizide de dizilim bu kurala uyarak yapılır.
3. 7 sayısını köke yerleştirdikten sonra 5 sayısı 7 sayısının sol altına yerleştirilir. 1 sayısı hem 7'den hem de 5'ten küçük olduğu için en sol alta yerleştirilir. Kural bu şekilde uygulanmaya devam edildiğinde binary-search-tree aşağıdaki gibi olacaktır.
```
                7
               / \
              /   \
             5     8
            / \     \
           /   \     \
          1     6     9
         / \
        /   \
       0     3
            / \
           /   \
          2     4

```