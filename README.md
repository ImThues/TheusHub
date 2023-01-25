local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "Key", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})

https://github.com/ImThues/TheusHub.git

getgenv().KeyInput = "Theus Hub"
	function Destroy()
		game:GetService("CoreGui").Orion:Destroy()
end

function CheckKey()
	if sf_key == KeyInput then
		local Window = OrionLib:MakeWindow({Name = "Key", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})
	end
end

local Tab = Window:MakeTab({
	Name = "Key",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

local Section = Tab:AddSection({
	Name = "Key"
})

Tab:AddLabel("Entre no meu discord para pega a key")
Tab:AddLabel("https://discord.gg/qsu9ahFn")

Tab:AddTextbox({
	Name = "Key",
	Default = "",
	TextDisappear = true,
	Callback = function(Value)
		KeyInput = Value
	end	  
})

Tab:AddButton({
	Name = "Check Key",
	Callback = function()
      		CheckKey()
  	end    
})
