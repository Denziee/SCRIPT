-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local MAIN = Instance.new("Frame")
local PROTEIN = Instance.new("TextButton")
local AUTOREBIRTH = Instance.new("TextButton")
local OPGUI = Instance.new("TextLabel")
local CLOSE = Instance.new("TextButton")
local OPENGUI = Instance.new("Frame")
local OPEN = Instance.new("TextButton")

--Properties:

ScreenGui.Parent = game.CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

MAIN.Name = "MAIN"
MAIN.Parent = ScreenGui
MAIN.BackgroundColor3 = Color3.fromRGB(0, 255, 255)
MAIN.Position = UDim2.new(0.44151777, 0, 0.233657822, 0)
MAIN.Size = UDim2.new(0, 222, 0, 266)
MAIN.Visible = false
MAIN.Active = true
MAIN.Draggable = true

PROTEIN.Name = "PROTEIN"
PROTEIN.Parent = MAIN
PROTEIN.BackgroundColor3 = Color3.fromRGB(0, 170, 0)
PROTEIN.Position = UDim2.new(0.224966794, 0, 0.313061267, 0)
PROTEIN.Size = UDim2.new(0, 122, 0, 67)
PROTEIN.Font = Enum.Font.SourceSans
PROTEIN.Text = "PROTEIN"
PROTEIN.TextColor3 = Color3.fromRGB(0, 0, 0)
PROTEIN.TextScaled = true
PROTEIN.TextSize = 14.000
PROTEIN.TextWrapped = true
PROTEIN.MouseButton1Down:Connect(function()
	loadstring(game:HttpGet("https://pastebin.com/raw/PWb3uj8g",true))()
end)

AUTOREBIRTH.Name = "AUTO REBIRTH"
AUTOREBIRTH.Parent = MAIN
AUTOREBIRTH.BackgroundColor3 = Color3.fromRGB(0, 170, 0)
AUTOREBIRTH.Position = UDim2.new(0.224966794, 0, 0.619545162, 0)
AUTOREBIRTH.Size = UDim2.new(0, 122, 0, 69)
AUTOREBIRTH.Font = Enum.Font.SourceSans
AUTOREBIRTH.Text = "AUTO REBIRTH"
AUTOREBIRTH.TextColor3 = Color3.fromRGB(0, 0, 0)
AUTOREBIRTH.TextScaled = true
AUTOREBIRTH.TextSize = 14.000
AUTOREBIRTH.TextWrapped = true
AUTOREBIRTH.MouseButton1Down:Connect(function()
	loadstring(game:HttpGet("https://pastebin.com/raw/MqY9xg4n",true))()
end)


OPGUI.Name = "OP GUI"
OPGUI.Parent = MAIN
OPGUI.BackgroundColor3 = Color3.fromRGB(0, 0, 127)
OPGUI.BackgroundTransparency = 0.500
OPGUI.Position = UDim2.new(0.211711705, 0, 0, 0)
OPGUI.Size = UDim2.new(0, 173, 0, 71)
OPGUI.Font = Enum.Font.SourceSans
OPGUI.Text = "OP GUI ULS"
OPGUI.TextColor3 = Color3.fromRGB(0, 0, 0)
OPGUI.TextScaled = true
OPGUI.TextSize = 14.000
OPGUI.TextWrapped = true

CLOSE.Name = "CLOSE"
CLOSE.Parent = MAIN
CLOSE.BackgroundColor3 = Color3.fromRGB(170, 0, 0)
CLOSE.Position = UDim2.new(0, 0, 4.19095159e-09, 0)
CLOSE.Size = UDim2.new(0, 47, 0, 73)
CLOSE.Font = Enum.Font.SourceSans
CLOSE.Text = "X"
CLOSE.TextColor3 = Color3.fromRGB(0, 0, 0)
CLOSE.TextScaled = true
CLOSE.TextSize = 14.000
CLOSE.TextWrapped = true
CLOSE.MouseButton1Down:Connect(function()
	MAIN.Visible = false
	OPENGUI.Visible = true
end)

OPENGUI.Name = "OPEN GUI"
OPENGUI.Parent = ScreenGui
OPENGUI.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
OPENGUI.Position = UDim2.new(0.114518151, 0, 0.272095084, 0)
OPENGUI.Size = UDim2.new(0, 100, 0, 55)
OPENGUI.Active = true
OPENGUI.Draggable = true

OPEN.Name = "OPEN"
OPEN.Parent = OPENGUI
OPEN.BackgroundColor3 = Color3.fromRGB(170, 0, 0)
OPEN.Position = UDim2.new(0.0499999523, 0, -0.00181829929, 0)
OPEN.Size = UDim2.new(0, 95, 0, 31)
OPEN.Font = Enum.Font.SourceSans
OPEN.Text = "OPEN"
OPEN.TextColor3 = Color3.fromRGB(0, 0, 0)
OPEN.TextScaled = true
OPEN.TextSize = 14.000
OPEN.TextWrapped = true
OPEN.MouseButton1Down:Connect(function()
	OPENGUI.Visible = false
	MAIN.Visible = true
end)
