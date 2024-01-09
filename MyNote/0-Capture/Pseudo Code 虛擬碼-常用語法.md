### 語法規則
1、每一條指令佔一行(else if除外)
2、指令後不跟任何符號
3、用**縮排**表示**塊結構、分支結構**，代替begin..end、if-then-else語句

----

[[演算法名稱]]
[[指令序列]]
[[輸入/輸出]]
[[分支選擇]]
[[賦值]]
[[迴圈]]
[[陣列]]
[[演算法結束]]
[[註釋]]
[[物件]]
### 範例
```
// 氣泡排序
 procedure Bubble(n:integer);
   var temp,i,j:integer;
   change:boolean;
   begin
      for i:=1 to n-1 do
      begin
        change:=false;
        for j:=n-1 downto i do
          if a[j]>a[j+1] then
          begin
            change:=true;
            temp:=a[j]; a[j]:=a[j+1]; a[j+1]:=temp;
          end;
          if not(change) then exit;
      end;
   end;

// 插入排序
procedure insertsort(n:integer);
  var i,j:integer;
  begin
    for i:=2 to n do
    begin
      a[0]:=a[i];
      j:=i-1;
      while a[j]>a[0] do
      begin
        a[j+1]:=a[j];
        j:=j-1;
      end;
      a[j+1]:=a[0];
    end;
  end;

```

```pseudocode
/* this is a pseudocode sample */

a := 1
b ← a + 2
c :=[100]

//如果a大於等於2，就做標籤列印(Label_Print)，否則就
if a ≥ 2 then
    goto Label_Print
else
    for i := 0 to 100
        a := a + i

    do j := (a+b*i)/100
        c[j] = a+b*i
    until j>100

    return

Label_Print:
    while b ≠ 3 and a = 4 do
        call log(b,a)
    end

exit
```
