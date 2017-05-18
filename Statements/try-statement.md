# Операторы и выражения

### Оператор try

Корректный пример оформления оператора try может выглядеть следующим образом:

```Pascal
// ПРАВИЛЬНО:
try
  try
    EnumThreadWindows(CurrentThreadID, @Disable, 0);
    Result := TaskWindowList;
  except
    EnableTaskWindows(TaskWindowList);
    raise;
  end;
finally
  TaskWindowList := SaveWindowList;
  TaskActiveWindow := SaveActiveWindow;
end;
```



