# AutoHotkey

## Basic usage

### Variable  
* test  

### Functions
* Function
  * 範例
    ```
    Add(x, y)
    {
        return x + y
    }
    ```
  * 參考
    * [Functions](https://lexikos.github.io/v2/docs/Functions.htm)

### 流程控制
* For  
> 無窮迴圈
  * 語法
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
* For, count
> 指定次數迴圈
  * 語法
    ```
    Loop %RepeatCount% {
        ...
    }
    ```
  * 範例
    ```
    Loop, 3 {
        MsgBox, Iteration number is %A_Index%.  ; A_Index will be 1, 2, then 3
        Sleep, 100
    }
    ```
  * 參考
    * [Loop](https://www.autohotkey.com/docs/commands/Loop.htm)
### Color  
* PixelGetColor  
> 取得指定位置座標顏色
  * 語法
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
