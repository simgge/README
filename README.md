# README
CASE1:  
- Optimum gereksinimlerle makineyi kurdum. 
- Kurarken network configuration yapmamıştım, onu da root kullanıcısında "nmcli d" komutundan NetworkManager TUI'yi açarak interfacete DHCP konfigürasyonu kısmında "Automatically Connect"i seçerek gerçekleştirdim. 
- yum check-update ile updateleri gerçekleştirdim. 
- Kurulum esnasında simge.ucar userını oluşturmuştum. - df -h ve fdisk -l ile current size'a baktım.  
- ls /sys/class/scsi_host/  
- ls /sys/class/scsi_device/ 
- fdisk -l 
- Yeni partition için: fdisk /dev/sda , sonra çıkan harf karşılıklarına göre yönlendirdi. m help için kullanıldı, sonra p n p harflerine yönlendirdi. 
- pwd /opt/bootcamp/ ile girildi, touch bootcamp.txt yazılıp dosya oluşturuldu. vim ile içine "merhaba trendyol" yazıldı. 
- find /home -iname 'bootcamp.txt' -exec mv '{}' /opt/bootcamp/ \;  

CASE2: 

- docker ps -a 
- docker run nginx:1.19.9 
- docker ps ile arka planda çalışıp çalışmadığına baktım. 
- docker run -p [oluşturulan docker imageının port nosu] nginx:1.19.9 ile erişime açtım. (expose) 
* Yani aslında "db kullanan bir uygulamayı dockerize ederken ve nginxten serve ederken" port forwarding yapıyorum.* 
- docker stop [image]  
- docker start (ayağa kalktı)
