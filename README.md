# Getting the ui libary started
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/YungPloits/UILib/main/UICode"))()
local Lib = Library.CreateLib() -- this is NEEDED
```




# To create a new tab in your UI:

```lua
local myTab = Lib:Tab("MyTabName", "5009915812")
```



# To add a section to the tab:

```lua
local mySection = myTab:Section("MySectionName")
```


# To add a button to the section:

```lua
mySection:Button("Click Me", function()
    print("Button Clicked!")
end, "This is a button description")
```


# To add a toggle switch to the section:

```lua
mySection:Toggle("Enable Feature", false, function(state)
    print("Toggle state: ", state)
end, "This is a toggle description", false)
```


# To add a dropdown menu to the section:

```lua
mySection:Dropdown("Choose Option", {"Option1", "Option2", "Option3"}, function(selected)
    print("Selected option: ", selected)
end, "This is a dropdown description")
```


# To add a text box to the section:

```lua
mySection:TextBox("Enter Text", function(text)
    print("Entered text: ", text)
end, "This is a text box description")
```

# To add a keybind to the section:

```lua
mySection:Keybind("Set Keybind", Enum.KeyCode.E, function()
    print("Keybind activated!")
end, "This is a keybind description", {Enum.KeyCode.LeftShift})
```


# To add a slider to the section:

```lua
mySection:Slider("Adjust Value", 0, 100, 50, function(value)
    print("Slider value: ", value)
end, false, "This is a slider description")
```


# To add a label to the section:

```lua
mySection:Label("This is a label text")
```


# To create a notification:

```lua
Library:Notification("Notification Title", "Desc of noti", 2.5)
```
