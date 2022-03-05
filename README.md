local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Pittboom666 HUB", "DarkTheme")

local Tab = Window:NewTab("MAIN MENU")
local SectionX = Tab:NewSection("XD")

local Tab = Window:NewTab("AUTO FARM")
local Section = Tab:NewSection("Script")
--------------------------------------------
Section:NewButton("RIVER HUB", "RIVER HUB", function()
    pcall(function()
   loadstring(game:HttpGet("http://riverhub.xyz/" .. tostring(game.PlaceId) .. ".lua"))()
end)
end)

local Tab = Window:NewTab("TELEPORT")
local Section = Tab:NewSection("TELEPORT PLAYER") 

players = {}
 
for i,v in pairs(game:GetService("Players"):GetChildren()) do
   table.insert(players,v.Name)
end
 
Section:NewDropdown("Select Player", " ", players, function(abc)
    Select = abc
end)
 
--------------------------------------------------------- 

Section:NewButton("Refresh", " ", function()
    table.clear(players)
for i,v in pairs(game:GetService("Players"):GetChildren()) do
   table.insert(players,v.Name)
end
end)
 
Section:NewButton("Teleport", " ", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players[Select].Character.HumanoidRootPart.CFrame
end)

local Section = Tab:NewSection("World 1")
local Section = Tab:NewSection("Map")
--------------------------------------------
Section:NewButton("Spawn", "....", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-686.761902, 51.1999855, -620.252686, 0.0486828275, 1.7901062e-08, 0.998814285, 7.14462445e-08, 1, -2.14046469e-08, -0.998814285, 7.24035729e-08, 0.0486828275)
end)
---------------------------------------------
Section:NewButton("Story", "....", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(49.8495255, 1387.99963, 838.557495, 0.998389542, -3.00830649e-08, 0.0567297526, 3.11547907e-08, 1, -1.80074071e-08, -0.0567297526, 1.97458121e-08, 0.998389542)
end)
---------------------------------------------
Section:NewButton("Orb", "....", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-862.545776, 46.9666519, -809.66333, -0.752968132, -7.3325765e-08, 0.658056974, -1.92348928e-08, 1, 8.9418549e-08, -0.658056974, 5.46716628e-08, -0.752968132)
end)
---------------------------------------------
Section:NewButton("infinite", "....", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-142.493744, 1387.99963, 838.829163, 0.999710679, 1.23114825e-08, 0.024053229, -1.44713663e-08, 1, 8.9621949e-08, -0.024053229, -8.9944109e-08, 0.999710679)
end)
---------------------------------------------
local Section = Tab:NewSection("TRIAL")

Section:NewButton("TRIAL 1", "....", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-244.839844, 63.160717, -823.334961, 0.522527933, 0.0684481263, -0.849870205, -1.08378959e-08, 0.996772408, 0.0802795514, 0.852622151, -0.0419482999, 0.52084142)
end)
---------------------------------------------
Section:NewButton("TRIAL 2", "....", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-505.129822, 107.907372, -896.952637, -0.991446078, 0.032788787, -0.126331002, 7.54329843e-09, 0.967929304, 0.251222759, 0.130516768, 0.249073818, -0.959649742)
end)
---------------------------------------------
Section:NewButton("TRIAL 3", "....", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-766.489197, 173.220016, -900.701782, 0.979928434, -0.00641799252, 0.199246317, 9.60626423e-09, 0.999481618, 0.0321946032, -0.199349657, -0.0315484069, 0.979420424)
end)
---------------------------------------------
local Section = Tab:NewSection("RAID")

Section:NewButton("Raid 1", "....", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-933.88501, 182.697098, -779.966797, 0.681992292, -0.0137211829, 0.731230617, -9.17307208e-09, 0.999823987, 0.0187612139, -0.731359363, -0.0127950097, 0.681872249)
end)
---------------------------------------------
Section:NewButton("Raid 2", "....", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1041.88745, 199.102463, -608.118591, 0.147827297, -0.0716644004, 0.98641336, -9.55916509e-12, 0.997371256, 0.0724605098, -0.989013195, -0.010711642, 0.147438705)
end)
---------------------------------------------
Section:NewButton("Raid 3", "....", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-935.090393, 201.344772, -379.07019, -0.874614239, -0.0610562526, 0.480959535, 9.12264042e-09, 0.992038369, 0.125936076, -0.484819472, 0.110145487, -0.867650867)
end)
---------------------------------------------
local Section = Tab:NewSection("CHALLENGE")


Section:NewButton("CHALLENGE 1", "....", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-770.65271, 247.240448, -262.594238, -0.948309064, -0.0568297282, 0.312218338, -6.69288669e-09, 0.983835101, 0.17907685, -0.317348242, 0.169820204, -0.932979763)
end)
---------------------------------------------
Section:NewButton("CHALLENGE 2", "....", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-552.345642, 290.186981, -198.980408, -0.986292481, 0.0152723789, -0.164298326, -6.67926026e-09, 0.995707452, 0.0925562009, 0.165006623, 0.0912874863, -0.982058764)
end)
---------------------------------------------
Section:NewButton("CHALLENGE 3", "....", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-449.135193, 302.050934, -426.433319, 0.207861006, 0.168694109, -0.96350199, 4.17719326e-09, 0.985016346, 0.172460943, 0.978158355, -0.035847906, 0.204746485)
end)
---------------------------------------------
