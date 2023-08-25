# Creating A Database Table
1) İlk önce Tabloları classlar olarak models.py içinde yaratıyoruz. Aşağıda Products tablosu için örnek bir kod var.
`myapp/models.py`
```python
from django.db import models

# Create your models here.
class Product(models.Model):
    name = models.CharField(max_length=100)
    price = models.IntegerField()
    desc = models.CharField(max_length=200)
```
2) mysite/settings.py da INSTALLED_APPS listesine app'in ismini eklyin.
`mysite/settings.py`
```python
INSTALLED_APPS = [
    "myapp",
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
]
```
3) Aşağıdaki komutları çalıştırın. (models.py da Her yeni class oluşturduğunuzda)

```console
(env) C:\Users\fsezer\Desktop\Django\djangopro\mysite>python manage.py makemigrations
(env) C:\Users\fsezer\Desktop\Django\djangopro\mysite>python manage.py migrate
```


