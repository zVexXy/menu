local player = game.Players.LocalPlayer
local gui = Instance.new("ScreenGui")
gui.Parent = player:WaitForChild("PlayerGui")

local frame = Instance.new("Frame")
frame.Size = UDim2.new(0, 200, 0, 80)
frame.AnchorPoint = Vector2.new(0.5, 0.5)
frame.Position = UDim2.new(0.5, 0, 0.5, 0)
frame.BackgroundColor3 = Color3.fromRGB(50,50,50)
frame.BorderSizePixel = 2
frame.BackgroundTransparency = 0
frame.Active = true
frame.Draggable = true
frame.Parent = gui

local btn1 = Instance.new("TextButton")
btn1.Size = UDim2.new(0.5, -6, 1, -12)
btn1.Position = UDim2.new(0, 6, 0, 6)
btn1.Text = "Sobrevivente"
btn1.TextScaled = true
btn1.BackgroundColor3 = Color3.fromRGB(40,180,40)
btn1.Parent = frame

local btn2 = Instance.new("TextButton")
btn2.Size = UDim2.new(0.5, -6, 1, -12)
btn2.Position = UDim2.new(0.5, 6, 0, 6)
btn2.Text = "Caçador"
btn2.TextScaled = true
btn2.BackgroundColor3 = Color3.fromRGB(180,40,40)
btn2.Parent = frame

btn1.MouseButton1Click:Connect(function()
    print("Sobrevivente ativado!")
end)
btn2.MouseButton1Click:Connect(function()
    print("Caçador ativado!")
end)
