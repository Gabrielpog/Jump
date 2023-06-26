# Jump
You can jump in any game that disabled the jump
Section:NewLabel("jump toggle")
local Tab = Window:NewTab("Jump")
local Window = Library.CreateLib("JUMP GUI", "DarkTheme")
label:UpdateLabel("Jump Toggle")
Section:NewButton("Jump button", "ButtonInfo", function()
    print("Clicked")
end)
