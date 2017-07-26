# Операторы и выражения

### Циклы for, while, repeat until

Вложенные выражения циклов `for`, `while` и `repeat until` должны быть выделены отступом размером в два пробела. Каждую часть вложенного составного оператора необходимо размещать на новой строке.

Примеры оформления цикла `for`:

```Pascal
// НЕПРАВИЛЬНО:
for I := 0 to 10 do begin
  DoSomething; 
  DoSomethingElse;
end;
```

```Pascal
// НЕПРАВИЛЬНО:
for I := 0 to 10
do begin
  DoSomething;
  DoSomethingElse;
end;
```

```Pascal
// ПРАВИЛЬНО:
for I := 0 to 10 do
  DoSomething;
```

```Pascal
// ПРАВИЛЬНО:
for I := 0 to 10 do
begin
  DoSomething;
  DoSomethingElse;
end;
```

Примеры оформления цикла `while`:

```Pascal
// НЕПРАВИЛЬНО:
while X < J do begin
  DoSomething; 
  DoSomethingElse;
end;
```

```Pascal
// НЕПРАВИЛЬНО:
while X < J
do begin
  DoSomething;
  DoSomethingElse;
end;
```

```Pascal
// ПРАВИЛЬНО:
while X < J do 
begin
  DoSomething; 
  DoSomethingElse;
end;
```

```Pascal
// ПРАВИЛЬНО:
while X < J do
  DoSomething;
```

Конструкция `repeat until` не требует наличия операторных скобок.  
Примеры оформления цикла `repeat until`:

```Pascal
// НЕПРАВИЛЬНО:
repeat
begin
  X := J;
  J := UpdateValue;
end;
until J > 25
```

```Pascal
// ПРАВИЛЬНО:
repeat
  X := J;
  J := UpdateValue;
until J > 25;
```



