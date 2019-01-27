# KB-AspNetCore-Linux-Conf
AspNetCoreWebApp.conf
  - konfigurace VirtualHost pro Apache, který komunikuje na portu 5000
  - kopíruje se do adresáře /etc/apache2/conf-enabled
  - jeden univerzální konfigurační soubor, při vývoji aplikací jenom vyměňujeme AspNet Core Web aplikaci, která komunikuje na portu 5000
  
kestrel-AppApache.service
  - konfigurace AspNet Core Web aplikace jako služby v systému Linux
  - kopíruje se do adresáře /etc/systemd/system
  - tímto způsobem můžeme vyvíjet více aplikací, vždy je jedna služba enambled a ostatní disabled
  
