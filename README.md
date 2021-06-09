# Функция List.Contains в Power Query

### Написание функции
List.Contains(list, value, optional criteria)

**Аргументы:**  
* list - список значений,  
* value - значение,   
* criteria - функция сравнения (необязательный параметр).  

**Результат:**  
* если значение value содержится в списке list, выдаёт TRUE.  
* если значение value не содержится в списке list, выдаёт FALSE.  

### Примеры
```
let  
    letters = {"a","б","в","г"},  
    one = "А",  
    result = List.Contains(letters, one)  
in result  
```
