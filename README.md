local UILibrary = loadstring(game:HttpGet("https://pastebin.com/raw/V1ca2q9s"))()

local MainUI = UILibrary.Load("Size Legends Simulator")
local FirstPage = MainUI.AddPage("Farming")

local FirstLabel = FirstPage.AddLabel("Farming")
local FirstToggle = FirstPage.AddToggle("Auto Fast-Weigth [InGroup]", false, function(Value)
_G.Weigth = Value
while _G.Weigth do wait(0.5)
local Event = game:GetService("Players").b82zf9y.PlayerGui.PlayersGui.Top.AutoClick.InGroupStart
Event:FireServer()

end
end)

local FirstToggle = FirstPage.AddToggle("Auto Slow-Weigth [Normal]", false, function(Value)
_G.Weigth1 = Value
while _G.Weigth1 do wait()
    local vu = game:GetService("VirtualUser")
vu:ClickButton1(Vector2.new(100000,100000))
end
end)

local FirstLabel = FirstPage.AddLabel("[Shop-Tp]")

local FirstDropdown = FirstPage.AddDropdown("Select : >", {
"Sell",
"Upgrade",
"BoostArea",
"CoinArea",

}, function(Value)
if Value == "Sell" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-111.847488, -16.3379364, 2043.90039, 1, 0, 0, 0, 1, 0, 0, 0, 1)
elseif Value == "Upgrade" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-77.4786911, -22.974577, 2088.65967, 1, 0, 0, 0, 1, 0, 0, 0, 1)
elseif Value == "BoostArea" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-140.024429, 78.8747559, 2114.63721, 1, 0, 0, 0, 1, 0, 0, 0, 1)
elseif Value == "CoinArea" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-328.544373, 78.8747559, 2057.74707, 1, 0, 0, 0, 1, 0, 0, 0, 1)

end
end)

local FirstPage = MainUI.AddPage("Zone")

local FirstLabel = FirstPage.AddLabel("Zone - TP")

local FirstDropdown = FirstPage.AddDropdown("Select : >", {
"x2 Str - [500 Need]",
"x3 Str - [2.5K Need]",
"x5 Str - [20K Need]",
"x10 Str - [150K Need]",
"x20 Str - [4.5M Need]",
"x50 Str - [2.5B Need]",
"x100 Str - [20B Need]",
"x150 Str - [800B Need]",
"x195 Str - [550T Need]",
"x275 Str - [650Qa Need]",
"x375 Str - [125Qi Need]",
"x450 Str - [15Sx Need]",
"x650 Str - [49Sp Need]",

}, function(Value)
if Value == "x2 Str - [500 Need]" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-179,-28,2260)
elseif Value == "x3 Str - [2.5K Need]" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-53,-28,2511)
elseif Value == "x5 Str - [20K Need]" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-240,-28,2400)
elseif Value == "x10 Str - [150K Need]" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-420,-28,2301)
elseif Value == "x20 Str - [4.5M Need]" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-834,27,2610)
elseif Value == "x50 Str - [2.5B Need]" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-799,-27,1788)
elseif Value == "x100 Str - [20B Need]" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-203,-28,1786)
elseif Value == "x150 Str - [800B Need]" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-92,-27,2920)
elseif Value == "x195 Str - [550T Need]" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(210,-28,2251)
elseif Value == "x275 Str - [650Qa Need]" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(230,-28,1990)
elseif Value == "x375 Str - [125Qi Need]" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(138,-23,1756)
elseif Value == "x450 Str - [15Sx Need]" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-578,-28,2954)
elseif Value == "x650 Str - [49Sp Need]" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-847,29,2212)

end
end)

repeat wait() until game:IsLoaded()
game:GetService("Players").LocalPlayer.Idled:connect(function()
game:GetService("VirtualUser"):ClickButton2(Vector2.new())
end)
