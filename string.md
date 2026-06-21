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

literal olarak oluşturulmuş stringlerde aynı referansı gösterme olasılığı varken, new anahtar sözcüğüyle oluşturulmuş stringlerde bu yoktur.


String Değişkenleri Ardı Ardına Eklemek

+ operatörü ve concat() metodu yardımıyla.

public class App {
    public static void main(String[] args) throws Exception {
        String s="Franz" + "Kafka";
        System.out.println(s);
    }
}

Java compiler yukarıdaki kodu aşağıdakine dönüştürür.

String s=(new StringBuilder()).append("Franz").append("Kafka").toString();

Java'da string birleştirmek için stringbuilder veya stringbuffer 

Birleştirme işlemi sadece karakter dizileri değil ilkel (primitive) veri tipleri de kullanılabiliyor.


concat() ile String Değişkenleri Eklemek

public class App {
    public static void main(String[] args) throws Exception {
        String s1="Franz ";
        String s2="Kafka";
        String s3=s1.concat(s2);
        System.out.println(s3);
    }
}

Java Substring metodu
String sınıfının substring metodu, en temel metodlardan biridir.

public String substring(int startIndex)

public String substring(int startIndex, int endIndex)


public class App {
    public static void main(String[] args) throws Exception {
        String s="Fatih Özkaynak";
        System.out.println(s.substring(6));//Özkaynak 
        System.out.println(s.substring(0,5));//Fatih
    }
}



toUpperCase() ve toLowerCase() method

String s="KeReM";
System.out.println(s.toUpperCase());//KEREM
System.out.println(s.toLowerCase());//fatih
System.out.println(s);//KeReM


trim() method

String değişkeninin önündeki ve sonundaki boşlukları atar

String s=" Kerem ";
System.out.println(s);// Kerem 
System.out.println(s.trim());//Kerem


startsWith() ve endsWith() method

String s="Fatih";
System.out.println(s.startsWith("Fa"));//true
System.out.println(s.endsWith("h"));//true


charAt() method

Belirli bir indeksteki karakteri geri döndürür

String s="Fatih";
System.out.println(s.charAt(0));//F
System.out.println(s.charAt(3));//i


length() method

String s="Fatih";
System.out.println(s.length());//5


valueOf() method

Elimizdeki herhangi bir primitive veri tipini string'e dönüştürür.

int a=10;
String s=String.valueOf(a);
System.out.println(s+10);
>1010


replace() method

String s1="Java bir programlama dilidir. Java OOP paradigmasına örnek bir dildir.";
String replaceString=s1.replace("Java","C++");
System.out.println(replaceString);




CharSequence'ı bir etiket olarak düşünebiliriz.
String, StringBuilder, StringBuffer bu etiketi taşır.

Java StringBuffer class

Java StringBuffer sınıfı, değiştirilebilir string oluşturmak için kullanılır.
değişken olmanın dışında, String sınıfı ile aynıdır.
İş parçacığı (thread) için güvenlidir. StringBuffer örnek değişkeni bir thread tarafından kullanılırken diğreleri tarafından erişilemez.
Bu da çeşitli problemleri çözme konusunda avantaj sunar.

append() method

public class App {
    public static void main(String[] args) throws Exception {
        StringBuffer sb=new StringBuffer("Merhaba ");
        sb.append("Java");//orijinal string değişti
        System.out.println(sb);//Merhaba Java yazar
    }
}



insert() method

public class App {
    public static void main(String[] args) throws Exception {
        StringBuffer sb=new StringBuffer("Merhaba ");
        sb.insert(1,"Java");
        System.out.println(sb);//MJavaerhaba
    }
}



replace() method



























































