# Bir Sayının Faktöriyelini Hesaplamak

## ❓ Soru
Verilen bir sayının faktöriyelini hesaplayan algoritmayı yazınız.

## ⛓ Program Kısımları
1. `n` sayısının değerini girmek.
2. Bir döngü kullanarak `n!` değerini hesaplamak.
3. `n!` değerini yazdırmak

## 👓 Çözüm Yöntemi 
- `n! = 1*2*3 …. (n-2)*(n-1)*n` veya `n! = n*(n-1)*(n-2) … 2*1` olduğu bellidir.
- `f` diye bir değişken tanımlayabiliriz, başlangıç değeri 1 olsun, ve onu 2,3 …. `n`ye kadar sayılarıyla çarpabiliriz, bunu yapmak için `i` sayacı tanımlanır 2’den `n`ye kadar değer alır (`i`nin her arttığında `x`le çarpılacak şekilde).
  
## 👩‍🔧 Çözüm Adımları
1. `i`, `f`, `n` tanımlanması.
2. `n`nin değerinin girilmesi.
3. `n!`i hesaplayan döngünün oluşturulması.
4. `f`nin değerinin yazdırılması.

## 🤖 Kod
<details>
<summary>Tıkla</summary>


```java
import java.util.*;
public class Faktoryel {
 public static void main(String arg[]) {
  Scanner input = new Scanner(System.in);
  int i, n, f = 1; // 1. adım
  System.out.print("n=");
  n = input.nextInt(); // 2. adım
  for (i = 2; i <= n; i++) // 3. adım, I. nota bak
   f = f * i; // II. nota bak
  System.out.println("n!=" + f); // 4. adım
  input.close();
 }
}
```
</details>


## 🎉 Ekran Çıktısı

```
n=5
n!=120
```

## 💡 Notlar 
1. `i=1` olduğunda sonucu etkilemeyeceği için `i=2`den başlıyoruz.
2. `f` değerini `i` sayacının değerleriyle çarpacak işlem.