# Binary-Search-Tree
Kodluyoruz Eğitimi kapsamında açtığım bir proje
Binary Search Tree (BST) oluştururken, her öğe ağaca eklenir ve her ekleme işlemi sırasında belirli kurallara uyulur: Her düğümün sol alt düğümünde ondan küçük, sağ alt düğümünde ise ondan büyük öğeler bulunur. Şimdi verilen diziyi kullanarak bir BST oluşturalım ve her adımda ağacın durumunu belirtelim:

### Adım Adım Binary Search Tree Oluşturma

1. **Root oluşturma:**
   - Root: 7

2. **5 ekle:**
   - 5, 7'den küçük olduğu için 7'nin soluna eklenir.
   ```
       7
      /
     5
   ```

3. **1 ekle:**
   - 1, 7'den küçük ve 5'ten de küçük olduğu için 5'in soluna eklenir.
   ```
       7
      /
     5
    /
   1
   ```

4. **8 ekle:**
   - 8, 7'den büyük olduğu için 7'nin sağına eklenir.
   ```
       7
      / \
     5   8
    /
   1
   ```

5. **3 ekle:**
   - 3, 7'den küçük, 5'ten küçük ama 1'den büyük olduğu için 1'in sağına eklenir.
   ```
       7
      / \
     5   8
    /
   1
    \
     3
   ```

6. **6 ekle:**
   - 6, 7'den küçük ama 5'ten büyük olduğu için 5'in sağına eklenir.
   ```
       7
      / \
     5   8
    / \
   1   6
    \
     3
   ```

7. **0 ekle:**
   - 0, 7'den, 5'ten ve 1'den küçük olduğu için 1'in soluna eklenir.
   ```
       7
      / \
     5   8
    / \
   1   6
  / \
 0   3
   ```

8. **9 ekle:**
   - 9, 7'den ve 8'den büyük olduğu için 8'in sağına eklenir.
   ```
       7
      / \
     5   8
    / \   \
   1   6   9
  / \
 0   3
   ```

9. **4 ekle:**
   - 4, 7'den küçük, 5'ten küçük, 1'den büyük ve 3'ten büyük olduğu için 3'ün sağına eklenir.
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

10. **2 ekle:**
    - 2, 7'den küçük, 5'ten küçük, 1'den büyük ve 3'ten küçük olduğu için 3'ün soluna eklenir.
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

### Sonuç

Ağacın son hali:
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

Bu adımlar diziyi bir Binary Search Tree (BST) yapısına dönüştürür. Her adımda eklenen öğe, ağaçta doğru yere yerleştirilir ve BST'nin özelliklerine uyulur.
