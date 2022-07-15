# Veri Yapıları ve Algoritmalar Bitirme Ödevi

[patika.dev linkim](https://app.patika.dev/akslepis)

## Proje 1 - Insertion Sort

[22,27,16,2,18,6] -> Insertion Sort

1. Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.
3. Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
5. [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

### 1- Insertion Sort Aşamaları
```
[22|,27,16,2,18,6]
[22,27|,16,2,18,6]
[16,22,27|,2,18,6]
[2,16,22,27|,18,6]
[2,16,18,22,27|,6]
[2,6,16,18,22,27]
```
### 2- Big-O Gösterimi

Best case -> O($n$)

Average case -> O($n^2$)

Worse case -> O($n^2$)

### 3- Time Complexity

Average case -> [22,27,16,2,18,6]

Best case -> [2,6,16,18,22,27]

Worst case -> [27,22,18,16,6,2]

### 4- 18 Sayısı Case
```
[2,6,16,18,22,27] Dizinin sıralanmış halidir dolayısıyla 18 sayısını ele alırsak ortada olduğu için average case olur.
```
### 5- [7,3,5,8,2,9,4,15,6] Insertion Ile Ilk 4 Adımı

```
[7|,3,5,8,2,9,4,15,6]
[3,7|,5,8,2,9,4,15,6]
[3,5,7|,8,2,9,4,15,6]
[3,5,7,8|,2,9,4,15,6]
```

## Proje 2 - Merge Sort

[16,21,11,8,12,22] -> Merge Sort

1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.


### 1- Merge Sort Aşamaları

```
            [16,21,11,8,12,22]
                    |
                    v

       [16,21,11]        [8,12,22]
            |                |
            v                v  
    [16,21]   [11]    [8,12]   [22]
       |       |        |       |
       v       v        v       v 
   [16] [21]  [11]   [8] [12]  [22]
       |       |        |       |
       v       v        v       v
    [16,21]   [11]    [8,12]   [22]
            |                |
            v                v
        [11,16,21]        [8,12,22]
                     |
                     v
            [8,11,12,16,21,22] 
```

### 2- Big-O Notation Gösterimi
Worst case  -> 0(n*logn)

Average case -> 0(n*logn)

Best case -> 0(n*logn)

## Proje 3- Binary Search Tree Projesi
[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

### Binary Search Tree Aşamaları
Root 7 dir, 7'nin sağında 7 den büyük sayılar solunda 7 den küçük sayılar bulunur.

```
      7
```
```
      7
     /
    5 
```
```
      7
     /
    5
   /
  1 
```
```
      7
     / \
    5   8
   /
  1 
```
```
      7
     / \
    5   8
   /
  1
   \
    3 
```
```
      7
     / \
    5   8
   / \
  1   6 
   \
    3 
```
```
      7
     / \
    5   8
   / \
  1   6 
 / \
0   3 
```
```
      7
     / \
    5   8
   / \   \
  1   6   9
 / \
0   3 
```
```
      7
     / \
    5   8
   / \   \
  1   6   9
 / \
0   3
     \
      4 
```
```
      7
     / \
    5   8
   / \   \
  1   6   9
 / \
0   3
   / \
  2   4 
```
