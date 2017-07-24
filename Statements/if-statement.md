# Операторы и выражения

### Оператор if-then-else

Оператор `if-then-else` должен занимать как минимум две строки:

```Pascal
// НЕПРАВИЛЬНО:
if A < B then DoSomething; 

// ПРАВИЛЬНО:
if A < B then 
  DoSomething;
```

Содержимое "ветки" оператора необходимо выделять отступом размером в два пробела.

Каждую часть вложенного составного оператора следует располагать на отдельной строке. Конструкция оформляется согласно следующему примеру:

```Pascal
// ПРАВИЛЬНО:
if A < B then 
begin
  DoSomething; 
  DoSomethingElse;
end 
else 
begin
  DoThis;
  DoThat;
end;

// НЕПРАВИЛЬНО:
if A < B then begin
  DoSomething; 
  DoSomethingElse;
end else begin
  DoThis;
  DoThat;
end;
```

Приведенные ниже виды оформления оператора менее популярны, но также являются корректными:

```Pascal
// ПРАВИЛЬНО:
if Condition then
begin
  DoThis;
end else
begin
  DoThat;
end;

// ПРАВИЛЬНО:
if Condition then
begin
  DoThis;
end
else
  DoSomething;

// ПРАВИЛЬНО:
if Condition then
begin
  DoThis;
end else
  DoSomething;

// ПРАВИЛЬНО:
if Condition then
  DoThis
else if AnotherCondition then
  DoThat
else if YetAnotherCondition then
  DoSmthElse;

// ПРАВИЛЬНО:
if Condition then
  DoThis
else DoThat;
```



