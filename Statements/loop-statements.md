# Выражения и конструкции

### Циклы for, while, repeat until

Вложенные выражения циклов `for`, `while` и `repeat until` должны быть выделены отступом размером в два пробела. Каждую часть вложенного сложного выражения необходимо размещать на новой строке.

Примеры оформления цикла `for`:

```Pascal
// НЕПРАВИЛЬНО:
for I := 0 to 10 do begin
  DoSomething; 
  DoSomethingElse;
end;

// НЕПРАВИЛЬНО:
for I := 0 to 10
do begin
  DoSomething;
  DoSomethingElse;
end;

// ПРАВИЛЬНО:
for I := 0 to 10 do
  DoSomething;

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

// НЕПРАВИЛЬНО:
while X < J
do begin
  DoSomething;
  DoSomethingElse;
end;

// ПРАВИЛЬНО:
while X < J do 
begin
  DoSomething; 
  DoSomethingElse;
end;

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

// ПРАВИЛЬНО:
repeat
  X := J;
  J := UpdateValue;
until J > 25;
```



