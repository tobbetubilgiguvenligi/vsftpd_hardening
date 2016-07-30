# vsftpd Hakında
vsftpd GPL lisanslı *NIX systemler için geliştirilmiş bir FTP (File Transfer Protokol) sunucusudur. İsmini very secure (çok güvenli) FTP'den alan sunucu Güvenlik, Performans ve Stabilite özelliklerini sunmak konusunda iddialıdır. 
#### Özellikleri
  * Sanal IP yapılandırması
  * Sanal kullanıcılar
  * Bağımsız veya inetd çalışma özelliği
  * Kullanıcı bazlı yapılandırma
  * Kaynak bazlı IP yapılandırması
  * Kaynak bazlı IP kısıtlama
  * IPv6 Desteği
  * SSL Desteği
  * ve daha fazlası

Daha detaylı bilgi, performans analizleri, güvenlik analizleri için geliştiricinin sitesine [burdan](https://security.appspot.com/vsftpd.html) göz atabilirsiniz.
  redhat,suse,debian,freebsd,gnu,gnome,kde,kernel ve çok daha fazla açık kaynak organizasyonları FTP server olarak vsftpd tercih etmektedir.

## vsftpd Sunucusu Sıkılaştırma Klavuzu
Bu klavuzda vsftpd sunucusunun sıkılaştırılması ve SSL/TLS desteğine kavuşturulması için adımlar anlatılacaktır. Bu adımları manul olarak yapabileceğiniz gibi hem sıkılaştırma işlemi için hemde SSL/TLS desteği için hazırlanmış betikleri kullanmaznızda mümkündür. Tüm adımlar Ubuntu 14.04.4 LTS ve Kali Linux 2016-1 işletim sistemleri üzerinde test edilmiştir.

###vsftp Sunucusunun Kurulumu
Sıkılaştırma işlemi paket yöneticisi yardımıyla yüklenen vsftpd sunucusuna uygulanmıştır. Kaynak kod üzerinden derleme yaparak kurulum yapılmış sunucu için birçok adım aynı olsada değişiklik yapılacak yapılandırma dosyanının dizini değişiklik gösterebilir. vsftpd sunucusunu yüklemek için terminalden aşağıdaki komutu girmek yeterlidir.

    sudo apt-get install vsftpd 


###vsftp Sunucusunun Sıkılaştırılması

###vsftp Sunucusunun SSL/TLS Desteği Eklenmesi
