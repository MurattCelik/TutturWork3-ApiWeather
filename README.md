##### TutturHomework3-ApiWeather
 
##Shell Script İle Hava Durumunu Twittera Yazdırma
        
####         Shell Script ile belli bir siteden curl kullanarak hava durumunun Apisini aldıktan sonra jsawk yardımı ile sadece sıcaklığını döndürüyoruz.Daha sonra oluşturduğumuz twitter uygulamasıyla Twitter Apisini kullanarak t uygulamasına bağlayarak Crontab ayarlı belirlediğimiz zamanlarda tanımlı Twitter hesabına anlık sıcaklık otomatikmen aktarılıyor.


#####Gerekli İşlemler

  **1-**Hava Durumu Apisi

  **2-**Jsawk 

  **3-**Twitter Apisi

  **4-**Twitter İçin Yazılan t Uygulaması

  **5-**CronTab Oluşturulması

 
  **1-Hava Durumu Apisi**
  
Gerekli olan hava durumun Apisini almamız için herhangi bir hava durumu sitesine üye
olmamız gerekiyor.Bu kod için openweathermap isimli siteye üye olduktan sonra oluşturduğumuz 
uygulama ile hava durumun Apisini alıyoruz.
    
  **2-Jsawk** 
  
Aldığımız hava durumun Apisi ile hava durumuyla ilgili her detay veriliyor ama istediğimiz sadece havanın sıcaklığı ve burda
jsawk devreye giriyor.Jsawk yardımıyla sadece sıcaklığı döndürüyoruz.

https://github.com/micha/jsawk
       
  **3-Twitter Api**
           
Gerekli olan twitter Apisini tanımlı bir hesaptan oluşturduğumuz uygulama ile Twitter Apisini alıyoruz.Bizim için gerekli
olan daha doğrusu t uygulaması için gerekli olan sadece Api Key ve Secret Key'dir.Shell'de bunlarla t uygulaması ile bağlantıyı
kurduktan sonra otomatik twet atılıyor.
           
  **4-Twitter İçin Yazılan t Uygulaması**
         
Gerekli bağlantı için t uygulamasını sisteme yüklüyoruz.Yükledikten sonra "authorize" komutu ile bağlantıya geçiyoruz.
Daha sonra Sırayla bizden Api Key VE Secret Key'i girmemizi istiyor.Girdikten sonra geriye sadece twittera erişim iznini
vermemiz gerekiyor,verdikten sonra bağlantıyı gerçekleştirmiş bulunmaktayız.
Shell'de t update deyip istediğimizi yazdığımızda otomatikmen twittera atılıyor.
Bizim kodda yazmasını istediğimiz içerik biz buraya sıcaklığı yazdırıyoruz ek olarak date komutu ile de tarihide
yazdırıyoruz.

https://github.com/sferik/t
           
  **5-CronTab Oluşturulması**
   
Crontab Unix sistemlerinde zaman bazlı çalışan bir görev planlayıcısıdır.
Bizim yaptırmak isteğimiz işlem ise belirlediğimiz zaman aralıklarında çalşması için CronTab Oluşturmaktır.

https://github.com/Cron/Cron
     
     
     
     
     
     
     
