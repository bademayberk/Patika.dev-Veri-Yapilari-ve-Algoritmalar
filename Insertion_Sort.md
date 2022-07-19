## Soru 1:
***[22,27,16,2,18,6] -> Insertion Sort***

***1. Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız.***

***2. Big-O gösterimini yazınız.***

***3. Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.***

***4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.***


*1.* Dizinin dizilim aşamaları:
1. İlk önce 22 ve 27 sayıları karşılaştırılır. 22, 27'den küçük olduğu için dizinin diziliminde herhangi bir değişiklik olmaz.
2. 27 ile 16 sayıları karşılaştırılır. 16 sayısı sola götürülür. Ardından en sola yerleştirilir.
3. 2 sayısı, sol tarafta kalan sayılarla karşılaştırılır. 2 karşılaştırıldığı sayıların hepsinden küçük olduğu için en sola yerleştirilir.
4. 18 sayısı karşılaştırılır, 16'nın sağına yerleştirilir.
5. En son 6 karşılaştırılır, 2'nin sağona yerleştirilir.

Dizinin her aşama sonrası dizilimi aşağıda gösterilmiştir.
```
1- [22, 27, 16, 2, 18, 6]
2- [16, 22, 27, 2, 18, 6]
3- [2, 16, 22, 27, 18, 6]
4- [2, 16, 18, 22, 27, 6]
5- [2, 6, 16, 18, 22, 27]
```
2. Big-O gösterimi:
```
Worst Case (En Kötü Senaryo) = O(n^2)
Average Case (Ortalama Durum) = O(n^2)
Best Case (En İyi Senaryo) = O(n)
```
4. Dizi sıralandıktan sonra 18 sayısı dizinin tam ortasında olacağı için average case (ortalama durum) kapsamına girer.

## Soru 2:
***[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.***
1. adım: Önce 7 ile 3 karşılaştırılır. 3 daha küçük olduğu için sol tarafa yerleştirilir.
`Dizinin yeni hali --> [3, 7, 5, 8, 2, 9, 4, 15, 6]`
2. adım: 7 ile 5 karşılaştırılır. 5 daha küçük olduğu için 3'ün sağına yerleştirilir.
`Dizinin yeni hali --> [3, 5, 7, 8, 2, 9, 4, 15, 6]`
3. adım: 8 ile 7 karşılaştırılır. 8 daha büyük olduğu için dizinin diziliminde harhangi bir değişiklik olmaz.
4. adım: 2, sol tarafındaki sayılarla karşılaştırılır. En sol tarafa yerleştirilir.
`Dizinin yeni hali --> [2, 3, 5, 7, 8, 9, 4, 15, 6]`


## Sorular Selection Sort Yöntemiyle Yapılırsa

## Soru 1:
***[22,27,16,2,18,6]***

***1- Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız.***

***2- Big-O gösterimini yazınız.***

***3- Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.***

***4- Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.***


*1.* Dizinin diziliminin aşamaları:
1. İlk önce en küçük sayı belirlenir. 2 sayısı en küçük sayı olduğu için 22 sayısı ile yer değiştirir.
2. İkinci en küçük sayı incelenir. 6 sayısı ile 27 sayısı yer değiştirir.
3. Üçüncü en küçük sayı 16 sayısı olduğu için dizinin diziliminde herhangi bir değişiklik olmaz.
4. En küçük dördüncü sayı olan 18 sayısı ile 22 sayısı yer değiştirir.
5. 22 ile 27 sayılarının konumu doğru olduğu için dizide herhangi bir değişiklik olmaz.

Dizinin her aşama sonrası dizilimi aşağıda gösterilmiştir.
```
1- [2, 27, 16, 22, 18, 6]
2- [2, 6, 16, 22, 18, 27]
3- [2, 6, 16, 22, 18, 27]
4- [2, 6, 16, 18, 22, 27]
5- [2, 6, 16, 18, 22, 27]
```
2. Big-O gösterimi:
```
Worst Case (En Kötü Senaryo) = O(n^2)
Average Case (Ortalama Durum) = O(n^2)
Best Case (En İyi Senaryo) = O(n^2)
```
4. Dizi sıralandıktan sonra 18 sayısı dizinin tam ortasında olacağı için average case (ortalama durum) kapsamına girer.

## Soru 2:
***[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.***
1. adım: Önce en küçük eleman seçilir. Bunun için tüm elemanlar incelenir. 2 sayısı dizinin en küçük elemanı olduğu için 7 sayısı ile yer değiştirir.
`Dizinin yeni hali --> [2, 3, 5, 8, 7, 9, 4, 15, 6]`
2. adım: 2. en küçük sayıyı bulmak için 2 sayısı hariç tüm sayılar incelenir. 3 sayısı en küçük 2. sayıdır ve hali hazırda 2. sırada bulunduğu için dizinin dizilimi aynı kalır.
3. adım: 3. en küçük sayı için 2 ve 3 sayıları hariç tüm sayılar incelenir. 4 sayısı en küçük 3. sayı olduğu için 5 sayısı ile yer değiştirir.
`Dizinin yeni hali --> [2, 3, 4, 8, 7, 9, 5, 15, 6]`
4. adım: 4. en küçük sayı için dizilmemiş sayılar incelenir. 5 sayısı en küçük 4. eleman olduğu için 8 sayısı ile yer değiştirir.
`Dizinin son hali --> [2, 3, 4, 5, 7, 9, 8, 15, 6]`