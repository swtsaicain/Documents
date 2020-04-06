# AutoHotkey

## Basic usage

### Variable  
* test  

### 流程控制
* For  
> 無窮迴圈
```
Loop {
    ...
}
```
  * 範例
```
Loop {
    if (A_Index > 25)
        break  ; Terminate the loop
    if (A_Index < 20)
        continue ; Skip the below and start a new iteration
    MsgBox, A_Index = %A_Index% ; This will display only the numbers 20 through 25
}
```
  * 參考
    * [Loop](https://www.autohotkey.com/docs/commands/Loop.htm)

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
    * Mode: 抓取顏色的方法
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
