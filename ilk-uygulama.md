class Basit {
    public static void main(String args[]){
        System.out.println("Merhaba Java");
    }    
}

class anahtar sözcüğü java'da bir sınıf bildirmek için kullanılır.

public herkes tarafından görünebileceğini bildirir, erişim düzenleyicisidir (access modifier).

static bir anahtar kelimedir, statik yöntem olarak bildirir. Java'da her şey çağrıldığında yüklenir.
main'i birdaha çağırmamıza gerek olmadığını ifade eder.

void bir şey geri göndermeyecek demektir.

main programın başlangıç noktası.

String[] args komut satırı argümanı için kullanılır.

System.out.println() yazdırma ifadesidir.



Java'da bir kod çalıştırılırken iki aşamadan geçer
1-derleme, 2-yorumlama.
derleme aşamasında yazdığımız kaynak kodumuz var. Compile ettik
ve byte kodlara dönüştürdük. Ardından Class'a dönüştü.


Runtime (Çalışma Zamanı):
classfile
classloader
bytecode verifier
interpreter
runtime
hardware (OS)

İlk başta derliyoruz, derlediğimiz zaman byte kodlara dönüşüyor, byte kodları yorumlayarak
donanım üzerinde sınıfta görmek istediğimiz çıktıları elde etmiş oluyoruz.

Java kaynak dosyasının ismi sınıf isminden farklı olabilir mi?

Evet olabilir.

Java kaynak dosyasında çoklu sınıflar olabilir.


















