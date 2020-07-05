# II Hafta (6-7 Haziran) Ödevleri 

## 6 Haziran Ödevleri:
- [x] Github'ın Gitflow'u ile diğer yaklaşımları arasındaki fark nedir? ( gitflow vs ..)
- [x] [Git and GitHub with Briana Swift](https://www.youtube.com/playlist?list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4) Youtube Listesi incelensin. (11 Video)
- [x] Merge pull request
    - [ ] Create a merge commit
    - [ ] Squash and merge 
    - [x] Rebase and merge altında ne fark var (Ödev)
- [x] issue ve #pull request de id ler neden artıyor farklı sekmeler olmasına rağmen?
- [x] [Ramp up on Git and GitHub](https://lab.github.com/githubtraining/paths/ramp-up-on-git-and-github) (ödev)
- [x] Aspnetboilerplate ve yan ürünler araştırması. [AspNet Boilerplate - Web Application Framework](https://aspnetboilerplate.com/)
- [x] hackerRank.com --> [30 Days Of Code](https://www.hackerrank.com/domains/tutorials/30-days-of-code)

## 7 Haziran Ödevleri:
- [x] Razor Pages Nedir?
- [x] 4 Farklı Projede Yapılacak *Change Authentication* :
  - [x] No Authentication
  - [x] Individual User Account
  - [x] Work or School Accounts
  - [x] Windows Authentication seçili projeler oluşturulmalı
- [x] Ayarlardaki Output kısmındaki Console Application nedir? diğerleri arasında fark nedir? [Ders Akışındaki 6. Madde'yi inceleyin.] ( araştırma ödev verildi ).
- [x] c# json serialize / deserialize
- [x] MVC vs MVVM
   - [x] MVP vs MVW vs MVU Pattern arasındaki farkı araştır
   - [x] Model-View-Update (MVU) nedir?




### Github Flow ve GitFlow
Repo içerisinde linkten ulaşabilirsiniz.

[GitFlow - GitHub Flow](https://github.com/Kodluyoruz51BootcampMVCCore/ii-hafta-odevi-hsynkrcf/blob/master/gitflow-vs-githubflow.md)

## Rebase And Merge

Rebasing ve Merging bir daldaki değişiklikleri başka bir dalda ancak farklı şekillerde entegre etmek için tasarlanmıştır.

![Rebase Commit Merge](https://miro.medium.com/max/1400/1*pzT4KMiZDOFsMOKH-cJjfQ.png)

- When you do rebase a feature branch onto master, you move the base of the feature branch to master branch’s ending point.
- Merging takes the contents of the feature branch and integrates it with the master branch. As a result, only the master branch is changed. The feature branch history remains same.
- Merging adds a new commit to your history.

## İssues ve Pull Request

Açıklayıcı ve örnekleyici birşey bulamadım ama elimde bir link var :)
https://developer.github.com/v3/issues/

## ASP.NET BoilerPlate

ASP.NET Boilerplate, “her şirket tek tek uğraşmasın, tüm .NET developer’lar için ortak bir framework geliştirelim” hedefiyle ortaya çıkmış açık kaynak kodlu, iyi dokümante edilmiş bir projedir. Sadece framework değil, modern uygulamalar için DDD(Domain Driven Design) tekniklerini baz alan sağlam bir mimari ve model sunar.
- Şirketin yan ürünleri için --> https://volosoft.com/open-source

## HackerRank 

HackerRank biz developerlar arasında, hepimiz kullanmasakta illaki duymuşuzdur. Önce kendi profil linkimi bırakayım.
- https://www.hackerrank.com/hsynkrcf  :+1:
- Yurtdışında iş görüşmelerinde mutlaka istiyorlarmış diye birşey duymuştum. Girdim 3 saat boyunca algoritma çözmeye çalıştım fakat öylece bıraktım.
- Boş vakitlerimde bu siteye uğramayı seviyorum, hem kendinizi geliştirirsiniz hem de cv'nize katkı sağlar. :)

## RazorPage Nedir ?

Razor Pages, ASP.NET Core 2 ile birlikte gelen yeni bir özellik. Daha önce kullandığımız ASP.NET Web forms çatısına yaklaşım olarak benzemekle birlikte klasik ASP.NET Webforms’u kullanmadan ASP.NET mvc üzerine geliştirilmiştir. Razor Pages, sayfa bazlı senaryolar için bildiğimiz mvc (model view controller)’a göre daha kolay uygulama geliştirmeyi sağlayan bir platformdur. Frontend çatılarda kullanılan yaklaşım olan mvvm (model view view model) yapısına benzeşen çift yönlü bağlantı (two way binding) özelliğini desteklemektedir.

[Buradan Detaylı İnceleyebilirsiniz](https://www.onbirkod.com/webformsun-yeniden-dogusu-razor-pages)

## JSON Serialize - Deserialize ?

Geldik sevdiğim konulara hemen kendi yaptığım serilize repomun linkini bırakayım. :shipit:
- https://github.com/hsynkrcf/MySerializationDLL
- Kısaca elimizdeki verileri internet üzerinden protokoller ile bir yerden bir yere taşımak için kullanırız.

#### .Net Framework ile Serileştirme
Serileştirme işlemini ve serileştirilmiş nesneleri dönüştürme işlemini gerçekleştirecek olan nesneler, System.Net.Runtime.Serialization ad uzayında bulunmaktadır. Serialization işlemi, bir nesneyi, depolamak veya serileştirmek amacıyla istenen formata dönüştürme işlemidir. Deserialization ise serileştirilmiş biçimdeki verilerin tekrar nesnelere dönüştürülmesi işlemidir. Örneğin, network ortamında bir bilgisayardan başka bir bilgisayara veri transferi gerçekleştirmek için önce bağlantı kurulur, ardından gönderilecek olan nesne oluşturduğumuz uygulama tarafından serileştirilir, daha sonra uzak bilgisayardaki uygulama tarafından deserialization işlemi ile aktarılan veri anlamlı bir nesneye dönüştürülür. Türleri Şunlardır.

1. Binary Serialization
2. SOAP Serialization
3. JSON Serialization

## MVC vs MVP vs MVVM
MVC (Model-View-Controller), MVP (Model-View-Presenter) ve MVVM (Model-View-View Model) patternlerinin oluşmasının arkasında yatan temel motivasyon aslında az öncede bahsettiğim gibi hem Separation of Concerns prensibini uygulamak hemde kolay bir şekilde Unit Test yazılmasına olanak sağlamak, yani Test Driven Development (TTD) yöntemini uygulayabilmek. Bazı durumlarda da reusibility’i arttırabiliyor tabi, çünkü bu patternleri uyguladığımız zaman ufak değişiklerle, alt yapımızı koruyarak uygulamımın farklı platformlarda (Windows Forms, Asp.NET, WPF …) çalışmasını sağlayabiliyoruz yani UI bağımsız uygulamalar geliştirebiliyoruz.

### MVC (Model-View-Controller)
Controller kullanıcıdan gelen inputları karşılar, ayrıca UI ile ilgili bütün akışı yönetir ve kararları verir. Controller View hakkında hiç birşey bilmez ama View Controller’ı bilir. Görüldüğü üzere Controller ile View arasında 1-n bir ilişki var yani bir Controller birden fazla View tarafından kullanılabilir. Controller kullanıcıdan gelen inputlar doğrultusunda Model üzerinde değişikleri yapar, Model değiştiğini View’e notify eder yani View ile Model arasında Observer ilişkisi var. View, Model’e register olur, görüldüğü üzere bir model’e birden fazla View register olabilir. Aralarında ki observer ilişkisi sayesinde, Model’deki herangi bir değişiklik ona register olmuş bütün View’lere yansır.

MVC’nin en büyük avantajı sorumlulukları Model,View ve Controller’a temiz bir şekilde dağıtmasıdır. Controller’lar uygulamanın akışını kontrol ederler, nerede neyin nasıl yapılmasına gerektiğine karar verirler. View sadece kendisinin nasıl update olacağına ilişkin business’ı içerir, Model’i oluşturur ve kullanıcıya gösterir. View uygulamayla ilgili hiç bir logic içermediğinden dolayı farklı platformlar (Windows, Web) için aynı controller’ı kullanan birden fazla View olabilir.

### MVP (Model-View-Presenter)
MVP Pattern’i aslında MVC’den evrilmiş bir pattern, sadece bağımlılıklar değişiyor ve Controller’ın yerine Prenseter (ki bu durumda kendisine hala Controller denebiliyor) geliyor.

İnputları direk View karşılıyor, modern programlama ortamlarının mantığına daha uygun. View Presenter’ını biliyor, Presenter ise View’i bir interface aracılığıyla biliyor aralarında bir abstraction var. Ayrıca MVC’nin aksine View ile Presenter arasında 1–1 ilişki var. Presenter Model’i manipule ediyor, Model’in değişikleri Presenter’a notify etme durumu birazcık tartışmalı, etmeyedebilir, Presenter ilgili değişikliği yapıp, View’i kendisi güncelleyebilir. Zaten buradaki en büyük fark MVC’nin aksine Presenter’ın View’i bir interface aracılığıyla kendisinin güncellemesi, View burada Presenter’a interface aracılığıyla istediği bilgiyi açabilir, ister Textbox’ın Text’i olsun ister Buton’ın Enabled’ı olsun. Presenter View’in nasıl bir View, Web mi? Windows mu? olduğuyla ilgilenmiyor, sadece data akışıyla ilgili ne yapması gerektiğini, View’den gelen etkileşimleri nasıl karşılaması gerektiğini ve View’de nasıl değişikler yapması gerektğini biliyor. Yani Prensenter’ımız burada karar mekanizaması rölünü üstleniyor.

### MVVM (Model-View-ViewModel)
MVVM Pattern’i hakkında bilgi vermeden önce Presentation Model hakkında bilgi vermek istiyorum. Çünkü MVVM dediğimiz şeye; WPF ve Silverlight için Prensentation Model diyebiliriz.

MVVM birazcık MVP’yi andırıyor fakat buradaki fark, Presentation Model hem View ile ilgili stateleri tutuyor hemde View hakkında hiç birşey bilmiyor. Aslında PM View’in state ve davranışlarıyla ilgili bilgiyi kendi üzerine alıyor ve Business Layer ile arasındaki kordinasyonu sağlıyor ve View’e karar vermeyle ilgili çok az şey bırakıyor. View yine stateleri tutuyor aslında. Fakat MVP’nin aksine Presentation Model View ile ilgili hiç bir bilgiye ihtiyaç duymuyor, bu yüzden ki View ile PM arasında 1-n bir ilişki var, bir PM birden fazla View’de kullanılabiliyor, bu kısmıyla MVC’ye benziyor, fakat MVC’nin aksine View üzerinde ki manipulasyonlar PM üzerinden gerçekleşiyor. Aslında şöylede bakabiliriz, PM ile View arasında yine bir observer ilişkisi var, .Net’e kullanım şekillerinden biride INotifyPropertyChanged interface’inden türeyip, .Net’in binding alt yapısını kullanması. Zaten özünde yaptığı iş DataBinding. Kendi propertylerini View’in propertyleriyle senkronize ediyor, aynı zamanda state’lerede karar veriyor, mesela şu şu TextBox dolduğunda şu Buton enabled olsun gibi. Tabi herzaman enabled olucak bir kontrol’un state’ini PM’de tutmak anlamsız.

PM’in en büyük avantajı, hiç bir View’e ihtiyaç duymadan bir View’in davranışlarını ve Data’sını barındarabilmesi, bu yapısıyla TDD’ye (Test Driven Development) çok uygun.

### MVU (Model-View-Update)
Buradaki siteyi ziyaret edebilirsiniz.
- https://thomasbandt.com/model-view-update

<p align="center"><strong>Hüseyin Karacif tarafından :heart: ile hazırlandı.</strong></p>
