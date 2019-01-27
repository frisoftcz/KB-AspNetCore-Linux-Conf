# KB-AspNetCore-Linux-Conf
AspNetCoreWebApp.conf
  - konfigurace VirtualHost pro Apache, který komunikuje na portu 5000
  - kopíruje se do adresáře /etc/apache2/conf-enabled
  - jeden univerzální konfigurační soubor, při vývoji aplikací jenom vyměňujeme AspNet Core Web aplikaci, která komunikuje na portu 5000
  
kestrel-AppApache.service
  - konfigurace AspNet Core Web aplikace jako služby v systému Linux
  - kopíruje se do adresáře /etc/systemd/system
  - tímto způsobem můžeme vyvíjet více aplikací, každá aplikace má svůj vlastní konfigurační soubor s jiným jménem
  - vždy je jedna služba enabled a ostatní disabled (je třeba zajistit, aby na portu 5000 komunikovala vždy jen jedna služba)
  
