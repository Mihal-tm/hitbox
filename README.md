local player = game.Players.LocalPlayer
local char = player.Character

local currentHitboxScale = char.Head.Size.X
local defaultHitboxScale = 2.5

local function setHitboxScale(scale)
    char.Head.Size = Vector3.new(scale, scale, scale)
    char.Head.CFrame = char.Head.CFrame + Vector3.new(0, (scale - currentHitboxScale) / 2, 0)
end

local function resetHitboxScale()
    setHitboxScale(defaultHitboxScale)
end

local function onMenuButtonClicked()
    local menu = Instance.new("ScreenGui")
    local frame = Instance.new("Frame")
    local resetButton = Instance.new("TextButton")
    local smallButton = Instance.new("TextButton")
    local mediumButton = Instance.new("TextButton")
    local largeButton = Instance.new("TextButton")
    
    menu.Name = "HitboxMenu"
    menu.Parent = game.CoreGui
    
    frame.Name = "Frame"
    frame.Parent = menu
    frame.BackgroundColor3 = Color3.new(1, 1, 1)
    frame.BorderSizePixel = 0
    frame.Position = UDim2.new(0.5, -50, 0.5, -50)
    frame.Size = UDim2.new(0, 100, 0, 100)
    
    resetButton.Name = "ResetButton"
    resetButton.Parent = frame
    resetButton.BackgroundColor3 = Color3.new(0, 1, 0)
    resetButton.BorderSizePixel = 0
    resetButton.Position = UDim2.new(0, 10, 0, 10)
    resetButton.Size = UDim2.new(0, 80, 0, 20)
    resetButton.Font = Enum.Font.SourceSans
    resetButton.Text = "Reset"
    resetButton.TextColor3 = Color3.new(1, 1, 1)
    resetButton.TextSize = 14
    resetButton.MouseButton1Click:Connect(function()
        resetHitboxScale()
    end)
    
    smallButton.Name = "SmallButton"
    smallButton.Parent = frame
    smallButton.BackgroundColor3 = Color3.new(0, 0, 1)
    smallButton.BorderSizePixel = 0
    smallButton.Position = UDim2.new(0, 10, 0, 40)
    smallButton.Size = UDim2.new(0, 80, 0, 20)
    smallButton.Font = Enum.Font.SourceSans
    smallButton.Text = "Small"
    smallButton.TextColor3 = Color3.new(1, 1, 1)
    smallButton.TextSize = 14
    smallButton.MouseButton1Click:Connect(function()
        setHitboxScale(1.5)
    end)
    
    mediumButton.Name = "MediumButton"
    mediumButton.Parent = frame
    mediumButton.BackgroundColor3 = Color3.new(1, 1, 0)
    mediumButton.BorderSizePixel = 0
    mediumButton.Position = UDim2.new(0, 10, 0, 70)
    mediumButton.Size = UDim2.new(0, 80, 0, 20)
    mediumButton.Font = Enum.Font.SourceSans
    mediumButton.Text = "Medium"
    mediumButton.TextColor3 = Color3.new(1, 1, 1)
    mediumButton.TextSize = 14
    mediumButton.MouseButton1
