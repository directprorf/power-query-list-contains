# Функция List.Contains в Power Query

### Написание функции
List.Contains(list, value, optional criteria)

**Аргументы:**  
* list - список значений,  
* value - значение,   
* а criteria - функция сравнения (необязательный параметр).  

**Результат:**  
Если значение value содержится в списке list, выдаёт TRUE.  
Если значение value не содержится в списке list, выдаёт FALSE.  

### Примеры
let  
  letters = {"a","б","в","г"},  
  one = "А",  
  result = List.Contains(letters, one)  
in result  
