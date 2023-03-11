--// Settings \\--
local defaultHitboxSize = 3 -- default hitbox size
local minHitboxSize = 1 -- minimum hitbox size
local maxHitboxSize = 10 -- maximum hitbox size

--// Create UI \\--
local ui = Instance.new("ScreenGui")
local mainFrame = Instance.new("Frame")
local titleLabel = Instance.new("TextLabel")
local hitboxLabel = Instance.new("TextLabel")
local hitboxSize = Instance.new("TextBox")
local applyButton = Instance.new("TextButton")
local closeButton = Instance.new("TextButton")

--// UI Settings \\--
ui.Name = "Hitbox Changer"
ui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

mainFrame.Name = "MainFrame"
mainFrame.Parent = ui
mainFrame.BackgroundColor3 = Color3.new(0.156863, 0.156863, 0.156863)
mainFrame.BorderSizePixel = 0
mainFrame.Position = UDim2.new(0.5, -150, 0.5, -100)
mainFrame.Size = UDim2.new(0, 300, 0, 200)

titleLabel.Name = "TitleLabel"
titleLabel.Parent = mainFrame
titleLabel.BackgroundColor3 = Color3.new(1, 1, 1)
titleLabel.BackgroundTransparency = 1
titleLabel.Position = UDim2.new(0, 0, 0, 15)
titleLabel.Size = UDim2.new(1, 0, 0, 50)
titleLabel.Font = Enum.Font.SourceSansBold
titleLabel.Text = "Hitbox Changer"
titleLabel.TextColor3 = Color3.new(1, 1, 1)
titleLabel.TextScaled = true
titleLabel.TextSize = 14
titleLabel.TextWrapped = true

hitboxLabel.Name = "HitboxLabel"
hitboxLabel.Parent = mainFrame
hitboxLabel.BackgroundColor3 = Color3.new(1, 1, 1)
hitboxLabel.BackgroundTransparency = 1
hitboxLabel.Position = UDim2.new(0, 50, 0, 80)
hitboxLabel.Size = UDim2.new(0, 200, 0, 50)
hitboxLabel.Font = Enum.Font.SourceSansBold
hitboxLabel.Text = "Hitbox Size:"
hitboxLabel.TextColor3 = Color3.new(1, 1, 1)
hitboxLabel.TextScaled = true
hitboxLabel.TextSize = 14
hitboxLabel.TextWrapped = true

hitboxSize.Name = "HitboxSize"
hitboxSize.Parent = mainFrame
hitboxSize.BackgroundColor3 = Color3.new(0.156863, 0.156863, 0.156863)
hitboxSize.BorderSizePixel = 0
hitboxSize.Position = UDim2.new(0, 50, 0, 120)
hitboxSize.Size = UDim2.new(0, 200, 0, 50)
hitboxSize.Font = Enum.Font.SourceSansBold
hitboxSize.PlaceholderText = "Enter hitbox size"
hitboxSize.Text = defaultHitboxSize
hitboxSize.TextColor3 = Color3.new(1, 1, 1)
hitboxSize.TextScaled = true
hitboxSize.TextSize = 14
hitboxSize.TextWrapped = true

applyButton.Name = "ApplyButton"
applyButton.Parent = mainFrame
applyButton.BackgroundColor3 = Color3.new(0.
