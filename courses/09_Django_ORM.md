## INSERT with DJANGO ORM
1) Aşağıdaki komutu çalıştırarak python shell'i açın (exit() yazarak python shell'i kapatabilirsiniz)

```console
(env) C:\Users\fsezer\Desktop\Django\djangopro\mysite>python manage.py shell
```
2) Python shell'e aşağıdaki kodları yazın.
```python
>>> from myapp.models import Product
>>> Product.objects.all()
<QuerySet []>
>>> a = Product(name="iPhone", price=900, desc="This is an iPhone")
>>> a.save()
>>> b = Product(name="iPad", price=1200, desc="This is an iPad")
>>> b.save()
>>> Product.objects.all()
<QuerySet [<Product: iPhone>, <Product: iPad>]>
>>> Product.objects.get(id=1)
<Product: iPhone>
```
