# KYRYLO-UI
**KYRYLO-UI** is a library for the Roblox Studio engine, written in the Luau language. With KYRYLO-UI, developers can create interfaces for their games quickly and easily. This library aims to simplify the process of UI development by providing a set of intuitive and efficient tools.

## Features
* **Simple and intuitive API**: KYRYLO-UI offers an easy-to-use interface, allowing developers to create UI elements without excessive complexity.
  
* **Fast and efficient rendering**: The library is designed to provide optimal performance, ensuring smooth and responsive UI updates.
  
* **Customizability**: KYRYLO-UI provides a range of customization options, allowing developers to tailor the appearance and behavior of their UI elements to match the style of their game.
  
* **Event-driven programming**: The library utilizes event-driven programming paradigms, enabling developers to create interactive UI elements that respond to user actions.
  
* **Documentation and examples**: Comprehensive documentation and examples are provided to help developers get started quickly and make the most of the library's features.

## Previews
![image](https://github.com/KIRILLUSHKA123/KYRYLO-UI/assets/60113306/22cfb44e-2763-41de-bee7-2b8530efdf34)


## Installation
* **Download** <a href="https://github.com/KIRILLUSHKA123/KYRYLO-UI/edit/main/README.md">any release of KYRYLO-UI</a>
* **Place** this module script in **ReplicatedStorage**
* ![image](https://github.com/KIRILLUSHKA123/KYRYLO-UI/assets/60113306/5dc4d278-8f4d-44c0-8152-56d5911cb06b)
* **Create** new local script in **StarterPlayerScripts** or **StarterGui**
* ![image](https://github.com/KIRILLUSHKA123/KYRYLO-UI/assets/60113306/7946c5fe-3348-4ed6-bb1c-74d7933269ce)
* **Create** your first window:
```lua
local ReplicatedStorage = game:GetService("ReplicatedStorage")
local Players = game:GetService("Players")

local LocalPlayer = Players.LocalPlayer

local KUI = require(ReplicatedStorage.KUI_Library)

KUI.Init(LocalPlayer.PlayerGui,50,20)

local Window = KUI.Window.new("Test1")

Window:Show()

Window:SetCorner(10)
Window:SetHeader("Test Window",{true,"close"})

local firstLine = KUI.Line.new("MyFirstLine",3)
local secondLine = KUI.Line.new("MySecondLine",2)

Window:SetLines( { firstLine, secondLine } )

local nameInput = KUI.InputText.new("Your Name:")
local changeNameButton = KUI.Button.new("Change Name")

nameInput:SetSizeOperator(8)
changeNameButton:SetSizeOperator(5)

firstLine:AddComponent( nameInput )
secondLine:AddComponent( changeNameButton )
```

## Contributing
* **Discord**: @kyrylo.
* **Email**: kirilljbicai@gmail.com

