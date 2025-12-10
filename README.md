# Zaporium Library
**Simple • Clean • Neon Blue Minimalist UI Library**  
Made with love by **Zap-Zaporium**  

![Preview](https://i.imgur.com/EXAMPLE_PREVIEW.png) *(replace with your own screenshot later)*

### Setup The Library
```lua
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Zap-Zaporium/Zap-is-Me/refs/heads/main/Zaporium.lua"))()

### Adding Tab/window
```lua
local tab = library:CreateWindow("Zaporium UI")
```



### Adding Folder
```lua
local folder = tab:AddFolder("Main Features")
```



### Adding Button
```luafolder:AddButton({
    text = "Click Me",
    flag = "my_button",
    callback = function()
        print("Button clicked!")
    end
})
})
```




### Adding Toggle
```lua
folder:AddToggle({
    text = "Toggle Feature",
    flag = "my_toggle",
    state = false,
    callback = function(value)
        print("Toggle is now:", value)
    end
})
```




### Adding Label
```lua
folder:AddLabel({
    text = "Zaporium is the best!"
})
```





### Adding Slider
```lua
folder:AddSlider({
    text = "Speed",
    min = 16,
    max = 500,
    value = 100,
    float = 1,
    flag = "speed_slider",
    callback = function(value)
        print("Speed set to:", value)
    end
})
```





### Adding TextBox
```lua
folder:AddBox({
    text = "Enter Name",
    value = "Player",
    flag = "player_name",
    callback = function(text, enterPressed)
        if enterPressed then
            print("Submitted:", text)
        end
    end
})
```





### Adding Dropdown
```lua
folder:AddList({
    text = "Choose Mode",
    values = {"Combat", "Movement", "Visuals", "Misc"},
    value = "Combat",
    flag = "mode_list",
    callback = function(selected)
        print("Mode changed to:", selected)
    end
})
```





### Adding Bind
```lua
folder:AddBind({
    text = "Toggle GUI",
    key = Enum.KeyCode.Insert,
    hold = false,
    flag = "gui_bind",
    callback = function()
        library:Close() -- Toggles visibility
    end
})
```

### Close Lib
```lua
library:Close()
```



### Final (REQUIRED OR THE UI WILL NOT SHOW)
```lua
library:Init()
```


### Credits : Tora Is Me
