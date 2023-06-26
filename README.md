# Jump
You can jump in any game that disabled the jump
Section:NewLabel("jump toggle")
local Tab = Window:NewTab("Jump")
local Window = Library.CreateLib("JUMP GUI", "DarkTheme")
label:UpdateLabel("Jump Toggle")
Section:NewButton("Jump button", "ButtonInfo", function()
    print("Clicked")
end)
Section:NewButton("jump button", "ButtonInfo", function()
    print("Clicked")
end)
getgenv().Toggled = false

local toggle = Section:NewToggle("Toggle", "Info", (state)
    getgenv().Toggled = state
end)

game:GetService("RunService").RenderStepped:Connect(function()
	if getgenv().Toggled then
		toggle:UpdateToggle("Toggle On")
	else
		toggle:UpdateToggle("Toggle Off")
	end
end)







