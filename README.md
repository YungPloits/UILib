Example Usage
Getting the ui libary started
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/YungPloits/UILib/main/hi"))()
local Lib = Library.CreateLib() -- this is NEEDED
```


Creating a Tab

To create a new tab in your UI:

```lua
local myTab = Lib:Tab("MyTabName", "5009915812")
```

Creating a Section

To add a section to the tab:

```lua
local mySection = myTab:Section("MySectionName")
```

Adding a Button

To add a button to the section:

```lua
mySection:Button("Click Me", function()
    print("Button Clicked!")
end, "This is a button description")
```

Adding a Toggle

To add a toggle switch to the section:

```lua
mySection:Toggle("Enable Feature", true, function(state)
    print("Toggle state: ", state)
end, "This is a toggle description", true)
```

Adding a Dropdown

To add a dropdown menu to the section:

```lua
mySection:Dropdown("Choose Option", {"Option1", "Option2", "Option3"}, function(selected)
    print("Selected option: ", selected)
end, "This is a dropdown description")
```

Adding a TextBox

To add a text box to the section:

```lua
mySection:TextBox("Enter Text", function(text)
    print("Entered text: ", text)
end, "This is a text box description")
```
Adding a Keybind

To add a keybind to the section:

```lua
mySection:Keybind("Set Keybind", Enum.KeyCode.E, function()
    print("Keybind activated!")
end, "This is a keybind description", {Enum.KeyCode.LeftShift})
```

Adding a Slider

To add a slider to the section:

```lua
mySection:Slider("Adjust Value", 0, 100, 50, function(value)
    print("Slider value: ", value)
end, false, "This is a slider description")
```

Adding a Label

To add a label to the section:

```lua
mySection:Label("This is a label text")
```

Creating a Notification

To create a notification:

```lua
Library:Notification("Notification Title", "This is the notification info", 5, {"Okay"})
```
