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
KUI.Init( <object> PlayerGui , <number> lineWidthInOffset , <number> blurSize  )
```

## Component: Window
```lua
local Window = KUI.Window.new( <string> name )
```
```lua
:GetCurrentPage()
>>> <number> CurrentPage

:SetTitle( <string> newTitle )
>>> <boolean> true or false

:SetCloseButtonEnabled( <boolean> newStatement (true/false) )
>>> <boolean> true or false

:SetCorner( <number> radius )
>>> <boolean> true

:SetBorder( <Color3> color , <number> size )
>>> <boolean> true

:SetLines( <table> lines )
>>> <boolean> true or false

:AddLine( <object> line )
>>> <boolean> true or false

:Show()
>>> <object> Window

:Hide()
>>> <object> Window

:Close()
>>> <object> Window

:BindAction( <string> action (show/hide/close) , <string> inputType (began/ended) , <Enum.KeyCode> keyboardBind )
>>> <boolean> true or false

:UnbindAction( <string> action (show/hide/close) , <string> inputType (began/ended) )
>>> <boolean> true or false
```

## Component: Line
```lua
local newLine = KUI.Line.new( <string> name , <number> layoutIndex )
```
```lua
:SetEnabled( <boolean> statement (true/false) )
>>> <object> Line

:SetLineLayout( <number> layoutIndex )
>>> <object> Line

:AddComponent( <object> component )
>>> <object> Component
```
