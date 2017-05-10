# Пробелы и межстрочные расстояния

### Перенос строк

Длина любой строки кода не должна превышать 80 символов. Если это условие не соблюдается, решением представляется разделение данной строки на несколько частей. Каждая перенесенная часть должна быть выравнена и находиться на расстоянии в два пробела от начала основной.

Слово `begin` следует располагать на отдельной строке.

Примеры:

```Pascal
// ПРАВИЛЬНО:

function CreateWindowEx(dwExStyle: DWORD; 
  lpClassName: PChar; lpWindowName: PChar; 
  dwStyle: DWORD; X, Y, nWidth, nHeight: Integer;
  hWndParent: HWND; hMenu: HMENU; hInstance: HINST; 
  lpParam: Pointer): HWND; stdcall;

// НЕПРАВИЛЬНО:

if ((X = Y) or (Y = X) or
  (Z = P) or (F = J) then
begin
  S := J;
end;
```



