-- MESSI HUB

-- Complete Script with Script Data Structure

-- Script Data Structure

local buttonsPagesData = {

    {Text = "AUTO GRAB TOOLS", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "INSTANT SPAWN", ScriptLink = "https://pastebin.com/raw/20TaKpzj"},

    {Text = "LOOPBRING", ScriptLink = "https://pastebin.com/raw/cMaUmR6d"},

    {Text = "USETOOLS", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "FPS", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "LAG", ScriptLink ="https://pastebin.com/raw/p8Gi1nZa"},

    {Text = "NO COOLDOWN", ScriptLink = "https://pastebin.com/raw/RT2nvfub"},

    {Text = "USE TOOLS", ScriptLink = "https://pastebin.com/raw/PhQc5TvG"},

    {Text = "INSTA-KILL", ScriptLink = "https://pastebin.com/raw/fwTDvFbT"},

    {Text = "GET TOOLS V5", ScriptLink = "https://pastebin.com/raw/JVuvBaPZ"},

    {Text = "NO COOLDOWN V9", ScriptLink = "https://pastebin.com/raw/Sv8Dcb4r"},

    {Text = "NO COOLDOWN", ScriptLink = "https://pastebin.com/raw/vkHMNBK9"},

    {Text = "SPEED", ScriptLink = "https://pastebin.com/raw/CDP7V3f2"},

    {Text = "HITBOX", ScriptLink = "https://pastebin.com/raw/aNay6q2J"},

    {Text = "GET BASE", ScriptLink = "https://pastebin.com/raw/Mu2XGsxD"},

    {Text = "SCRIPT 16", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 17", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 18", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 19", ScriptLink ="https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 20", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 21", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 22", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 23", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 24", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 25", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 26", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 27", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 28", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 29", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"},

    {Text = "SCRIPT 30", ScriptLink = "https://pastebin.com/raw/TkCL2MhS"}

}

local Players = game:GetService("Players")

local TweenService = game:GetService("TweenService")

local player = Players.LocalPlayer

local playerGui = player:WaitForChild("PlayerGui")

local screenGui = Instance.new("ScreenGui")

screenGui.Name = "MESSI HUB"

screenGui.Parent = playerGui

screenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

screenGui.IgnoreGuiInset = true

local mainFrame = Instance.new("Frame")

mainFrame.Name = "MainFrame"

mainFrame.Parent = screenGui

mainFrame.BackgroundColor3 = Color3.fromRGB(80, 0, 0)

mainFrame.BorderColor3 = Color3.fromRGB(149, 6, 6)

mainFrame.BorderSizePixel = 3

mainFrame.Position = UDim2.new(0.5, -240, 0.5, -180)

mainFrame.Size = UDim2.new(0, 480, 0, 360)

mainFrame.Active = true

mainFrame.Draggable = true

mainFrame.Visible = false -- start hidden for toggle effect

local bloodGradient = Instance.new("UIGradient")

bloodGradient.Color = ColorSequence.new{

    ColorSequenceKeypoint.new(0, Color3.fromRGB(149, 6, 6)),

    ColorSequenceKeypoint.new(0.35, Color3.fromRGB(190, 19, 32)),

    ColorSequenceKeypoint.new(0.7, Color3.fromRGB(110, 8, 15)),

    ColorSequenceKeypoint.new(1, Color3.fromRGB(60, 0, 0)),

}

bloodGradient.Rotation = 45

bloodGradient.Parent = mainFrame

local mainCorner = Instance.new("UICorner")

mainCorner.CornerRadius = UDim.new(0, 20)

mainCorner.Parent = mainFrame

local titleFrame = Instance.new("Frame")

titleFrame.Name = "TitleFrame"

titleFrame.Parent = mainFrame

titleFrame.BackgroundColor3 = Color3.fromRGB(110, 8, 15)

titleFrame.BorderColor3 = Color3.fromRGB(149, 6, 6)

titleFrame.BorderSizePixel = 2

titleFrame.Size = UDim2.new(1, 0, 0, 50)

titleFrame.ZIndex = 5

local titleGradient = Instance.new("UIGradient")

titleGradient.Color = ColorSequence.new{

    ColorSequenceKeypoint.new(0, Color3.fromRGB(149, 6, 6)),

    ColorSequenceKeypoint.new(0.5, Color3.fromRGB(100, 0, 0)),

    ColorSequenceKeypoint.new(1, Color3.fromRGB(80, 0, 0)),

}

titleGradient.Rotation = 90

titleGradient.Parent = titleFrame

local titleCorner = Instance.new("UICorner")

titleCorner.CornerRadius = UDim.new(0, 20)

titleCorner.Parent = titleFrame

local titleLabel = Instance.new("TextLabel")

titleLabel.Name = "TitleLabel"

titleLabel.Parent = titleFrame

titleLabel.BackgroundTransparency = 1

titleLabel.Position = UDim2.new(0, 10, 0, 0)

titleLabel.Size = UDim2.new(1, -20, 1, 0)

titleLabel.Font = Enum.Font.GothamBold

titleLabel.Text = "MESSI HUB"

titleLabel.TextColor3 = Color3.fromRGB(245, 245, 245)

titleLabel.TextScaled = true

titleLabel.TextStrokeTransparency = 0.2

titleLabel.TextStrokeColor3 = Color3.fromRGB(149, 6, 6)

titleLabel.ZIndex = 6

local glow1 = Instance.new("UIStroke")

glow1.Parent = titleLabel

glow1.Thickness = 6

glow1.Color = Color3.fromRGB(255, 0, 0)

glow1.Transparency = 0.5

local glow2 = Instance.new("UIStroke")

glow2.Parent = titleLabel

glow2.Thickness = 4

glow2.Color = Color3.fromRGB(139, 0, 0)

glow2.Transparency = 0.3

-- Animate glow

spawn(function()

    while screenGui.Parent do

        TweenService:Create(glow1, TweenInfo.new(2, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut, -1), {Transparency = 0.1}):Play()

        TweenService:Create(glow2, TweenInfo.new(2, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut, -1), {Transparency = 0.05}):Play()

        wait(2)

        TweenService:Create(glow1, TweenInfo.new(2, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut, -1), {Transparency = 0.5}):Play()

        TweenService:Create(glow2, TweenInfo.new(2, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut, -1), {Transparency = 0.3}):Play()

        wait(2)

    end

end)

-- Blood drip from title downward

spawn(function()

    while screenGui.Parent do

        wait(0.25)

        local drip = Instance.new("Frame")

        drip.Size = UDim2.new(0, math.random(5, 8), 0, math.random(15, 25))

        local dripX = titleLabel.AbsolutePosition.X + math.random(10, titleLabel.AbsoluteSize.X - 15)

        local dripY = titleFrame.AbsolutePosition.Y + titleFrame.AbsoluteSize.Y - mainFrame.AbsolutePosition.Y

        drip.Position = UDim2.new(0, dripX - mainFrame.AbsolutePosition.X, 0, dripY)

        drip.BackgroundColor3 = Color3.fromRGB(255, 0, 0)

        drip.BorderSizePixel = 0

        drip.ZIndex = 7

        drip.Parent = mainFrame

        local dripCorner = Instance.new("UICorner")

        dripCorner.CornerRadius = UDim.new(0, drip.Size.X.Offset / 2)

        dripCorner.Parent = drip

        local targetY = mainFrame.AbsoluteSize.Y

        local tween = TweenService:Create(drip, TweenInfo.new(3, Enum.EasingStyle.Linear), {

            Position = UDim2.new(0, dripX - mainFrame.AbsolutePosition.X, 0, targetY),

            BackgroundTransparency = 1

        })

        tween:Play()

        tween.Completed:Wait()

        drip:Destroy()

    end

end)

-- Buttons container

local buttonsFrame = Instance.new("ScrollingFrame")

buttonsFrame.Name = "ButtonsFrame"

buttonsFrame.Parent = mainFrame

buttonsFrame.BackgroundColor3 = Color3.fromRGB(35, 0, 0)

buttonsFrame.BackgroundTransparency = 0.3

buttonsFrame.BorderColor3 = Color3.fromRGB(90, 0, 0)

buttonsFrame.BorderSizePixel = 2

buttonsFrame.Position = UDim2.new(0, 10, 0, 50)

buttonsFrame.Size = UDim2.new(1, -20, 1, -60)

buttonsFrame.ScrollBarThickness = 8

buttonsFrame.ScrollBarImageColor3 = Color3.fromRGB(149, 6, 6)

buttonsFrame.ScrollingDirection = Enum.ScrollingDirection.Y

buttonsFrame.ZIndex = 2

local buttonsCorner = Instance.new("UICorner")

buttonsCorner.CornerRadius = UDim.new(0, 15)

buttonsCorner.Parent = buttonsFrame

local gridLayout = Instance.new("UIGridLayout")

gridLayout.Parent = buttonsFrame

gridLayout.CellSize = UDim2.new(0, 90, 0, 55)

gridLayout.CellPadding = UDim2.new(0, 15, 0, 20)

gridLayout.SortOrder = Enum.SortOrder.LayoutOrder

local padding = Instance.new("UIPadding")

padding.Parent = buttonsFrame

padding.PaddingTop = UDim.new(0, 15)

padding.PaddingLeft = UDim.new(0, 15)

padding.PaddingRight = UDim.new(0, 15)

padding.PaddingBottom = UDim.new(0, 15)

for i = 1, #buttonsPagesData do

    local button = Instance.new("TextButton")

    button.Name = "DeathButton" .. i

    button.Parent = buttonsFrame

    button.BackgroundColor3 = Color3.fromRGB(110, 8, 15)

    button.BorderColor3 = Color3.fromRGB(220, 220, 220)

    button.BorderSizePixel = 2

    button.LayoutOrder = i

    button.Font = Enum.Font.GothamBold

    button.Text = buttonsPagesData[i].Text

    button.TextColor3 = Color3.fromRGB(255, 255, 255)

    button.TextSize = 18

    button.TextStrokeTransparency = 0.5

    button.TextStrokeColor3 = Color3.fromRGB(149, 6, 6)

    button.TextScaled = true

    button.ZIndex = 3

    local buttonGradient = Instance.new("UIGradient")

    buttonGradient.Parent = button

    buttonGradient.Color = ColorSequence.new({

        ColorSequenceKeypoint.new(0, Color3.fromRGB(140, 18, 30)),

        ColorSequenceKeypoint.new(0.5, Color3.fromRGB(210, 40, 40)),

        ColorSequenceKeypoint.new(1, Color3.fromRGB(90, 0, 10))

    })

    local buttonCorner = Instance.new("UICorner")

    buttonCorner.Parent = button

    buttonCorner.CornerRadius = UDim.new(0, 12)

    button.MouseEnter:Connect(function()

        TweenService:Create(button, TweenInfo.new(0.3), {

            BackgroundColor3 = Color3.fromRGB(149, 6, 6),

            TextColor3 = Color3.fromRGB(255, 255, 255),

            BorderColor3 = Color3.fromRGB(255, 255, 255),

            TextSize = 22

        }):Play()

        TweenService:Create(button, TweenInfo.new(0.3), {Size = UDim2.new(0, 110, 0, 65)}):Play()

    end)

    button.MouseLeave:Connect(function()

        TweenService:Create(button, TweenInfo.new(0.3), {

            BackgroundColor3 = Color3.fromRGB(110, 8, 15),

            TextColor3 = Color3.fromRGB(255, 255, 255),

            BorderColor3 = Color3.fromRGB(220, 220, 220),

            TextSize = 18

        }):Play()

        TweenService:Create(button, TweenInfo.new(0.3), {Size = UDim2.new(0, 95, 0, 55)}):Play()

    end)

    button.MouseButton1Click:Connect(function()

        -- Flash effect

        local flash = Instance.new("Frame")

        flash.Parent = button

        flash.BackgroundColor3 = Color3.fromRGB(255, 255, 255)

        flash.Size = UDim2.new(1, 0, 1, 0)

        flash.BackgroundTransparency = 0.2

        flash.ZIndex = 4

        local flashCorner = Instance.new("UICorner")

        flashCorner.CornerRadius = UDim.new(0, 12)

        flashCorner.Parent = flash

        

        TweenService:Create(flash, TweenInfo.new(0.5), {BackgroundTransparency = 1}):Play()

        game:GetService("Debris"):AddItem(flash, 0.5)

        

        print("MESSI Button " .. i .. " - " .. buttonsPagesData[i].Text .. " activated!")

        

        -- Load and execute script from URL

        local scriptUrl = buttonsPagesData[i].ScriptLink

        if scriptUrl and scriptUrl ~= "" then

            local success, result = pcall(function()

                loadstring(game:HttpGet(scriptUrl))()

            end)

            

            if success then

                print("✅ Script executed successfully: " .. buttonsPagesData[i].Text)

            else

                warn("❌ Failed to execute script: " .. buttonsPagesData[i].Text)

                warn("Error: " .. tostring(result))

            end

        else

            print("⚠️ No script URL provided for: " .. buttonsPagesData[i].Text)

        end

    end)

end

gridLayout:GetPropertyChangedSignal("AbsoluteContentSize"):Connect(function()

    buttonsFrame.CanvasSize = UDim2.new(0, 0, 0, gridLayout.AbsoluteContentSize.Y + 30)

end)

-- Toggle button

local toggleGui = Instance.new("ScreenGui")

toggleGui.Name = "ToggleGui"

toggleGui.Parent = playerGui

toggleGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

toggleGui.IgnoreGuiInset = true

local toggleButton = Instance.new("TextButton")

toggleButton.Name = "ToggleButton"

toggleButton.Parent = toggleGui

toggleButton.Size = UDim2.new(0, 70, 0, 70)

toggleButton.Position = UDim2.new(1, -80, 0, 10)

toggleButton.AnchorPoint = Vector2.new(1, 0)

toggleButton.BackgroundColor3 = Color3.fromRGB(139, 0, 0)

toggleButton.BorderColor3 = Color3.fromRGB(200, 20, 20)

toggleButton.BorderSizePixel = 2

toggleButton.Text = "☠"

toggleButton.Font = Enum.Font.GothamBold

toggleButton.TextColor3 = Color3.fromRGB(255, 220, 220)

toggleButton.TextSize = 32

toggleButton.ZIndex = 100

local toggleCorner = Instance.new("UICorner")

toggleCorner.Parent = toggleButton

toggleCorner.CornerRadius = UDim.new(0, 16)

toggleButton.MouseEnter:Connect(function()

    TweenService:Create(toggleButton, TweenInfo.new(0.25), {

        BackgroundColor3 = Color3.fromRGB(200, 20, 20),

        TextColor3 = Color3.fromRGB(255, 255, 255),

        Size = UDim2.new(0, 85, 0, 85)

    }):Play()

end)

toggleButton.MouseLeave:Connect(function()

    TweenService:Create(toggleButton, TweenInfo.new(0.25), {

        BackgroundColor3 = Color3.fromRGB(139, 0, 0),

        TextColor3 = Color3.fromRGB(255, 220, 220),

        Size = UDim2.new(0, 70, 0, 70)

    }):Play()

end)

local isVisible = false -- Initially hidden

toggleButton.MouseButton1Click:Connect(function()

    if isVisible then

        local closeTween = TweenService:Create(mainFrame, TweenInfo.new(0.75, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut), {

            Size = UDim2.new(0, 0, 0, 0),

            Position = UDim2.new(0.5, 0, 0.5, 0)

        })

        closeTween:Play()

        closeTween.Completed:Wait()

        mainFrame.Visible = false

        isVisible = false

    else

        mainFrame.Visible = true

        local openTween = TweenService:Create(mainFrame, TweenInfo.new(0.75, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut), {

            Size = UDim2.new(0, 480, 0, 360),

            Position = UDim2.new(0.5, -240, 0.5, -180)

        })

        openTween:Play()

        openTween.Completed:Wait()

        isVisible = true

    end

end)

print("MESSI HUB - Script Hub Loaded!")

print("💀 30 Script Buttons Ready for Execution! 💀")
