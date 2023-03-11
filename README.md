local hitbox = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChildOfClass("Part")
local menu = Instance.new("ScreenGui")
local main = Instance.new("Frame")
local title = Instance.new("TextLabel")
local hitboxText = Instance.new("TextLabel")
local hitboxSlider = Instance.new("TextButton")
local rangeText = Instance.new("TextLabel")
local rangeSlider = Instance.new("TextButton")

menu.Name = "Hitbox Menu"
menu.Parent = game.CoreGui
menu.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

main.Name = "Main"
main.Parent = menu
main.BackgroundColor3 = Color3.fromRGB(22, 22, 22)
main.BorderColor3 = Color3.fromRGB(27, 42, 53)
main.Position = UDim2.new(0.7, 0, 0.4, 0)
main.Size = UDim2.new(0, 150, 0, 200)

title.Name = "Title"
title.Parent = main
title.BackgroundColor3 = Color3.fromRGB(22, 22, 22)
title.BorderColor3 = Color3.fromRGB(27, 42, 53)
title.Size = UDim2.new(1, 0, 0, 30)
title.Font = Enum.Font.SourceSansBold
title.Text = "Hitbox Menu"
title.TextColor3 = Color3.fromRGB(255, 255, 255)
title.TextSize = 18

hitboxText.Name = "HitboxText"
hitboxText.Parent = main
hitboxText.BackgroundColor3 = Color3.fromRGB(22, 22, 22)
hitboxText.BorderColor3 = Color3.fromRGB(27, 42, 53)
hitboxText.Position = UDim2.new(0, 0, 0, 40)
hitboxText.Size = UDim2.new(1, 0, 0, 20)
hitboxText.Font = Enum.Font.SourceSans
hitboxText.Text = "Hitbox Scale"
hitboxText.TextColor3 = Color3.fromRGB(255, 255, 255)
hitboxText.TextSize = 14

hitboxSlider.Name = "HitboxSlider"
hitboxSlider.Parent = main
hitboxSlider.BackgroundColor3 = Color3.fromRGB(51, 51, 51)
hitboxSlider.BorderColor3 = Color3.fromRGB(27, 42, 53)
hitboxSlider.Position = UDim2.new(0.1, 0, 0, 70)
hitboxSlider.Size = UDim2.new(0.8, 0, 0, 20)
hitboxSlider.Font = Enum.Font.SourceSans
hitboxSlider.Text = ""
hitboxSlider.TextColor3 = Color3.fromRGB(0, 0, 0)
hitboxSlider.TextSize = 14

rangeText.Name = "RangeText"
rangeText.Parent = main
rangeText.BackgroundColor3 = Color3.fromRGB(22, 22, 22)
rangeText.BorderColor3 = Color3.fromRGB(27, 42, 53)
rangeText.Position = UDim2.new(0, 0, 0, 100)
rangeText.Size = UDim2.new(1, 0, 0, 20)
rangeText.Font = Enum.Font.SourceSans
rangeText.Text = "Hitbox Range"
rangeText.TextColor3 = Color3.fromRGB(255
