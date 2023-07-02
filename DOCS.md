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
KUI.Init(LocalPlayer.PlayerGui,50,20)
```
```
**Parameters:**
1 | object | PlayerGui
2 | number | Line width in offset
3 | number | Blur size
```

## Component: Window
```lua
local Window = KUI.Window.new("Test1")
```
```
**Parameters:**
1 | string | Name
```
```
**Methods:**

```
