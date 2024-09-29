# Windows PowerShell: Kapsamlı Bir Rehber

## Giriş

Windows PowerShell, sistem yönetimi ve komut satırı arayüzünde devrim yaratmayı vaat ediyor. 
Nesne tabanlı pipeline, yönetici odaklı yapısı ve diğer Microsoft yönetim teknolojilerine geniş erişimi ile PowerShell, 
hem yöneticilerin hem de ileri düzey kullanıcıların verimliliğini önemli ölçüde artırıyor.

Yeni bir teknolojiyi öğrenirken, tanıdık olmayan özellikler ve işlevlerle karşılaşmak başlangıçta kafa karıştırıcı olabilir. 
Bu durum, Windows PowerShell'e yeni başlayan kullanıcılar için özellikle geçerlidir; çünkü bu, tam donanımlı bir komut satırı arayüzü ile ilk deneyimleri olabilir. 
Daha da kötüsü, PowerShell'in muazzam entegre script yazma yeteneklerinden haberdar olmuş olmaları ve programlama dünyasından uzak durma korkusu taşımalarıdır.

Ancak bu korkular tamamen yersizdir; PowerShell, sizinle birlikte büyüyen ve sizi kendine çeken bir shelldir. 
Şimdi, PowerShell’in sunduğu olanakları keşfetmeye başlayalım:

1. Standart Windows Komutları ile Uyumluluk

PowerShell, mevcut bilgi ve becerilerinizi tamamen göz ardı etmenizi gerektirmez. 
Standart Windows komutları ve uygulamalarıyla uyumlu çalışır.

2. Cmdlet’ler ile Gelişmiş Komut Yapısı

PowerShell, ortak bir Fiil-İsim sözdizimi paylaşan güçlü yeni bir komut türü olan cmdlet’leri tanıtır. 
Cmdlet’ler, standart komutlara göre birçok kullanılabilirlik iyileştirmesi sunar.

3. Nesne Tabanlı Çalışma

PowerShell, nesneleri doğrudan anlamaktadır. Zengin yapılandırılmış nesnelerle çalışmak, 
PowerShell komutlarını birleştirmeyi ve kullanmayı geleneksel shellerdeki düz metin dünyasına göre çok daha kolay hale getirir.

4. Yönetici Odaklı Tasarım

Tüm bu yeniliklere rağmen, PowerShell güçlü bir etkileşimli shell olarak tasarlanmıştır. 
Çalışan bir PowerShell uygulamasında komut girişi yapma deneyimi ön plandadır.

5. Keşif Desteği

Üç basit komut kullanarak, PowerShell’in sunduğu hemen her şeyi öğrenebilir ve keşfedebilirsiniz.

6. Yaygın Script Yazma İmkanları

Tam donanımlı bir script dili ile PowerShell, komut satırından doğrudan otomasyon görevlerini kolayca gerçekleştirmenizi sağlar.

7. Teknolojiler Arası Köprü

PowerShell, .NET, COM, WMI, XML ve Active Directory ile çalışma imkanı sunarak daha önce izole olan teknolojilerle çalışmayı daha kolay hale getirir.

8. Veri Depolarının Yönetimini Basitleştirir

Sağladığı sağlayıcı modeli sayesinde, PowerShell veri depolarını dosya ve klasörleri yönetmek için kullandığınız tekniklerle yönetmenizi sağlar.

# Windows PowerShell: Etkileşimli Kabuk ile Tanışın

Windows PowerShell, sistem yönetimi ve otomasyon için güçlü bir araçtır. 
Temelinde etkileşimli bir shell olarak tasarlanmış olan PowerShell, script yazma ve diğer gelişmiş özellikleri desteklese de, 
esas odak noktası kullanıcıların hızlı ve etkili bir şekilde etkileşimde bulunmasını sağlamaktır.

## PowerShell'i Başlatma

PowerShell'i başlatmak oldukça basittir. Aşağıdaki yöntemlerden birini kullanarak PowerShell'i açabilirsiniz:

- Başlat Menüsü: Başlat → Tüm Programlar → Eklentiler → Windows PowerShell.
- Çalıştır Komutu: Başlat → Çalıştır, ardından "PowerShell" yazarak Enter tuşuna basın.

Bu işlemlerden birini gerçekleştirdiğinizde, Windows XP, Windows Server 2003 ve benzeri eski sürümlerin geleneksel komut istemi penceresine oldukça benzer bir PowerShell istemi penceresi açılır.
"PS C:>" ifadesi, PowerShell'in girdi almaya hazır olduğunu gösterir.

Resim :

![Resim](https://i.ibb.co/VT6vmCz/resim-2024-09-29-213224306.png)

## Neden PowerShell?

1. Etkileşimli Shell

PowerShell, kullanıcıların komutları doğrudan girebileceği etkileşimli bir ortam sunar. 
Bu, özellikle sistem yöneticileri ve geliştiriciler için günlük görevleri hızlı bir şekilde yerine getirmeyi sağlar. 
Kullanıcılar, komutları yazarken anında geri bildirim alarak işlemlerini daha verimli hale getirebilirler.

2. Hızlı Başlangıç

PowerShell, kullanıcıların hemen verimli bir şekilde çalışmaya başlamasına olanak tanır. 
Temel komutları öğrenerek kısa sürede karmaşık görevleri yerine getirebilir ve sistem yönetimi süreçlerini otomatikleştirebilirsiniz.

3. Gelişmiş Özellikler

PowerShell, yalnızca temel komutları desteklemekle kalmaz; aynı zamanda script yazma, 
nesne tabanlı işlem yapma ve veri yönetimi gibi gelişmiş özellikler de sunar. 
Bu sayede, kullanıcılar daha karmaşık senaryoları kolayca yönetebilirler.

# Windows PowerShell ile Dosya Sistemi Navigasyonu

Windows PowerShell, kullanıcıların dosya sisteminde kolayca gezinmelerini sağlayan güçlü bir etkileşimli shell'dir. 
PowerShell'i başlattıktan sonra, hem DOS tarzı hem de Unix tarzı komutları kullanarak dosya sisteminde dolaşabilirsiniz. 
Bu yazıda, temel dosya yönetim komutları olan pushd, cd, dir, pwd ve popd komutlarının nasıl kullanılacağını inceleyeceğiz.

## Temel Komutlar

1. İlk olarak Prompt fonksiyonu ile istemin görünümünü özelleştiriyoruz.

```powershell
function Prompt { "PS > " }
```

Resim :

![Resim](https://i.ibb.co/58G46vR/resim-2024-09-29-215000396.png)

2. pushd

```powershell
pushd .
```

pushd komutu, mevcut konumu kaydeder ve belirtilen dizine geçiş yapar. 
Eğer hiçbir dizin belirtmezseniz, mevcut dizini kaydeder.

3. cd

```powershell
cd \
```

cd komutu, "change directory" anlamına gelir ve belirttiğiniz dizine geçiş yapmanızı sağlar. 
Örneğin, cd \ komutu ile root dizine dönebilirsiniz.

4. dir

```powershell
dir
```

dir komutu, mevcut dizindeki dosya ve klasörleri listelemek için kullanılır. 
Bu komut, dosyaların isimlerini, boyutlarını ve son yazılma tarihlerini gösterir.

Resim :

![Resim](https://i.ibb.co/SNTSTWL/resim-2024-09-29-215559115.png)

5. pwd

```powershell
pwd
```

pwd (print working directory) komutu, mevcut çalışma dizininizin yolunu gösterir. 
Bu, hangi dizinde bulunduğunuzu kontrol etmek için faydalıdır.

Resim :

![Resim](https://i.ibb.co/C2gG09X/resim-2024-09-29-215738825.png)

6. popd

```powershell
popd
```

popd komutu, daha önce kaydettiğiniz konuma geri dönmenizi sağlar. 
Bu, pushd ile kaydedilen konumu geri yükler.

Resim : 

![Resim](https://i.ibb.co/mtqSzbP/resim-2024-09-29-215929244.png)

Bu örnekte, ilk olarak Prompt fonksiyonu ile istemin görünümünü özelleştiriyoruz. 
Ardından pushd . komutuyla mevcut konumu kaydediyoruz. cd \ ile kök dizine geçiyoruz ve dir komutunu kullanarak dizindeki öğeleri listeliyoruz. 
Son olarak, popd ile önceki konuma geri dönüyoruz ve pwd ile mevcut dizini kontrol ediyoruz.

Ek olarak ipconfig komutu.

```powershell
ipconfig 
```

ipconfig, ağ bağlantılarınızın IP adreslerini ve diğer yapılandırma bilgilerini görüntülemek için kullanılan bir komuttur. 
PowerShell'de bu komutu çalıştırdığınızda, mevcut ağ bağlantılarınız hakkında detaylı bilgiler alırsınız. 

Örneğin:

```powershell
PS > ipconfig

Ethernet adapter Ethernet:

   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : fe20::e4a2:9371:10ea:98da%4
   IPv4 Address. . . . . . . . . . . : 192.168.1.20
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . :
```

Bu çıktıda, Ethernet adaptörünüzün DNS suffix'i, IP adresi, alt ağ maskesi ve varsayılan ağ geçidi gibi bilgiler yer almaktadır.
