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
1 | object | PlayerGui
2 | number | Window size in offset
3 | number | Blur size
```
