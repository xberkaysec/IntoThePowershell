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

# PowerShell'de Birleştirilebilir Komutlar

PowerShell'de, bir komut çıktısı ürettiğinde, bu çıktıyı doğrudan başka bir komuta girdi olarak iletmek için bir pipeline karakteri (|) kullanabilirsiniz. İkinci komut, ilk komut tarafından üretilen nesneleri anladığında, sonuçlar üzerinde işlem yapabilir. 
Bu şekilde birçok komutu zincirleyerek, birkaç basit işlemden güçlü bileşimler oluşturabilirsiniz.

## Örnek: Dosyaları Taşıma

Aşağıdaki komut, Path1 dizinindeki tüm öğeleri alır ve bunları Path2 dizinine taşır:

```powershell
Get-Item Path1\* | Move-Item -Destination Path2
```

## Daha Karmaşık Komutlar Oluşturma

Daha karmaşık komutlar oluşturmak için pipeline'a ek cmdlet'ler ekleyebilirsiniz. 
Aşağıdaki örnekte, ilk komut sistemde çalışan tüm süreçleri alır. 
Bu süreçler, her bir gelen öğe üzerinde bir karşılaştırma yaparak Where-Object cmdlet'ine iletilir. 
Burada karşılaştırma, ```$_.Handles -ge 500``` ifadesidir; bu ifade, mevcut nesnenin ($_ değişkeniyle temsil edilen) 
Handles özelliğinin 500 veya daha büyük olup olmadığını kontrol eder. 
Bu karşılaştırmayı sağlayan her nesne, Handles özelliğine göre sıralama yapmak için Sort-Object cmdlet'ine iletilir. 
Son olarak, nesneler Format-Table cmdlet'ine iletilerek, süreçlerin Handles, ID, Name ve Description bilgilerini içeren bir tablo oluşturulur.

## Örnek I-3: Karmaşık PowerShell Komutları

Aşağıdaki PowerShell komutu, pipeline kullanarak çeşitli cmdlet'leri birleştirerek nasıl daha karmaşık işlemler yapılabileceğini göstermektedir:

Get-Process |
Where-Object { $_.Handles -ge 500 } |
Sort-Object Handles |
Format-Table Handles, ID, Name, Description -AutoSize

Resim : 

![Resim](https://i.ibb.co/MC9P5G5/resim-2024-10-01-121730565.png)

# Kendinizi Koruma Teknikleri: PowerShell'de Güvenli Kullanım

PowerShell, güçlü komutlar ve işlevsellik sunan bir shell ortamıdır. 
Ancak, sistem bilgilerini değiştiren komutların kullanımı bazen endişe verici olabilir. 
Özellikle, aşağıdaki gibi bir komutun ne yaptığını düşünmek önemlidir:

```powershell
gps [b-t]*[c-r] | Stop-Process 
```

Bu komut, b'den t'ye kadar olan harflerle başlayan ve c'den r'ye kadar olan harflerle biten tüm süreçleri durdurmayı amaçlar. 
Peki, bu komutun ne yapacağını nasıl bilebilirsiniz? PowerShell, veri değiştiren komutlar için -WhatIf ve -Confirm parametrelerini destekler. 
Bu parametreler, bir komutun ne yapacağını önceden görmenizi sağlar.

## -WhatIf Parametresi ile Önizleme

Aşağıdaki komutu kullanarak, Stop-Process komutunun hangi süreçleri durduracağını görebilirsiniz:

```powershell
gps [b-t]*[c-r] | Stop-Process -WhatIf
```

Resim :

![Resim](https://i.ibb.co/QNZ7P1m/resim-2024-10-01-124522940.png)

Bu örnekte, -WhatIf parametresini kullanarak, Stop-Process komutunu uygulamadan önce hangi süreçlerin durdurulacağını önceden görebilirsiniz.

Bu tür teknikleri kullanarak, kendinizi koruyabilir ve sisteminizin güvenliğini artırabilirsiniz. 
Unutmayın, bilgi güçtür; doğru bilgiyi kullanmak ise güvenliğin anahtarıdır.

# PowerShell'de Yaygın Keşif Komutları

PowerShell, sistem yönetimi ve otomasyonu için güçlü bir araçtır. 
Bu yazıda, PowerShell'de sıkça kullanılan keşif komutlarını inceleyeceğiz. 
Ad hoc öğrenmenin en etkili yöntemlerinden biri, belirli bir anahtar kelime ile ilişkili komutları bulmaktır. 

## Get-Command ile Komut Bulma

Belirli bir wildcard ile eşleşen tüm komutları bulmak için Get-Command cmdlet'ini kullanabilirsiniz. 
Örneğin, "process" kelimesini içeren PowerShell komutlarını ve Windows uygulamalarını bulmak için aşağıdaki komutu kullanabilirsiniz:

```powershell
Get-Command *process*
```

Resim :

![Resim](https://i.ibb.co/djdgz2B/resim-2024-10-01-132036404.png)

## Get-Help ile Komut Açıklaması

Bir komutun ne yaptığını öğrenmek için Get-Help cmdlet'ini kullanabilirsiniz. 
Örneğin, Wait-Process komutunun detaylarını görmek için:

```powershell
Get-Help Wait-Process
```

Resim :

![Resim](https://i.ibb.co/KqqFtWW/resim-2024-10-01-132432186.png)

Bu komut, Wait-Process hakkında bilgi sağlayacaktır.

## Get-Member ile Nesne Bilgisi Alma

PowerShell, .NET Framework ile etkileşimde bulunmanıza olanak tanır. 
Bir nesnenin (örneğin, bir .NET System.String) özelliklerini ve yöntemlerini görüntülemek için Get-Member cmdlet'ini kullanabilirsiniz. 
Aşağıdaki komut, bir string nesnesinin tür adını ve üyelerini gösterir:

```powershell
"Merhaba!" | Get-Member
```

Çıktı şu şekilde olacaktır:

Resim :

![Resim](https://i.ibb.co/W5kzSMd/resim-2024-10-01-133405864.png)

PowerShell'de keşif yapmak, sistem yöneticileri ve geliştiriciler için kritik bir beceridir. Get-Command, Get-Help ve Get-Member gibi cmdlet'ler, komutları anlamanızı ve etkili bir şekilde kullanmanızı sağlar. Bu araçları kullanarak PowerShell becerilerinizi geliştirebilir ve sistem yönetimini daha verimli hale getirebilirsiniz. 

# PowerShell ile Her Yerde Komut Dosyası Yazma

PowerShell, komut satırında yazılan komutlar ile bir betikte (script) yer alan komutlar arasında hiçbir ayrım yapmaz. 
En sevdiğiniz cmdlet’ler scriptlerde çalışırken, en sevdiğiniz script teknikleri (örneğin, foreach ifadesi) doğrudan komut satırında da kullanılabilir. Aşağıdaki örnek, çalışan tüm süreçlerin (process) id sayısını toplamak için nasıl bir işlem yapabileceğinizi göstermektedir:

```powershell
$idCount = 0
foreach($process in Get-Process) { $idCount += $process.ID }
$idCount
```

Resim :

![Resim](https://i.ibb.co/M5r8Q3V/Script-PS.png)

PowerShell, koleksiyonlar hakkında istatistikler ölçmek için Measure-Object adlı bir komut sunmasına rağmen, 
bu kısa örnek, PowerShell’in genellikle ayrı bir script veya programlama diline ihtiyaç duyan teknikleri nasıl uygulamanıza izin verdiğini göstermektedir.

# .NET Framework ile Etkileşim

PowerShell, PowerShell scriptleme anahtar kelimelerinin yanı sıra, aşina olduğunuz,
.NET Framework nesneleriyle de doğrudan oluşturup çalışmanıza olanak tanır. 
PowerShell, Visual Studio’daki C# anlık moduna oldukça benzer hale gelir. 
Aşağıdaki örnek, bir web sayfasını alıp içeriğini nasıl işleyebileceğinizi göstermektedir:

```powershell
$webClient = New-Object System.Net.WebClient
$webContent = $webClient.DownloadString("http://testphp.vulnweb.com")
$webContent.Substring(0, 100)
```

Resim :

![Resim](https://i.ibb.co/SdkdXmm/Web-Client-PS.png)

# Ad Hoc Geliştirme ile PowerShell Kullanımı

PowerShell, etkileşimli yönetim ile script yazma arasındaki sınırları bulanıklaştırarak, 
kullanıcıların hızlı bir şekilde ad hoc betikler geliştirmesine olanak tanır. 
PowerShell oturumlarınızın geçmişi, bu tür geliştirmeler için mükemmel bir temel oluşturur. 
Aşağıda, PowerShell oturumunuzdaki komut geçmişini nasıl kullanabileceğinizi gösteren bir örnek bulunmaktadır.

# Komut Geçmişini Kullanarak Script Oluşturma

PowerShell'de Get-History cmdlet'ini kullanarak oturumunuzun geçmişini alabilir ve 
her bir komutun CommandLine özelliğini (yani yazdığınız komutu) yeni bir script dosyasına yazabilirsiniz. 
İşte bu süreci adım adım nasıl gerçekleştireceğiniz:

## Adım 1: Komut Geçmişini Alın

Aşağıdaki komutu kullanarak geçmişinizi alabilirsiniz:

```powershell
 Get-History | ForEach-Object { $_.CommandLine } > C:\Users\BerKolik\Desktop\Software\Betik\PowerShell\The-Powershell-1\Project\History\script.ps1
```

Resim :

![Resim](https://i.ibb.co/4WMCdVj/Get-History-PS.png)

Bu komut, oturum geçmişinizdeki her bir komutun satırını alır ve dosyaya yazar.

## Adım 2: Script Dosyasını Düzenleyin

Oluşturduğunuz betik dosyasını Notepad gibi bir metin düzenleyici ile açabilirsiniz:

```
notepad script.ps1
```

Bu aşamada, dosyadaki içeriği gözden geçirebilir ve saklamak istediğiniz komutları düzenleyebilirsiniz.

# PowerShell ile Teknolojileri Birleştirme

PowerShell, .NET Framework'ü tam anlamıyla kullanmanıza olanak tanırken, desteklediği yaygın teknolojilerle de dikkat çekiyor. 
Aşağıda, PowerShell ile XML, WMI, CIM ve COM nesneleri gibi çeşitli teknolojilerle nasıl çalışabileceğinizi gösteren örnekler bulunmaktadır.

## XML ile Çalışma

PowerShell, XML verileriyle etkileşim kurmanıza olanak tanır. 

Aşağıdaki örnekte, XML içeriğini nasıl işleyebileceğinizi görebilirsiniz:

```powershell
$xmlContent = [xml] $content
$xmlContent
$xmlContent.rss
$xmlContent.rss.channel.item | select Title
```

## WMI ve CIM ile Etkileşim

PowerShell, Windows Management Instrumentation (WMI) ve Common Information Model (CIM) ile çalışma yeteneğine sahiptir. 
Aşağıdaki örnek, BIOS bilgilerini almak için Get-CimInstance cmdlet'ini kullanmaktadır:

```powershell
Get-CimInstance Win32_Bios
```

## Active Directory ile Çalışma

PowerShell, Active Directory Service Interfaces (ADSI) ile etkileşim kurmanıza da olanak tanır. 

Aşağıdaki örnekte, yerel yöneticinin bilgilerini alabilirsiniz:


```powershell
[ADSI] "WinNT://./Administrator" | Format-List *
```

▎COM Nesneleri ile Çalışma

PowerShell, geleneksel COM nesneleri ile de çalışmanıza olanak tanır. 
Aşağıdaki örnekte, Windows Güvenlik Duvarı ayarlarını almak için bir COM nesnesi oluşturulmuştur:

```powershell
$firewall = New-Object -com HNetCfg.FwMgr
$firewall.LocalPolicy.CurrentProfile
```

Resim :

![Resim](https://i.ibb.co/mhRytdN/resim-2024-10-01-230234517.png)

# PowerShell ile Namespace Navigasyonu: Sağlam Bir Kılavuz

PowerShell, sistemle etkileşim kurmanın birçok yolunu sunar ve bunlardan biri de sağlayıcılardır.
PowerShell sağlayıcıları, veri depolarında gezinmenizi ve yönetmenizi sağlar. 
Bu, dosya sistemi ile çalışırken kullandığınız tekniklerle aynı yöntemleri kullanarak yapılabilir. 
Aşağıda, bu sağlayıcılarla nasıl çalışabileceğinizi gösteren bazı örnekler bulunmaktadır.


## Dosya Sistemi Üzerinde Gezinme

PowerShell ile dosya sisteminde gezinmek oldukça basittir. 
Aşağıdaki örnek, C: sürücüsünde nasıl gezineceğinizi göstermektedir:

```powershell
Set-Location C:\
Get-ChildItem
```

Bu komutları çalıştırdığınızda, belirtilen dizindeki dosya ve klasörlerin listesini alırsınız:

Resim :

![Resim](https://i.ibb.co/H4JHfkK/resim-2024-10-01-231452807.png)


## Kayıt Defteri Üzerinde Gezinme

PowerShell, Windows kayıt defteri üzerinde de gezinmenize olanak tanır. 
Aşağıdaki örnekte, Kayıt Defteri'nin "HKEY_CURRENT_USER\\Software\\Microsoft\\Windows" yolunda nasıl gezineceğinizi görebilirsiniz:

```powershell
Set-Location HKCU:\Software\Microsoft\Windows\
Get-ChildItem
```

Bu komutlar, belirtilen kayıt defteri anahtarındaki alt anahtarları ve değerleri listeleyecektir.

## Sertifika Deposu Üzerinde Gezinme

PowerShell, makinenizin sertifika deposu üzerinde de gezinmenize imkan tanır. 
Aşağıdaki örnek, "CurrentUser\\Root" sertifika deposunda nasıl gezineceğinizi göstermektedir:

```powershell
Set-Location cert:\CurrentUser\Root
Get-ChildItem
```

Bu komutlar çalıştırıldığında, sertifika deposundaki sertifikaların listesi görüntülenecektir.

PowerShell sağlayıcıları, sistem verilerine erişimi ve yönetimini son derece kolaylaştırır. Dosya sistemi, kayıt defteri ve sertifika deposu gibi farklı veri kaynaklarında gezinmek için aynı teknikleri kullanarak verimli bir şekilde çalışabilirsiniz.
