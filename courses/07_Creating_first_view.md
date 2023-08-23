# İlk View'ı Oluşturma
1) App klasörünün altındaki views.py dosyasına aşağıdaki gibi bir fonksiyon ekleyin.

`myapp/views.py`
```python
from django.shortcuts import render
from django.http import HttpResponse
# Create your views here.
def index(request):
    return HttpResponse("Hello World")
```
2) App klasörünün içine bir urls.py adlı dosya oluşturun ve içinde aşağıdaki kodlar olsun.
 
`myapp/urls.py`
```python
from django.contrib import admin
from django.urls import path
from . import views
urlpatterns = [
    path("", views.index),
]
```
3) Proje klasörünün altındaki urls.py dosyasındaki kodlar şöyle olmalıdır.

`mysite/urls.py`
```python
from django.contrib import admin
from django.urls import path,include

urlpatterns = [

    path('admin/', admin.site.urls),
    path("myapp/",include("myapp.urls"))
]

```
 
