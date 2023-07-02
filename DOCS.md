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
METHODS:
:GetCurrentPage()
>>> <number> CurrentPage

:SetHeader( <string> title , <table> closeButtonInfo )
>>> <object> 

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

EVENTS:
.Events.OnShow

.Events.OnHide

.Events.OnClose
```

## Component: Line
```lua
local newLine = KUI.Line.new( <string> name , <number> layoutIndex )
```
```lua
METHODS:
:SetEnabled( <boolean> statement (true/false) )
>>> <object> Line

:SetLineLayout( <number> layoutIndex )
>>> <object> Line

:AddComponent( <object> component )
>>> <object> Component

EVENTS:
.Events.OnEnable

.Events.OnDisable

.Events.OnChangeLineLayout
```

## Component: InputText
```lua
local newInputText = KUI.InputText.new( <string> placeholderText , <string> defaultText , <number> textFontSize , <boolean> editableText (true/false) )
```
```lua
METHODS:
:SetComponentLayout( <number> layoutIndex )
>>> <object> InputText

:SetSizeOperator( <number> sizeOperator )
>>> <object> InputText

:SetPlaceholderText( <string> text )
>>> <object> InputText

:SetText( <string> text )
>>> <object> InputText

:SetEnabled( <boolean> statement )
>>> <object> InputText

:GetText()
>>> <string> text

EVENTS:
.Events.OnFocused

.Events.OnFocusLost

.Events.OnChangeComponentLayout
```

## Component: Button
```lua
local exampleButton = KUI.Button.new( <string> defaultText , <number> textFontSize , <boolean> clickableButton (true/false) )
```
```lua
METHODS:
:SetComponentLayout( <number> layoutIndex )
>>> <object> Button

:SetSizeOperator( <number> sizeOperator )
>>> <object> Button

:SetText( <string> text )
>>> <object> Button

EVENTS:
.Events.OnClick

.Events.OnChangeComponentLayout
```

## Component: Label
```lua
local exampleLabel = KUI.Label.new( <string> defaultText , <number> textFontSize )
```
```lua
METHODS:
:SetComponentLayout( <number> layoutIndex )
>>> <object> Label

:SetSizeOperator( <number> sizeOperator )
>>> <object> Label

:SetTextAlignment( <Enum.TextXAlignment> x_alignment , <Enum.TextYAlignment> y_alignment )
>>> <object> Label

:SetText( <string> text )
>>> <object> Label

EVENTS:
.Events.OnChangeComponentLayout
```
