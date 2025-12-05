<p>Sınıf (class) soyut bir veri tipidir. Nesne (object) onun somutlaşan bir cismidir.</p>

> Sınıflar, nesnelerin templetini şablonunu taslağını oluştururlar nesneler "new" operatörü ile oluşturulmadan nesneler hayata geçmezler yani yaşamazlar yaşamayla kastımız hafızada yer kaplamalarıdır.
Java dilinde bir sınıf tasarımdır.

> Nesneler, somut kavramları tekabül ederler yani "new" operatörü ile oluşturulduklarında hafızada bir yer kapladıkları için artık yaşıyorlardır.

> Bir sınıftan bir nesne yaratan genel sözdizimi (syntax) şöyledir:
sınıf_adı   nesne adı = new     sınıf_adı();

> **sınıf adı**: nesnenin türüdür

>> örnek olarak class otomobil {} türü class olan otomobil adlı bir sınıf(class) oluşturulur. Bu türü class (sınıf) olan otomobil adından bir
nesne oluşturulduğunda da nesnenin türü (class) otomobil olur.

>> **nesne adı**: Tasarımdan (yani kasıt tanımlanan sınıftan) üretilecek olan
somut nesnenin ana bellekteki adresini işaret eder. Bu nedenle, 
*nesne adı* işaret ettiği (misal otomobil) adıymış gibi de düşünebilir.
Bundan böyle işaretçi (referans) adı ile işaret ettiği nesneyi aynı adla
anacağız.

> *=* : atama operatörü

> *new* : Sınıftan nesne yaratan operatör (nesne yaratıcı, kurucu, inşaa edici)
nesne yaratıcı (instantiate)

> *sınıf_adı()* : Yaratılacak nesnenin tasarımı

- PS (dipnot) öndeğer   default value

>> Şimdi Otomobil diye bir sınıfımız olsun ve Otomobil sınıfından bir
nesne yaratacak (kuracak) olan deyimleri açıklayalım.

> *Otomobil oto_1*;

>> derleyiciye Otomobil sınıfına ait bir nesnenin ana bellekeki adresini 
gesterecek referans bildirimidir. Referansın adı oto_1 dir. Çeşitli
kaynaklarda buna *pointer*, *gösterici*, *işaretçi*, *referans* gibi
adlar vrelir C/C++ dilindeki pointer teriminin karşılığıdır
>>> Örneğimizdeki oto_1 referansının tek ve önemli görevi *Otomobil*
sınıfına ait bir nesnenin bellekteki adresini işaret etmektir.























