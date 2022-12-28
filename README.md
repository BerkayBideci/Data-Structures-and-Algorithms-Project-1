# Veri Yapıları ve Algoritmalar | Insertion Sort & Selection Sort Projesi
- [www.patika.dev](www.patika.dev) eğitimleri kapsamında tasarlanmıştır.

---

Proje 1
[22,27,16,2,18,6] -> Insertion Sort

Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

Big-O gösterimini yazınız.

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız.

Average case: Aradığımız sayının ortada olması  
Worst case: Aradığımız sayının sonda olması  
Best case: Aradığımız sayının dizinin en başında olması.

---

1. [22,27,16,2,18,6] insertion sort uygulandığında ilk sıralanmamış elementin(unsorted) sonrasındaki elemente bakılır. Kendisinden büyükse yeri değiştirilmez ve bir sonraki sıralanmamış elemente(unsorted) geçilir. Bir sonraki sıralanmamış element(unsorted) kendisinden küçükse gerekli pozisyona alınır ve sıralanmış sayılır(sorted). Ancak sıralanmış element(sorted) insertion sort tamamlanana dek hala pozisyon değiştirebilir.  
Sonuç: [**16**,22,**27**,2,18,6]
2. İşlem hali hazırda sıralanmış pozisyonun(sorted) bir sonraki pozisyonuna(unsorted) kayarak devam eder.  
Sonuç: [**2**,**16**,22,27,18,6]
3. İşlem hali hazırda sıralanmış pozisyonun(sorted) bir sonraki pozisyonuna(unsorted) kayarak devam eder.  
Sonuç: [2,16,**18**,**22**,27,6]
4. İşlem hali hazırda sıralanmış pozisyonun(sorted) bir sonraki pozisyonuna(unsorted) kayarak devam eder ve insertion sort tamamlanır.  
Sonuç: [2,**6**,**16**,18,22,27]

- Big-O Notation = O($n^2$)
- Dizi sıralandıktan sonra 18 sayısı dizinin ortalarında bulunması sebebiyle **Time Complexity** açısından **Average Case** olarak kabul edilir.

---

[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

---

1. [7,3,5,8,2,9,4,15,6] selection sort uygulandığında en küçük element bulunur ve birinci sıradaki sıralanmamış element(unsorted) ile yeri değiştirilir. Yeri değiştirilen veya hali hazırda bulunması gereken yerde olan element sıralanmış(sorted) sayılır.  
Sonuç: [**2**,3,5,8,**7**,9,4,15,6]
2. İşlem hali hazırda sıralanmış pozisyonun(sorted) bir sonraki pozisyonuna(unsorted) kayarak devam eder. Eğer sıradaki pozisyonda bulunan element hali hazırda doğru sıradaysa sıralanmış sayılır(sorted) ve aynı kurallarla bir sonraki pozisyonuna geçer.  
Sonuç: [2,3,**4**,8,7,9,**5**,15,6]
3. İşlem hali hazırda sıralanmış pozisyonun(sorted) bir sonraki pozisyonuna(unsorted) kayarak devam eder.
Sonuç: [2,3,4,**5**,7,9,**8**,15,6]
4. İşlem hali hazırda sıralanmış pozisyonun(sorted) bir sonraki pozisyonuna(unsorted) kayarak devam eder.
Sonuç: [2,3,4,5,**6**,9,8,15,**7**]
5. Bu şekilde devam ederek selection sort tamamlanır.