-- Madcity Godmode (LocalPlayer)

local this_guy_has_godmode = game.Players.LocalPlayer.Name
_G.God = true -- On/Off
while _G.God and wait() do
       pcall(function()
           local A_1 = "RevivePlayer"
           local A_2 = game:GetService("Workspace")[this_guy_has_godmode]
           local A_3 = game:GetService("Workspace").ObjectSelection.DownedPart.DownedPart
           local Event = game:GetService("ReplicatedStorage").Event
           Event:FireServer(A_1, A_2, A_3)
           end)
end
