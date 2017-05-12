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

Многострочные комментарии обычно применяются при оформлении сообщения об авторском праве в начале модуля программы. Еще одно популярное их применение: описание метода перед его объявлением.

Примеры:

```Pascal
// ПРАВИЛЬНО: 

{ TMyObject.MyMethod

  Данный шаблон используется для выполнения фрагмента кода. }

procedure TMyObject.MyMethod;
begin
end;

// НЕПРАВИЛЬНО:

procedure TMyObject.MyMethod;
{******************************************************
  TMyObject.MyMethod

  Данный шаблон используется для выполнения фрагмента кода. 
*******************************************************}
begin
end;
```

Второй способ представления многосточных комментариев - использование скобок `(* *).` Чаще всего он используется в процессе разработки, когда применяют вложенные комментарии. Их применение возможно, если уровень вложенности не превышает 2.

Delphi не поддерживает вложенные комментарии одного типа, поэтому, фактически, уровень вложенности здесь только один: фигурные скобки внутри скобок со звездочками или скобки со звездочками внутри фигурных.

Такой прием позволяет сохранять в комментарии фрагмент кода, который сам содержит многострочные комментарии:

```Pascal
(* procedure TForm1.Button1Click(Sender: TObject);
begin
  StartAnyProcess; // Начать процесс
  ContinueDoingSmth; // Продолжить итерацию
  { ???: Здесь нужно будет обрабатывать возможные ошибки, может,
    используем try finally? }
  FewMoreOperations; // Завершить процесс
end; *)
```



