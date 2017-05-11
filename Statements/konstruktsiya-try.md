# Выражения и конструкции

### Конструкция try

Корректный пример оформления конструкции try может выглядеть следующим образом:

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



