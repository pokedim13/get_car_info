<h1>Получение информации по госномеру</h1>

<h3>Использование:</h3>

```python
from car_info import CarInfo

# Укажите российский автомобильный номер в формате А123АА97
car = CarInfo('Е005КХ05')
data = car.get_data()

# Некоторая информация
print('Номер:', data.number)
print('vin:', data.vin)
print('Марка:', data.marka)
print('Модель:', data.model)
print('Год производства:', data.year)
```

При указании гос номера необходимо использовать кириллицу!
<hr>

> `car.get_data()` возвращает Pydantic объект, где описаны характеристики автомобиля
<hr>

###### • Вся полученная информация находится в общем доступе. Данные получены с помощью <a href="https://vinvision.ru/">www.vinvision.ru</a>
