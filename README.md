getgenv().speed = 100  -- Adjust the speed if you're getting kicked
loadstring(game:HttpGet('https://raw.githubusercontent.com/BAG0N/OPM_DF/main/TweenTP.lua'))()

local GUI = loadstring(game:HttpGet("https://raw.githubusercontent.com/derekcool38/Dribblish/main/Source.lua"))()

local UI = GUI:CreateWindow("Mike Black Doe")

local Home = UI:addPage("Main",2,true)

Home:addToggle("AutoAttack",function(value)
_G.AutoAttack = value
 while _G.AutoAttack do 
local args = {
    [1] = 3,
    [2] = CFrame.new(Vector3.new(-9062.8330078125, -2955.572265625, -2926.6064453125), Vector3.new(-0.92950016260147, -0.30390030145645, -0.20898342132568))
}

game:GetService("ReplicatedStorage").Package.Events.Combat:FireServer(unpack(args))

local args = {
    [1] = 4,
    [2] = CFrame.new(Vector3.new(-9062.8330078125, -2955.572265625, -2926.6064453125), Vector3.new(-0.92950016260147, -0.30390030145645, -0.20898342132568))
}

game:GetService("ReplicatedStorage").Package.Events.Combat:FireServer(unpack(args))

local args = {
    [1] = 1,
    [2] = CFrame.new(Vector3.new(-9062.8330078125, -2955.572265625, -2926.6064453125), Vector3.new(-0.92950016260147, -0.30390030145645, -0.20898342132568))
}

game:GetService("ReplicatedStorage").Package.Events.Combat:FireServer(unpack(args))

local args = {
    [1] = 5,
    [2] = CFrame.new(Vector3.new(-9062.8330078125, -2955.572265625, -2926.6064453125), Vector3.new(-0.92950016260147, -0.30390030145645, -0.20898342132568))
}

game:GetService("ReplicatedStorage").Package.Events.Combat:FireServer(unpack(args))

local args = {
    [1] = 5,
    [2] = CFrame.new(Vector3.new(-9062.8330078125, -2955.572265625, -2926.6064453125), Vector3.new(-0.92950016260147, -0.30390030145645, -0.20898342132568))
}

game:GetService("ReplicatedStorage").Package.Events.Combat:FireServer(unpack(args))
wait()
end
end)

Home:addToggle("Thug",function(value)
_G.Thug = value
 while _G.Thug do 
     game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
   game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Living.Thug.HumanoidRootPart.CFrame*CFrame.new(0,-7,0) * CFrame.Angles(-80,0,0)
   wait()
 end
end)

local Home = UI:addPage("Quest",2,true)

Home:addToggle("Thug Quest",function(value)
local args = {
    [1] = "Thugs"
}

game:GetService("ReplicatedStorage").Package.Events.GetQuest:InvokeServer(unpack(args))

end)
