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

### Примеры в коде
```
let  
    letters = {"a","б","в","г"},  
    one = "Б",  
    result = List.Contains(letters, one)  
in result  
```
Выдаёт FALSE так как большая буква Б не содержится в списке.

```
let  
    letters = {"a","б","в","г"},  
    one = "Б",  
    result = List.Contains(letters, one, Comparer.OrdinalIgnoreCase)  
in result  
```
Выдаёт TRUE так как при сравнении игнорируется регистр.
