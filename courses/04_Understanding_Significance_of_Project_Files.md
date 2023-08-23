# Understanding Significance of Project Files
![image](https://github.com/fuatsezer/Django/assets/63423939/c3c9123f-e096-4dba-8cb6-18b03fa132f3)
## These project files are:
`Dıştaki _projectroot/root` proje için bir kapsayıcıdır. Klasör yeniden adlandırılabilir.

`Manage.py` Bu Django projesi ile çeşitli şekillerde etkileşime girmenizi sağlayan bir komut satırı yardımcı programıdır. **Bu dosyaya dokunmayın.**

`İçteki _projectroot/` projeniz için gerçek python paketidir. Adı içindeki Adı, içindeki herhangi bir şeyi içe aktarmak için kullanmanız gereken Python paketinin adıdır (ör. _projectroot.urls).

`_projectroot/__init__.py` Python'a bu dizinin bir Python paketi olarak değerlendirilmesi gerektiğini söyleyen boş bir dosya.

`_projectroot/settings.py` Bu Django projesi için yapılandırma.

`_projectroot/urls.py` Bu Django projesinin URL bildirimleri; Django destekli sitenizin bir "içindekiler tablosu".

`_projectroot/asgi.py` ASGI uyumlu web sunucularının projenize hizmet vermesi için bir giriş noktası.

`_projectroot/wsgi.py` Projenize hizmet verecek WSGI uyumlu web sunucuları için bir giriş noktası.

## The App files

`admin.py` Modellerinizi Django admin'de değiştirilebilmeleri için buraya kaydediyoruz

`apps.py` Uygulama yapılandırma kodunu içerir

`models.py` Modellerinizi burada tanımlayın. Verilerin saklanması ve ilişkilerinin tanımlanması için kullanılan tablolardır.

`tests.py` Uygulama için testler yazma

`views.py` Templatelerde işlenecek verileri tanımlama
