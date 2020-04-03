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
  * 參數
    * OutputVar: 抓取顏色放置變數
    * X: x 座標
    * Y: y 座標
    * Mode
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
