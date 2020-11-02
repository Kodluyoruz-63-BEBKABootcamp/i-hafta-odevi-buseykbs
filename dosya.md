*

# ödev1
## hesaplarım

 - (https://github.com/buseykbs)
 - (https://www.hackerrank.com/buseykbs)
 - (https://stackoverflow.com/users/story/14512062)

 ## Docker ve docker'a ait kavramlar nedir?
 ### docker nedir?
 Docker, yazılım geliştiriciler ve sistemciler için geliştirilen açık kaynaklı bir sanallaştırma platformudur. Docker ile Linux, Windows ve MacOSX üzerinde Linux ve Windows sanal containerler(makineler) çalıştırabilirsiniz. 
 ### Docker Terimleri:
 #### docker deamon:
 Hypervisor’ün dockerdaki karşılığıdır. Bütün CPU ve RAM vb gibi işletim sistemine ait işlerin yapıldığı bölümdür.
 #### conteiner nedir:
 Docker Daemon tarafından Linux çekirdeği içerisinde birbirinden izole olarak çalıştırılan process’lerin her birine verilen isimdir. Virtual Machine (Sanal Makina) analojisinde Docker’ı Hypervisor’e benzetirsek fiziksel sunucu üzerinde halihazırda koşturulmakta olan her bir işletim sisteminin (sanal sunucunun) Docker’daki karşılığı Container’dır.
 #### ımage nedir:
 Containerlar layer halindeki Image’lardan oluşur. Docker Image ise containerlara kurulacak ve run edilecek olan uygulamaların veya OS’lerin image dosyalarıdır. Örnek verecek olursak mysql, mongodb, redis, ubuntu, mariadb.. Yüzlercesi mevcut. Buyrun: Docker Images List. Fakat burada şöyle bir ayrıntı var. Aslında container içerisindeki imagelerin içeriklerinin ve tanımlamalarının gerekli tutulduğu bir dosya var. Bu dosyamızın adı: Dockerfile. Tamamen bu isimde, ne büyük ne de küçük harflerden oluşan, bir bakıma containerlar içindeki imagelerın registration’ını yapan bir dosya. Burda önemli nokta şu: Her bir image Dockerfile dediğimiz bu dosyanın altında tanımlanması zorunlu.
 #### docker registry nedir:
 Gelelim bence işin en zevkli kısmına. Tıpkı github gibi geliştiriciler açık kaynaklı olarak docker imagelerini yükleyerek ve DockerHub’ta paylaşarak imagelerin bizim de indirip kullanmamıza olanak sağlıyorlar. Kısaca imagelar Docker Registrylerde tutuluyor.
 #### Docker CLI Nedir: 
  Kullanıcının Docker Daemon ile konuşmasını sağlayan, docker komutlarının çalıştırıldığı CLI ekranıdır.
  #### Docker Compose Nedir:
   Compose, birden fazla containere sahip docker uygulamalarını tanımlamak ve çalıştırmak için kullanılır. Compose ile uygulamanızın servislerini configure etmek için bir YAML dosyası kullanılır. Ardından, tek bir komutla configure ettiğiniz ayarlar ile tüm servislerinizi oluşturup ve başlatabilirsiniz.
   (https://docs.microsoft.com/tr-tr/dotnet/architecture/microservices/container-docker-introduction/docker-terminology)
   ## .net core versiyonları ve bu versiyonlar arassındaki farklar nelerdir?
   NET Core, Microsoft ve .NET tarafından desteklenen açık kaynaklı bir gelişim platformudur.

.NET Core aşağıdaki özelliklere sahiptir:

-   Cross Platform özelliği ile çapraz platformlarda çalışabilir. Yani Windows, macOS, Linux gibi ortamlarda çalışabilmektedir. Eğer yapmak istediğiniz uygulamanın birden fazla platformda çalışmasını istiyor iseniz .NET Core ile uygulama geliştirebilirsiniz.
-   .NET Core .NET Framework, Xamarin, Mono ile .NET standart kütüphanesi nedeni ile uyumlu olarak çalışır.
-   .NET Core MIT ve Apache 2 lisansları altında yer alan açık kaynaklı bir platformdur.
-   .NET Core modüler bir yapıya sahiptir ve sadece bir uygulamada istediğiniz, ihtiyacınız olan paketleri kullanabilirsiniz. Gereksiz paketler ile uğraşmazsınız.
-   Gelişim arayüzü Command line style dediğimiz (CLI) gelişim arayüzüdür. Yani komut satırı stilidir. Desteklenen tüm platformlarda kullanılabilen komut satırı araçlarını sağlamaktadır. Böylelikle yazılımı geliştiren kullanıcılar minimum ek yüklemeler ile uygulamalarını test edebilirler ve geliştirebilirler.
-   Docker gibi teknolojilere destek sağlar.
-   .NET Core en iyi performans için tasarlanmış bir yapıya sahiptir.
-   .NET Framework veya Java aracılığı ile oluşturulmuş olan diğer mikroservislerle uyumlu olarak çalışır.
-   .NET Core aynı zamanda aynı makine üzerinde diğer .NET versiyonları ile uyumlu bir şekilde çalışma olanağı tanır. Böylelikle aynı server üzerinde çoklu hizmetleri kullanabiliriz.
-   .NET Core Microsft tarafından desteklenmektedir.

![enter image description here](https://camo.githubusercontent.com/6b3cb5a052b6dd271168ec8d24c9fd8de1796135/68747470733a2f2f692e68697a6c69726573696d2e636f6d2f456b476631652e706e67)

## Yeni versiyon .net5 'e neden geçme ihtiyacı duydu bu neyi hedefliyor)
### .net'in gelececeği( .net5 yenilikleri)
.Net Core ile platformlar arası bir geçişe başlayan Microsoft .Net 5 ile  
yeniden bir araya geliyor.

.Net dünyasını yakın zamanda bekleyen 2 büyük release vardı, .Net Core 3.0 ve .Net 5.

.Net Core 3.0 versiyonu tamamlandı, şimdi sıra .Net 5'de.

Aslında bu geçiş aşamasında .Net Core 3 ve 3.1 versiyonları bence en önemli ve en değerli versiyonlardı.Köprüden önceki son çıkış gibi düşünebilirsiniz. :)

.Net Core 3.x versiyonunda gRPC, Blazor gibi yeni özelliklerini pazara çıkartan Microsoft, benim gözlemlerim doğrultusunda oldukça başarılı oldu diyebilirim. Çünkü .Net Core 3 .Net’in en hızlı kabul gören versiyonu oldu.

Temel olarak .Net 5 ile hedeflenen, .Net Core, .Net Framework, Xamarin ve Mono’nun avantajlarını tek bir çatı altında toplamaktır.

.Net 5 ile artık tek bir .Net olacak, yani Xamarin,Unity,ML .Net dahil olmak üzere tüm framework’ler tek bir çatı altında birleşiyor.

Release tarihi olarak şu anda planlanan tarih Kasım 2020 ancak Preview versiyonları ile .Net 5'i daha yakından tanıyabiliriz.

Şimdiye kadar .Net Core için yazdığımız kütüphaneler .Net Framework’te çalışmayabiliyordu, .Net Framework ile yazılmış bir uygulamayı .Net Core’a geçirirken shared library olarak bazı tanımlamalar yapmak gerekebiliyor.  
Çözüm olarak tanımlamalarımızı .Net Standart ile geliştirmemiz gerekiyordu ancak .Net 5 ile birlikte artık tek bir Base Class Library olacak.  
Şu anda Xamarin uygulamaları Mono Base Class Library kullanırken artık .Net 5 ile .Net Core Base Class Library kullanabilecek.
(https://medium.com/devopsturkiye/net-5-ve-yenilikleri-623aae985001)

##  Markdown yazımı hakkında bilgi sahibi olunması:
Hazırladığım ödevi stackedit sitesi üzerinde markdow'a uygun gerçekleştirdim.
## Yazılım alanında takip ettiğim kişiler:
 

 1. Hakkı Sağdıç (https://github.com/hakkisagdic)
 2. Engin Demiroğlu(https://github.com/engindemirog)
 3. Atıl Samancıoğlu 
 4. mert çobanoğlu (https://github.com/cobanov)

## Microsoft azure tarafında ne gibi hizmetler var?
 
###  Uygulama Geliştirme:

 -  Azure yönetilen veritabanları
-   Geliştirme ve test
-   DevOps
-   DevSecOps
-   E-ticaret
-   Oyun geliştirme
-   Nesnelerin İnterneti
-   Hızlı uygulama geliştirme
-   Mikro hizmet uygulamaları
-   Cep Telefonu
-   Modern uygulama geliştirme
-   Sunucusuz bilgi işlem
-   Azure’daki mesajlaşma hizmetleri


### Yapay Zeka:

 - Yapay Zeka
-   Bilgi araştırma

### Buluta Geçiş:

 - .NET uygulamaları geçişi
-   Azure’a geçiş merkezi
-   Geliştirme ve test
-   Linux geçişi
-   Ana bilgisayar geçişi
-   Azure üzerinde SAP
-   SQL Server geçişi
-   Windows Server geçişi

### Veri ve Analiz:

 -  Blok zinciri
-   İş zekası
-   Bulut ölçeğinde analiz
-   Nesnelerin İnterneti
-   Daha güvenli çalışma alanı için Azure IoT
-   Akıllı alanlar için Azure IoT

### Hibrit Bulut ve Altyapı:

-   Yedekleme ve olağanüstü durum kurtarma
-   Yüksek performanslı bilgi işlem (HPC)
-   Hibrit bulut çözümleri
-   Ultra düşük gecikmeli uç bilişim
-   İş açısından kritik uygulamalar
### Güvenlik ve idare
-   Azure idaresi
-   Yedekleme ve olağanüstü durum kurtarma
-   Gizli bilgi işlem
-   Azure ağ güvenliği

###  Sektör Çözümleri

-   Enerji
-   Finansal hizmetler
-   Oyun geliştirme
-   Kamu
-   Sağlık ve yaşam bilimleri
-   Üretim
-   Medya ve eğlence
-   Perakende

(https://azure.microsoft.com/tr-tr/solutions/)

## Beğendiğiniz 5 iş ilanı:
iş ilanlarına baktım fakat hangisini buraya yazacağıma karar veremedim.Benim için iş ilanlarına bakarken dikkat edeceğim en önemli şey firmanın çalışanlarına verdiği değerdir.Bu nedenle internetten öncelikli olarak çalışan yorumlarını incelerim.İkinci olarak dikkat edeceğim husus maaş bilgisidir. Daha sonra iş yerinin konumuna dikkat ederim.
