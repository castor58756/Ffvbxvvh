--// Hub Exploit para Blox Fruits - Feito para Natã //--

if not game:IsLoaded() then
    game.Loaded:Wait()
end

local Players = game:GetService("Players")
local LocalPlayer = Players.LocalPlayer

-- Criando UI Simples para o Hub
local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local Title = Instance.new("TextLabel")
local LoadScriptBtn = Instance.new("TextButton")

-- Configuração da GUI
ScreenGui.Parent = game.CoreGui

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
Frame.Position = UDim2.new(0.35, 0, 0.3, 0)
Frame.Size = UDim2.new(0, 250, 0, 150)
Frame.Active = true
Frame.Draggable = true

Title.Parent = Frame
Title.Text = "Hub de Exploit - Natã"
Title.Size = UDim2.new(1, 0, 0, 30)
Title.TextColor3 = Color3.fromRGB(255, 255, 255)
Title.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
Title.Font = Enum.Font.SourceSansBold
Title.TextSize = 18

LoadScriptBtn.Parent = Frame
LoadScriptBtn.Text = "Executar Script Blox Fruits"
LoadScriptBtn.Size = UDim2.new(1, 0, 0, 50)
LoadScriptBtn.Position = UDim2.new(0, 0, 0.3, 0)
LoadScriptBtn.BackgroundColor3 = Color3.fromRGB(0, 170, 255)
LoadScriptBtn.TextColor3 = Color3.fromRGB(255, 255, 255)
LoadScriptBtn.Font = Enum.Font.SourceSansBold
LoadScriptBtn.TextSize = 16

-- Função para executar o script remoto
LoadScriptBtn.MouseButton1Click:Connect(function()
    print("Carregando script para Natã...")
    loadstring(game:HttpGet("https://raw.githubusercontent.com/Rubix215/BloxFruitRubix/refs/heads/main/OPBloxFruits"))()
end)

print("Hub de Exploit carregado com sucesso, Natã!")
