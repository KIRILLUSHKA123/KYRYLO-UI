# KYRYLO-UI | DOCUMENTAION 

## Installation
* File **KUI_Library**(module-script) place to **ReplicatedStorage**.
* File that setup your UI place in **StarterGui** or in **StarterPlayerScripts**.

## Require
```lua
local KUI = require(ReplicatedStorage.KUI_Library)
```

## Init
```lua
KUI.Init( <object> PlayerGui , <number> ,20)
```
```
Parameters:

1 | object | PlayerGui
2 | number | Line width in offset
3 | number | Blur size
```

## Component: Window
```lua
local Window = KUI.Window.new( <string> name )
```
```lua
:Show()
>>> Window

:Hide()
>>> Window

:Close()
>>> Window

:BindAction( <string> action (show/hide/close) , <string> inputType (began/ended) , <Enum.KeyCode> keyboardBind )
>>> true or false

:UnbindAction( <string> action (show/hide/close) , <string> inputType (began/ended) )
>>> true or false
```
