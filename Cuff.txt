local Char = game.Players.LocalPlayer.Character
    local Hum = Char:FindFirstChildOfClass("Humanoid") or Char:FindFirstChildOfClass("AnimationController")

    for i,v in next, Hum:GetPlayingAnimationTracks() do
       if v.Animation.AnimationId == "rbxassetid://3144026747" then
           v:Stop(2)
           wait(2)
           game.Players.LocalPlayer.Character.RightLowerArm:FindFirstChild("CUFF"):Destroy()
    game.Players.LocalPlayer.Character.LeftLowerArm:FindFirstChild("CUFF"):Destroy()
    game:GetService("Players").LocalPlayer.PlayerGui.MainScreenGuiTimerJail:Destroy()
    game.Players.LocalPlayer.Character.BodyEffects:FindFirstChild("Cuff"):Destroy()
    end
end