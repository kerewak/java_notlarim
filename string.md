String, Java programlama dilindeki önemli sınıflardan biridir.
Temel olarak char elemanlar dizisini göstermek için kullanılan bir nesnedir.

Aşağıdaki iki ifade temel olarak aynıdır.
char[] ch={'f','a','t','i','h'};
String s=new String(ch);

String s="fatih";

Java programlama dilinde String sınıfı birçok kullanışlı kütüphane sunmaktadır.

compare(), concat(), equals(), split(), length(), replace(), compareTo(), intern(), substring()

Java.lang.String sınıfı Serializable, Comparable ve CharSequence arayüzleri (interfaces) ile gerçekleştirilir
(implemente edilir).


CharSequence Interface

CharSequence arabirimi, karakter dizisini temsil etmek için kullanılır.
String, StringBuffer ve StringBuilder sınıfları tarafından uygulanır.
Bu 3 sınıfı kullanarak java'da string oluşturabiliriz.


En yaygın bilinen string sınıfıdır. String sınıfının Java içerisinde önemli bir yeri vardır.

Stringler Java programlama dilinde değişmezler, immutable'dır.

String sınıfının bir nesnesini oluşturduğumuz zaman o nesneyi değiştiremeyiz. Değiştirdiğimizde yeni bir örnek değişken elde etmiş oluruz.
Değiştirilebilir string nesnelere ihtiyacımız varsa o zaman StringBuffer veya StringBuilder kullanacağız.

String oluşturmanın iki temel yöntemi vardır.

String Literal

String s = "merhaba";
String sınıfının bir s isimli örnek değişkenini oluşturduk.

JVM ilk önce String sabit havuzunu kontrol eder.
"merhaba" bu string sabit havuzu içerisinde mi? Eğer varsa yeniden bir merhaba değişkeni oluşturmuyor, belleği efektif kullanabilmek açısından.
Bu referans değişken o string sabit havuzundaki "merhaba" neresi ise orayı işaret ediyor.

Not: String nesneleri, String sabit havuzu olarak bilinen özel bir bellek alanında depolanır.

new anahtar sözcüğü ile tanımladığımız her string heap içerisinde yeni bir örnek değişken oluşturarak havuz dışarısında yeni bir bellek alanını işaret eder.


Literallerle oluşturulan o string, string sabit havuzu içerisinde yer alırken, new anahtar sözcüğü ile oluşturulan string ise heapte özel bölge oluşturarak yer ayrılır.











