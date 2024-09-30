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

# PowerShell Cmdlet'leri: Temel Bilgiler ve Kullanım

PowerShell, geleneksel Windows yürütülebilir dosyaların yanı sıra, 
cmdlet adı verilen güçlü bir komut türünü de destekler. 
Cmdlet'ler, "Verb-Noun" (Fiil-İsim) yapısında adlandırılır; örnek olarak Get-Process, Get-History ve Stop-Process verilebilir.

## Cmdlet Kullanımı

Aşağıdaki örnekte, belirli bir işlemi isimle almak için Get-Process cmdlet'ini kullanıyoruz:

```powershell
Get-Process -Name opera
```

(opera sizde yoksa opera yerine başka bir isim yazın örneğin, audiodg vb.)

Bu komut, "opera" adlı işlemin bilgilerini getirir:

```powershell
Handles  NPM(K)    PM(K)      WS(K)     CPU(s)     Id  SI ProcessName
-------  ------    -----      -----     ------     --  -- -----------
   2088      67   135800     316124      41,73   6756   1 opera
    370      24    24404     106256       1,17   9260   1 opera
    927      45   231364     188380      22,97   9324   1 opera
    355      23    16504      42420       3,95   9340   1 opera
    236      16     9728      21120       0,27   9444   1 opera
    380      25    25768      99136       0,58   9624   1 opera
    371      24    21092      96476       0,61   9692   1 opera
    537      29    50608     139152      21,31   9724   1 opera
    644      28    59336     152228       3,83   9816   1 opera
    355      23    18208      90844       0,48   9984   1 opera
    297      18     8012      21472       1,06   9992   1 opera
```


## Cmdlet'lerde Verbs (Fiiller)

PowerShell'de yaygın olarak kullanılan fiillerin (verbs) listesini öğrendiğinizde, 
yeni isimlerle (nouns) çalışmak daha kolay hale gelir. 
Örneğin, bir nesne ile çalışırken Get, Set, Start ve Stop gibi standart eylemler her zaman geçerlidir. 

## Otomatik Tamamlama ve Kısayollar

PowerShell, cmdlet ve parametre adlarını otomatik tamamlama özelliği sunar. 

Örneğin:

```powershell
Get-Pr<TAB> -N<TAB> lsass
```

Hızlı etkileşimli kullanım için, bu kadar yazmak bile fazla olabilir. 
PowerShell, yaygın komutlar için takma adlar (alias) tanımlar ve kendi takma adlarınızı oluşturmanıza da izin verir. 
Ayrıca, PowerShell'de yalnızca parametre adını yeterince yazarak belirsizliği ortadan kaldırmanız yeterlidir.
PowerShell büyük/küçük harf duyarsızdır. 

Aşağıdaki örnekte, gps takma adını kullanarak ve parametre kısaltmasını uygulayarak daha az yazabilirsiniz:

```powershell
gps -n opera
```

Resim : 

![Resim](https://i.ibb.co/XpQvNS6/Cmdlet-gps.png)

## Pozisyonel Parametreler

PowerShell, cmdlet'lerde pozisyonel parametreleri destekler. 
Pozisyonel parametreler, parametre değerlerini komut satırında belirli bir konumda sağlayarak adla belirtme zorunluluğunu ortadan kaldırır. 
Örneğin, Get-Process cmdlet'i ilk pozisyonel parametre olarak bir işlem adı alır. 

Bu parametre, joker karakterleri de destekler:

```powershell
gps o*a
```

![Resim](https://i.ibb.co/9g067jR/Gps-Cmdlet-2.png)

# PowerShell'de Derin Entegrasyon: Nesnelerle Çalışmanın Gücü

PowerShell, yapılandırılmış verileri ve zengin işlevsel nesneleri nasıl ele aldığıyla kendini göstermeye başlar. 
PowerShell'in nesne tabanlı yapısını keşfedeceğiz ve bunun nasıl etkili bir şekilde kullanılabileceğini öğreneceğiz.

## Temel Nesne Oluşturma

PowerShell'de basit bir metin dizesi oluşturmak için aşağıdaki komutu kullanabilirsiniz:

```powershell
"Merhaba!"
```

Resim :

![Resim](https://i.ibb.co/0Q2SVqx/Hello-Powershell.png)

Bu komut çalıştırıldığında, "Merhaba!" ifadesi ekrana yazdırılır. 

Örneğin, bu nesnenin Length özelliğini kullanarak kaç karakter içerdiğini öğrenebilirsiniz:

```powershell
"Merhaba!".Length
```

Resim :

![Resim](https://i.ibb.co/dW1sNTd/Powershell-lenght.png)

Sonuç olarak, 8 karakter olduğunu göreceksiniz.

## Cmdlet'ler ve Nesne Çıktısı

Tüm PowerShell komutları, çıktı olarak nesneler üretir. 
Örneğin, Get-Process cmdlet'i, bir System.Diagnostics.Process nesnesi oluşturur. 
Bu nesneyi bir değişkende saklayabilirsiniz. PowerShell'de değişken isimleri $ karakteri ile başlar. 
Eğer Notepad uygulamanız açıksa, aşağıdaki komut onu bir değişkende saklayacaktır:

```powershell
$process = Get-Process notepad
```

## Nesne Yöntemleri ile Etkileşim

Elde ettiğiniz Process nesnesi, .NET Framework'ten tam işlevsel bir nesnedir. 
Bu nesne üzerinde çeşitli işlemler gerçekleştirmek için yöntemleri çağırabilirsiniz. 
Örneğin, bir işlemi durdurmak için Kill() yöntemini kullanabilirsiniz:

```powershell
$process.Kill()
```

Resim : 

![Resim](https://i.ibb.co/6ggVrRy/Powershell-Nesne.png)

Bu örnek, Stop-Process cmdlet'inin sunduğu işlevselliği daha doğrudan gösterse de, zengin nesnelerle etkileşimde bulunma yeteneğinizi vurgular.

# PowerShell ile Yönetici İşlemleri: İlk Sınıf Kullanıcılar

PowerShell, .NET Framework'ten nesne desteği ile kullanıcılarının işlerini hızlandırırken, 
aynı zamanda yönetimsel görevler üzerine de yoğunlaşmaya devam etmektedir. 
Bu yazıda, PowerShell'in yönetimsel yeteneklerini ve sunduğu kullanışlı işlevleri keşfedeceğiz.

## Yönetimsel Sabitler: MB ve GB

PowerShell, megabayt (MB) ve gigabayt (GB) gibi standart yönetimsel sabitleri destekler. 
Örneğin, 100 GB'lık bir sabit diski CD-ROM'a yedeklemek için kaç disk gerektiğini hesaplayalım:

```powershell
100GB / 650MB
```

Bu komutun sonucu yaklaşık olarak 157,53... disk gerektirdiğini gösterir.

## Tarih ve Zaman İşlemleri

.NET Framework, geliştiriciler için bir platform olmasının yanı sıra yöneticiler için de büyük bir işlevsellik sunar. 
Örneğin, 2024 yılı bir artık yıl mı? PowerShell bu sorunun cevabını kolayca verebilir:

```powershell
[DateTime]::IsLeapYear(2024)
```

Sonuç olarak True (doğru) döner.

## Kalan Süre

Zafer bayramı tarihi olan "08/30/25" tarihine kadar ne kadar zaman kaldığını belirlemek için aşağıdaki komutları kullanabilirsiniz. 
Bu komut, belirtilen tarihi bir tarih nesnesine dönüştürür ve mevcut tarihten çıkararak kalan süreyi hesaplar:

```powershell
$result = [DateTime] "08/30/25" - [DateTime]::Now
$result.TotalDays
```

Bu işlem sonucunda, zafer bayramına kalan gün sayısını görebilirsiniz. 

