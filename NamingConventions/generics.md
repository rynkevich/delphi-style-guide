# Соглашения о наименовании

### Обобщенные типы

Средства обобщенного программирования, известные как дженерики \(_generics_\), представлены в языке Delphi обобщенными классами, интерфейсами, записями и методами.

Идентификаторы типов-параметров, используемых при описании дженерика, могут иметь вид не только обычного идентификатора типа \(шаблон `TName` \), но и одиночной буквы `T`, однако лишь в том случае, если в пределах программного модуля не встречается других типов-параметров.

Пример описания обобщенного класса:

```Pascal
 // ПРАВИЛЬНО:
 type
   TPair<TKey, TValue> = class
   private
     FKey: TKey;
     FValue: TValue;
     function GetKey: TKey;
     procedure SetKey(Key: TKey);
     function GetValue: TValue;
     procedure SetValue(Value: TValue);
   public
     property Key: TKey read GetKey write SetKey;
     property Value: TValue read GetValue write SetValue;
   end;
```

Следующее описание тоже будет являться правильным, если соблюдено вышеупомянутое условие:

```Pascal
// ПРАВИЛЬНО:
type
  TLinkedList<T> = class
    ...
  end;
```

Пример корретных объявлений дженерик-классов:

```Pascal
// ПРАВИЛЬНО:
var
  StrIntPair: TPair<string, Integer>;

// ПРАВИЛЬНО:
var
  SomeList: TLinkedList<Real>;
```



