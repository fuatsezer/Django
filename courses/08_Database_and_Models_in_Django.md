# Creating A Database Table
İlk önce Tabloları classlar olarak models.py içinde yaratıyoruz. Aşağıda Products tablosu için örnek bir kod var.
`myapp/models.py`
```python
from django.db import models

# Create your models here.
class Product(models.Model):
    name = models.CharField(max_length=100)
    price = models.IntegerField()
    desc = models.CharField(max_length=200)
```
