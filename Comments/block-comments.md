# Комментарии

### Многострочные комментарии

Язык поддерживает несколько способов представления многострочных комментариев. Наиболее популярный способ - это фигурные скобки: `{ }`. Его предпочитают и разработчики компиляторов языка. 

Использование символов `*` для выделения фрагментов текста не приветствуется. Вместо этого можно  использовать пробелы или переносы строк внутри содержимого комментария.

Текст комментария должен начинаться на той же строке, где расположена открывающая фигурная скобка. Ниже приведен пример из `DsgnIntf.pas`:

```Pascal
{ TPropertyEditor

  Edits a property of a component, or list of components, 
  selected into the Object Inspector.  The property 
  editor is created based on the type of the
  property being edited as determined by the types 
  registered by...
  
  etc...
  
    GetXxxValue
      Gets the value of the first property in the 
      Properties property.  Calls the appropriate 
      TProperty GetXxxValue method to retrieve the 
      value. 
      
    SetXxxValue Sets the value of all the properties 
      in the Properties property.  Calls the appropriate 
      TProperty SetXxxxValue methods to set the value. }
```



