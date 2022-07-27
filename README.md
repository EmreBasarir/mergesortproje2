# Proje 2 (Merge Sort)

[16,21,11,8,12,22] -> Merge Sort

**1) Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.**

*Cevap*

[16,21,11] [8,12,22] 

Merge Sort'a göre 2'ye bölerek tek hane kalana kadar bu işleme devam etmeliyiz.

[16,21] [11] [8,12] [22] 

Tekrar 2'ye bölüyoruz tek kalan rakamları alt satıra aynen yazabiliriz.

[16] [21] [11] [8] [12] [22] 

Tek kalana kadar bölme işlemini yaptık.

[16] [11,21] [8] [12,22] 

Sıralama yaparak çifterli birleştirmeye başladık 11,21 kendi aralarında sıraladık 12,22 sıralıydı.

[11,16,21] [8,12,22] 

Tekrar birleştirdik 11,21 sıralı önce 11 ile 16'yı kıyasladık ve küçük olanı başa yazdık sonra 16 ile 21'i sıraladık, 8,12,22 zaten sıralı geldi.

[8,11,12,16,21,22] 

sol taraf ve sağ tarafın en küçüklerini kıyasladık ve küçük olanı başa yazdık 8 elendi, sonra 11 ile sağ tarafı kıyasladık 11 yazdık, 16 ile sağ tarafı kıyasladık 12 yazdık, 16 ile 22 kıyasladık 16 yazdık, kalanları da kıyasladık ve sırayla yazdık.


**2) Big-O gösterimini yazınız.**

*Cevap*

Her satırda yaptığımız işlemin time complexity 'i O(n) gelir.Bu işlemi 2^x=n x=logn kez yapıyoruz , tüm işlemleri işin içine katarsak **O(nlogn)** time complexity'e sahiptir. 


