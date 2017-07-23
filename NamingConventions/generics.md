# Соглашения о наименовании

### Обобщенные типы

Средства обобщенного программирования, известные как дженерики \(_generics_\), представлены в языке Delphi обобщенными типами, обобщенными классами, обобщенными функциями и процедурами.

Пример описания обобщенного класса:

```Pascal
 type
   TPair<TKey, TValue> = class
   private
     FKey: TKey;
     FValue: TValue;
   public
     function GetKey: TKey;
     procedure SetKey(Key: TKey);
     function GetValue: TValue;
     procedure SetValue(Value: TValue);
     property Key: TKey read GetKey write SetKey;
     property Value: TValue read GetValue write SetValue;
   end;
```

Пример объявления обобщенного класса:

```Pascal
 type
   TStrIntPair = TPair<String, Integer>;
```



