# Binary Search Tree Projesi

<b>Soru :</b> [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

---
<b>Cevap :</b> Bir elemanı root olarak seçiyoruz. Sonra dizinin solundaki elemandan sağındaki elemana kadar teker teker karşılaştırıyoruz.


Dengeli bir dağılım için root olarak 7 elemanını aldım.

<b>Aşamalar:</b>

1. Dizinin solundan elemanları teker teker inceleriz.İlk olarak 7 ile 5 i karşılaştıracağız. 5, 7'den küçük olduğu için düğümün sol tarafına yazılır.
    + ```
                  7
                 /
                5

2. Sırada 1 var. 1, 7'den küçük olduğu için sola, 5 ise 7 den küçük 1 'den ise büyük olduğu için , 7 'nin soluna 5 , 5 'in de soluna 1 yazılır.
    + ```
                  7
                 /
                5
               /
              1

3. 8 sayısı, 7'den büyük olduğu için sağına yazılır.
    + ```
                  7
                 / \
                5   8
               /
              1

4. 3 sayısı, 7'den küçük olduğu için soluna, 7 'nin solundaki 5 'ten de küçük olduğu için onun da soluna ve son olarak 5 'in solundaki 1 'den büyük olduğu için 1'in sağına yazılır.
    + ```
                  7
                 / \
                5   8
               /
              1
               \
                3

5. 6 sayısı, 7'nin soluna, 7'nin solundaki 5'ten ise büyük olduğu için 5'in sağına yazılır.
    + ```
                  7
                 / \
                5   8
               / \
              1   6
               \
                3

6. 0 sayısı Binary tree'deki en küçük elemandır . Bu nedenle 0 sayısından önce en soldaki değer olan 1 'den de küçük olduğu için 1'in soluna yazılır.
    + ```
                  7
                 / \
                5   8
               / \
              1   6
             / \
            0   3

7. 9 sayısı, 7'den büyük olduğu için sağına, 8'den de büyük olduğu için 8'in sağına yazılmış olur.
    + ```
                  7
                 / \
                5   8
               / \   \
              1   6   9
             / \
            0   3

8. 4 sayısı, 7'den küçük olduğu için soluna,5'ten de küçük olduğu için onun da soluna, 1'den büyük ve aynı zamanda 1'in sağındaki 3'ten de büyük olduğu için 3'ün sağına yazılır.
    + ```
                  7
                 / \
                5   8
               / \   \
              1   6   9
             / \
            0   3
                 \
                  4

9. 2 sayısı, 7'den küçük olduğu için soluna, 5'ten de küçük olduğu için onun da soluna, 1'den büyük olduğu ancak 1'in sağındaki elemandan küçük olduğu için 1'in sağındaki eleman yani 3 sayısının soluna yazılmış olur.
    + ```
                  7
                 / \
                5   8
               / \   \
              1   6   9
             / \
            0   3
               / \
              2   4 
