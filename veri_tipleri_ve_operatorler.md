Java programlama dilinde iki tip veri tipi bulunmaktadır.
Primitive data types: Integer, Character, Boolean, Floating Point.
Non-primitive data types: Classes, Interfaces, Arrays.

Her primitive veri mantıksal bir değer taşır.

Integer sınıfı


Java'da Operatörler

Unary, Arithmetic, Shift, Relational, Bitwise, Logical
Ternary, Assignment.

Tekil (Unary):
Sonek (postfix):
expr++ expr--

Önek (prefix):
++expr --expr +expr -expr ~ !

Aritmetik:
multiplicative: * / %
additive + -

Shift (kaydırma): << >> >>>

İlişkisel:
karşılaştırma: < > <= >= instanceof
eşitlik: == !=


Java'da her şey bir nesneydi, o halde bizim oluşturduğumuz
bir değişken de aynı zamanda bir nesne. 


Bitwise:
bitwise AND &
bitwise exclusive OR ^
bitwise inclusive OR |

Mantıksal:
logical AND &&
logical OR ||


Ternary: ? :

Atama:
assignment: = += -= *= /= %= ^= |= <<= >>= >>>=



class OperatorOrnek {
    public static voiid main(String args[]){
        int a=2;
        int b=5;
        int min=(a<b)?a:b;
        System.out.println(min);
    }
}

(a<b) doğru ise min'e a'yı ata. Değilse b'yi ata.

Çıktı:2















