local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "Theus hub", HidePremium = false, SaveConfig = true, IntroEnabled = false})

_G.AutoAtk = true

function AutoAtk()
    while _G.AutoAtk == true do
game:GetService("ReplicatedStorage").Remotes.Combat:FireServer()
wait(0000000000000000.1)
    end
end

local Tab = Window:MakeTab({
	Name = "Super Saiyan",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

local Section = Tab:AddSection({
	Name = "Auto-Farm"
})

Tab:AddToggle({
	Name = "Auto Ataque",
	Default = false,
	Callback = function(Value)
		print(Value)
	_G.AutoAtk = Value
    AutoAtk()
    end    
})

local Section = Tab:AddSection({
	Name = "Transformacao"
})

Tab:AddButton({
	Name = "SSJGalaxy",
	Callback = function()
      		print("button pressed")
		game:GetService("ReplicatedStorage").ModeEvents.SSJGalaxyOn:FireServer()
  	end    
})

Tab:AddButton({
	Name = "SSJOmega",
	Callback = function()
      		print("button pressed")
		game:GetService("ReplicatedStorage").ModeEvents.SSJOmegaOn:FireServer()
  	end    
})

Tab:AddButton({
	Name = "SSJE",
	Callback = function()
      		print("button pressed")
		game:GetService("ReplicatedStorage").ModeEvents.SSJEOn:FireServer()
  	end    
})

Tab:AddButton({
	Name = "FLSSJ",
	Callback = function()
      		print("button pressed")
		game:GetService("ReplicatedStorage").ModeEvents.FLSSJOn:FireServer()
  	end    
})

Tab:AddButton({
	Name = "SSJRG",
	Callback = function()
      		print("button pressed")
		game:GetService("ReplicatedStorage").ModeEvents.SSJRGOn:FireServer()
  	end    
})

Tab:AddButton({
	Name = "SSJGK",
	Callback = function()
      		print("button pressed")
		game:GetService("ReplicatedStorage").ModeEvents.SSJGKOn:FireServer()
  	end    

})Tab:AddButton({
	Name = "SSJbeast",
	Callback = function()
      		print("button pressed")
		game:GetService("ReplicatedStorage").ModeEvents.SSJBeastOn:FireServer()
  	end    
})

local Tab = Window:MakeTab({
	Name = "Super Saiyan 2",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})



local Section = Tab:AddSection({
	Name = "INDEFINIDO"
})

Tab:AddButton({
	Name = "Kill",
	Callback = function()
      		print("button pressed")
			
		end    
})

local Tab = Window:MakeTab({
	Name = "Brookhaven",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

local Section = Tab:AddSection({
	Name = "Scripts"
})

Tab:AddButton({
	Name = "IceHub",
	Callback = function()
      		print("button pressed")
    loadstring(game:HttpGet("https://icehub.cf/IceHubLoader"))()
  	end    
})

local Tab = Window:MakeTab({
	Name = "Outros",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

local Section = Tab:AddSection({
	Name = "Scripts"
})

Tab:AddButton({
	Name = "Infinite Yield",
	Callback = function()
      		print("button pressed")
    	loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
  	end    
})

Tab:AddButton({
	Name = "Templehook",
	Callback = function()
      		print("button pressed")
        loadstring(game:HttpGet('https://bifao.tech/templehook/loader.lua'))()
  	end    
})

local Section = Tab:AddSection({
	Name = "WalkSpeed"
})

Tab:AddButton({
	Name = "Aumentar Velocidade",
	Callback = function()

		local character = game.Players.LocalPlayer.Character
		local humanoid = character.Humanoid
		
		humanoid.WalkSpeed = 100
	end
})

Tab:AddButton({
	Name = "Abaixar Velocidade",
	Callback = function()

		local character = game.Players.LocalPlayer.Character
		local humanoid = character.Humanoid
		
		humanoid.WalkSpeed = 16
	end
})

local Section = Tab:AddSection({
	Name = "JumpPower"
})

Tab:AddButton({
	Name = "Aumentar Pulo",
	Callback = function()

		local character = game.Players.LocalPlayer.Character
		local humanoid = character.Humanoid
		
		humanoid.JumpPower = 100
	end
})

Tab:AddButton({
	Name = "Diminuir Pulo",
	Callback = function()

		local character = game.Players.LocalPlayer.Character
		local humanoid = character.Humanoid
		
		humanoid.JumpPower = 40
	end
})

local Section = Tab:AddSection({
	Name = "Super Human"
})

Tab:AddButton({
	Name = "Super Human",
	Callback = function()
			print = ("button pressed")
		game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 200
		game.Players.LocalPlayer.Character.Humanoid.JumpPower = 100
	end
})

local Section = Tab:AddSection({
	Name = "Tp"
})

Tab:AddButton({
	Name = "Tp",
	Callback = function()
			print = ("button pressed")
			game.Players.LocalPlayer.character.HumanoidRootPart.CFrame = CFrame.new(-983.659912, -360.809326, 117.255722, 0, -1, 0, 1, 0, -0, 0, 0, 1)
	end
})
