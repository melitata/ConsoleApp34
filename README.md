Extension ve Rekürsif Metotlar
Extension(Genişletilmiş) Metot Kullanımı
Extension Metotların kelime anlamı genişletilebilir metotlardır. C# 3.0 ile hayatımıza giren, aynı kodu defalarca yazmak yerine, bir kere yazıp her yerden erişebileceğimiz kolay kullanımı olan metotlardır.

Extension metot yazarken dikkat etmemiz gereken bir kaç kural vardır. Şu şekilde :

Static bir class içerisinde static bir metot olarak yazılmalılar.
Extension metod da tanımlı parametrelerden sadece 1 tanesi this ile tanımlanabilir.
Rekürsif(Yinelemeli) Metot Kullanımı
Rekürsif metotlar ilk öğrenildiğinde içselleştirilmesi ve kullanılması zor metotlardır. Ama yazılımın ilerleyen yıllarında kullanımı oturur ve bir çok soruna rekürsif metotları kullanarak çözüm getirebilirsiniz. O nedenle acele etmemek gerek :)

Çok sık olmasa da bazen fonksiyonun kendi kendini çağırmasına ihtiyaç duyarız. For döngüsü karmaşık bir kod yazarak da bu ihtiyacı karşılamak mümkün. Rekürsif fonksiyonlar ise tam da bu ihtiyaç için ortaya koyulmuştur.

Rekürsif fonksiyon kendi kendini çağırma yeteneğine sahip olduğu için kullanırken çok dikkatli olmak gerek. En büyük sorunlardan biri sonsuz döngüye neden olmalı. Bu da System.StackOverflowException olarak bilinen hataya neden olur. Yani belleğin stack bölgesinde bu fonksiyon çağrımı için ayrılan alan tükenmiştir. Yinelemeli olarak yaptığınız işe bağlı olarak risk de artar.
