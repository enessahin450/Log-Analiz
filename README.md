<h1>LOG ANALİZİ</h1>

<h3>Log Nedir?</h3>
<ul>
<li>Bilişim sistemlerinin ürettiği kayıt bilgilerine log denir. Loglama ise bu kayıtların ve dijital hareketlerin tutulma işlemidir.</li>
<li>Meydana gelen olayları ve hareketleri kayıt altına alırlar.</li>
<li>Yazılımlar, IoT cihazları, işletim sistemleri ve web sunucuları aktif olarak log kaydı tutarlar.</li>
<li>Örneğin bir web sunucusunun içerisinde yer alan log dosyaları incelenerek ziyaretçilerin nereden geldiği ve web sunucusuna hangi istekleri gönderdiği kolaylıkla anlaşılabilir.</li>
</ul>
<h3>Loglar Nereden Üretilir?</h3>
<ul>
<li>Uygulamalar</li>
<li>Konteynerlar</li>
<li>Veritabanları</li>
<li>Güvenlik Duvarları</li>
<li>Uç Noktalar</li>
<li>IoT Cihazlar</li>
<li>Ağlar</li>
<li>Ağ Hizmetleri</li>
<li>Sunucular</li>
<li>İşletim Sistemleri</li>
</ul>
<h3>Günlük Log Kaydı Örneği</h3>
<p>
<b> 127.0.0.1 user-identifier frank [10/Oct/2000:13:55:36 -0700] "GET /apache_pb.gif HTTP/1.0" 200 2326(Wikipedia sunucu günlük kaydı örneği)</b> <br />
 user-idenfier -> Kullanıcı Tanımlayıcısı <br />
 127.0.0.1 -> Uzak ana makine adı. DNS ana makine adı IP kullanılır. <br />
 Frank -> Sayfayı isteyen kişinin kullanıcı kimliği. <br />
 [10/Oct/2000:13:55:36 -0700] -> Eylemin tarihi. <br />
 GET /apache_pb.gif HHTP/1.0 -> GET gerçekleştirilebilen iki komuttan biridir. apache_pb.gif HTTP erişilen URL’dir. HTTP sürümüdür.<br />
 <b>127.0.0.1 user-identifier frank [10/Oct/2000:13:55:36 -0700] "GET /apache_pb.gif HTTP/1.0" 200 2326 </b><br />
 200 -> Döndürülen belgenin durum kodu.<br />
 2326 -> Döndürülen belgenin bayt cinsinden boyutu.<br />
</p>
<h3>Neden Log Kaydı Tutulur?</h3>
<ul>
<li>Güvenlik Konusu : Saldırı olayları ve diğer izinsiz olayları araştırmak.</li>
<li>Geliştirme ve Kalite Güvencesi : Bir program ya da uygulama oluşturmasında sorunlu bug’ların kontrol edilmesi için yapılandırılan programlamanın düzgün çalışıp çalışmadığını kontrol etmek için.</li>
<li>Ağ Sorunlarını Giderme : Bir ağdaki yanıtlama ve sistem hatalarını düzeltme.</li>
<li>Uyum Konuları : Kurumsal firma ya da devlet politikalarına yanıt olarak bilgi toplama.</li>
</ul>
<h3>Log Kayıtları Kimler Tarafından Kullanılır</h3>
<ul>
<li>DevOps:
<ul>
<li>CI/CD’yi yönetme.</li>
<li>Uygulama çalışma süresini koruma.</li>
<li>Kritik uygulamaların hatalarını tespit etmek.</li>
<li>Uygulamaların performansınıoptimize etmek için alan belirleme.</li>
</ul>
</li>
<li>DevSecOps:
<ul>
<li>Uygulama geliştirme ve güvenliği.</li>
<li>Dağıtımdan önce olası sorunları bularak zaman, para ve tekrarlama gibi sorunlardan kurtulmak için.</li>
</ul>
</li>
<li>SecOps:
<ul>
<li>Bir saldırı hakkında ‘kim, ne zaman, nerede’ gibi ipuçları verir. </li>
<li>Şüpheli etkinliği  tanımlama.</li>
<li>Engellenen/izin verilen trafikteki ani artışları görmek için.</li>
<li>OODA döngüsü gibi metodolojilerinin uygulanması.</li>
</ul>
</li>
<li>BT Analistleri:
<ul>
<li>Uyumluluk yönetimi ve raporlama.</li>
<li>OpEx ve CapEx. </li>
</ul>
</li>
</ul>
<h3>Log Çeşitleri</h3>
<ul>
<li>Event Log:
<ul>
<li>Windows sistemlerde log kayıtlarının tutulduğu yerdir.</li>
<li>Yönetici hesabı ile işlemler yapılabilir.</li>
<li>Sistem üzerinde gerçekleşen bütün işlemler kayıt olarak tutulur.</li>
<li>Hesap kitlemeleri, oturum açma işlemi, uygulama hataları gibi güvenlik için farklı türde olayları kaydeder.</li>
<li>Event Log Kayıt Değerleri :<br /> 4624 -> Başarılı Login, 4625-> Başarısız         Login, 44672-> Admin Hesanı Logini, 5140-> Ağ Paylaşımı Planlandı,   5025-> Firewall Durduruldu.</li>
</ul>
</li>
<li>Syslog:
<ul>
<li>Sistem günlüğü anlamına gelir. Mesaj loglama standartıdır.</li>
<li>Unix ve Linux tabanlı sistemler için kullanılır. </li>
<li>Güvenlik duvarları, yönlendiriciler ve yazıcılar gibi çeşitli cihazlar syslog standartını kullanır.</li>
<li>Sistem yöneticileri için önemlidir.</li>
<li>Sistem hataları, sisteme saldırılar veya sistem üzerinde oluşan sorunlar kayıt altında tutulur.</li>
<li>Syslog sistemleri farklı bir sisteme devredilebilir. Bu sayede uzaktan log kayıtlarına ulaşıp yönetim sağlanabilir.</li>
</ul>
</li>
<li>Server Log:
<ul>

<li>Belirli bir zaman diliminde belirli bir sunucuyla ilgili etkinliklerin kaydını içerir.</li>
</ul>
</li>
<li>Transaction Log:
<ul>
<li>Temel olarak veri tabanındaki değişikliklerin kaydını tutar.</li>
<li>Örneğin bir kullanıcı veritabanına tablo ekler veya silerse transaction loga kaydedilir.</li>
<li>Eğer veritabanında bir arıza olursa veritabanının geri yüklenmesini ve verilerin kaybolmasını önler.</li>
<li>Temel olarak veri tabanındaki değişikliklerin kaydını tutar.</li>
</ul>
</li>
</ul>
<h3>Log Dosya Türleri</h3>
<ul>
<li>Access Log : Erişim günlükleri, sunucunuzdan hangi html dosyalarının istendiği bilgilerini kaydeder.</li>
<li>Agent Log : Sunucunuzda hangi web istemcilerinin istekte bulunduğuna ilişkin bilgileri kaydeder.</li>
<li>Referrer Log : Web sayfanıza geçmeden önce ziyaretçinin bulunduğu URL hakkındaki bilgileri kaydeder.</li>
<li>Error Log : Hata günlüğü, sunucunun başarısız isteklerini kaydeder. Birisi sunucunuzda var olmayan bir dosyaya erişmeye çalıştığında otomatik olarak hata mesajı oluşturur.</li>
</ul>
<h3>Log Yasası - 5651 Sayılı Kanun</h3>
<ul>
<li> İnternet sağlayıcılarında paylaşılan ağ trafiklerinin izlenmesi ve bağlantı kuran aygıtlarının mac, ip, ziyaret adresi, oturum süresi, bağlantı istekleri raporlarının kaydedilmesini zorunlu kılan yasa.</li>
<li>Amaç siber ortamda işlenen suç eylemlerinin yeri, zamanı ve failinin tespiti.</li>
<li>Kayıtlar 6 ay ile 2 yıl arasında saklanmalı.</li>
<li>Alınan kayıtların doğru, tutarlı ve sonradan değiştirilemez olması için zaman damgası (HASH) ile muhafaza edilir.</li>
</ul>
<h3>Apache Web Server</h3>
<ul>
<li>Apache açık kaynak kodlu, güçlü, sağlam ve esnek bir http (web) sunucusudur.</li>
<li>Apache Software Foundation (ASF) tarafından geliştirilir.</li>
<li>Açık kaynak kodlu olduğu için lisansı ücretsizdir.</li>
<li>İnternetteki web sitelerinin %60’ı Apache üzerinde çalışmaktadır. Apache en yakın rakibi Microsoft’un web sunucularının 3 katı Pazar payına sahiptir.</li>
</ul>
<h2>Windows Log</h2>

![windowsLog](https://user-images.githubusercontent.com/73036927/205508318-757ae67a-4e15-48c8-a266-8cb7a498aa81.png)


<h2>Linux Logları</h2>

![linuxLog](https://user-images.githubusercontent.com/73036927/205508371-53060cc0-0d6e-4a5a-810d-469143a15749.png)


<h2>Apache Log</h2>

![apacheLog](https://user-images.githubusercontent.com/73036927/205508402-6df10fcf-9226-4f5b-bf82-2b9ef92f8d5e.png)




<h3>ELK Nedir?</h3>
<ul>
<li>ElasticSearch : Dış uygulamalar üzerinden toplanan verilerin analizi ve içerik gibi işlemleri yapmamızı sağlayan bir arama motorudur.</li>
<li>Logstash : Log toplayan, ihtiyaca göre onları işleyen ve Eleasticsearch’e bu logları indekslenemek üzere gönderen sistemdir.</li>
<li>Kibana : Toplanıp anlamlı hale getirilen verinin, analizini yaptıktan sonraki görselleştirme işlemini yapar. Grafik yapılar ile analiz.</li>
</ul>

![ELK1](https://user-images.githubusercontent.com/73036927/205508446-c6b68908-69b6-43b5-b9fd-9541df74bb8f.png)



![ELK2](https://user-images.githubusercontent.com/73036927/205508451-d8c637a1-328f-4fdd-a140-a61f861ddfaf.png)
