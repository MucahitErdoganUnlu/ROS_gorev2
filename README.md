Görev Özeti:
Bu görevde srv dosyası kullanarak node’lar arasında haberleşme yapılması amaçlanmıştır.  Server ve client iki ayrı ros node olmak üzere srv dosyası sayesinde mesaj alıp verebilir. 

Görev Tanımı:
	Server ve client için iki ayrı dosya oluşturulmalı. Srv dosyasını kullanabilmek için srv isimli bir klasör olşturun ve srv dosyasının içeriğini düzenleyin. Client girdi olarak isim(string) ve yaş(int) almaktadır, server ise bu bilgileri alıp bir cümle içinde akrana bastıracak. 
	Burda diğer önemli nokta client bu bilgileri argüman olarak almalı. Ayrıca server ve client’in çalışma sürelerini de denetlemeniz rica olunur. Örneğin 5 sn sonra server’ı kapatmak gibi.

Örnek girdi:
![alt text](https://uniim1.shutterfly.com/render/00-RMNuRf_cvlSvCr7IsrJuykDnqygDeyuHrhkoGCpCYg4S-a0etjvYGpkMVNQMauH0VZV51t4MhjbEwRNyGscOgg?cn=THISLIFE&res=x-small&ts=1666950427)

Örnek çıktı:
![alt text](https://uniim1.shutterfly.com/render/00-RMNuRf_cvlSvCr7IsrJuykDnqygDeyuHrhkoGCpCYg4l2TbWhxA19loW9yoYFYkqqCe7ffHDJpwno-pEcjtJnw?cn=THISLIFE&res=small&ts=1666950179)
	



Notlar:
CMakeLists.txt ve package.xml dosyasını srv dosyası kullanacak şekilde ayarlamalısınız.
http://wiki.ros.org/ROS/Tutorials/WritingServiceClient%28c%2B%2B%29#roscpp_tutorials.2FTutorials.2FWritingServiceClient.Running_the_Server
srv dosyasını oluşturup kodu derledikten sonra devel klasöründe .h uzantılı dosyalar oluşacaktır, onu include etmeyi unutmayın.(Üstteki ros tutorialda “AddTwoInts.h” isimli dosya ordan geliyor)
Argümanları char olarak veriyorsunuz, srv dosyasındaki içeriğe göre tür dönüşümü yapmayı unutmayın.
Önce server’ı çalıştırmayı unutmayı, hatta birini kapatip nasıl bir sonuç alacağınıza bakabilirsiniz.
