# İki Sayının Tam Bölünüp Bölünmemesini Tespit Etmek

## ❓ Soru
Verilen iki sayının birbirine tam olarak bölünüp bölünemeyeceğini bulan algoritmayı yazınız. (Büyük sayı küçük sayıya bölünecek, sayıların girişteki sıraları farklı olabilir.)

## ⛓ Program Kısımları
1. “a” ve “b” değerlerini girmek.
2. “a” ile “b”yi karşılaştırmak (Gerekirse değiştirmek).
3. Birbirine bölünüp bölünmediğini öğrenmek.
4. 3.adıma göre sonuç yazdırmak.

## 👓 Çözüm Yöntemi 
- a mod b = 0 ise, “a” ve “b” tam bölündüğü bellidir.
  
## 👩‍🔧 Çözüm Adımları
1. “a”, “b”, “c” tanımlanması.
2. “a” ve “b”nin değerlerinin girilmesi.
3. Büyük sayının tespit edilmesi.

   i. “a”nın değerinin “c”de saklanması.

   ii. “b”nin değeri “a”ya atanması.

   iii. “c”de Saklanan değerinin “b”ye aktarılması.

4. Modun kontrol edilmesi:
   
   i. 0 ise “Tam Bolunebilir” yazdırılması.
   ii. 0 değilse “Tam Bolunemez” yazdırılması.

## 🤖 Kod
<details>
<summary>Tıkla</summary>


```java
import java.util.*;
public class onikinci_Program {
 public static void main(String arg[]) {
  Scanner input = new Scanner(System.in);
  int a, b, c; // 1. adım
  System.out.print("a=");
  a = input.nextInt(); // 2. adım
  System.out.print("b=");
  b = input.nextInt(); // 2. Adım
  if (a < b) // 3. adım
  {
   c = a; // 3. Adım (i) , I. nota bak
   a = b; // 3. Adım (ii)
   b = c; // 3. Adım (iii)
  }
  if (a % b == 0) // 4. Adım (i)
   System.out.println("Tam Bolunebilir");
  else // 4. Adım (ii)
   System.out.println("Tam Bolunemez");
 }
}
```
</details>


## 🎉 Ekran Çıktısı

```
a=5    b=3    Tam Bolunemez
a=2    b=6    Tam Bolunebilir
```

## 💡 Notlar 
1. a’nın değerinin kaybolmaması için geçici değişkende “c” değiştirme işleminin sırasında saklandı.
