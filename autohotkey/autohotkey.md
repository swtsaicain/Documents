# AutoHotkey

## Basic usage

### Variable  
* test  

### Color  
* PixelGetColor  
> 取得指定位置座標顏色  
```
  PixelGetColor, OutputVar, X, Y , Mode
```
  * 範例
```
^!z::  ; Control+Alt+Z hotkey.
MouseGetPos, MouseX, MouseY
PixelGetColor, color, %MouseX%, %MouseY%
MsgBox The color at the current cursor position is %color%.
return
```
  * 參考
    * [PixelGetColor](https://www.autohotkey.com/docs/commands/PixelGetColor.htm)
