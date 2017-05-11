# Выражения и конструкции

### Конструкция if-then-else

Конструкция if должна занимать как минимум две строки:

```Pascal
// НЕПРАВИЛЬНО:
if A < B then DoSomething; 

// ПРАВИЛЬНО:
if A < B then 
  DoSomething;
```

Содержимое "ветки" конструкции необходимо выделять отступом размером в два пробела.

Каждую строку сложного выражения следует располагать на отдельной строке. Конструкция оформляется согласно следующему примеру:

```Pascal
// НЕПРАВИЛЬНО:
if A < B then begin
  DoSomething; 
  DoSomethingElse;
end else begin
  DoThis;
  DoThat;
end;

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
```

Нижеприведенные виды оформления конструкции менее популярны, но также являются корректными:

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
else DoThat;
```



