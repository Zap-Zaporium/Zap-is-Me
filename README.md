# Zap-is-Me
# Zaporium — Neon Blue Minimalist GUI Library

Simple, beautiful, reusable Roblox UI library.

## How to Use (Examples)

Just copy and paste these snippets!

### Create a Window
```lua
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Zap-Zaporium/Zap-is-Me/refs/heads/main/Zaporium.lua"))()

local window = library:CreateWindow("My Cool GUI")

### Create a button
window:AddButton({
    text = "Kill All",
    callback = function()
        print("Everyone died!")
    end
})

window:AddToggle({
    text = "God Mode",
    state = true,        -- default on
    flag = "godmode",    -- optional: save state
    callback = function(value)
        print("God Mode:", value)
    end
})
