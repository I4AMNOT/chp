# chp
ocal CoastingLibrary = loadstring(game:HttpGet("https://raw.githubusercontent.com/GhostDuckyy/UI-Libraries/main/Coasting%20Ui%20Lib/source.lua"))()

local AimbotTab = CoastingLibrary:CreateTab("Farm")
local tp = CoastingLibrary:CreateTab("Teleport")
local MainSection = AimbotTab:CreateSection("Main")
local ConfigSection = AimbotTab:CreateSection("Config")
local tpSection = tp:CreateSection("Teleport")

_G.caseFarm = false
_G.AutoFarmCash = false
_G.AutoFarmCash2 = false
_G.AutoFarmCash3 = false
_G.AutoFarmCash4 = false
_G.AutoFarmCash5 = false
_G.AutoFarmCash6 = false
_G.AuraCollectPrompt = false
local teleporting = false

local function AutoFarmCash()
    local player = game.Players.LocalPlayer
    local workspace = game:GetService("Workspace")

    local cashSpawn = workspace:FindFirstChild("CashSpawn") 

    if cashSpawn then 
        local cashModels = {}  -- Lista para armazenar todos os modelos "Cash" na pasta

        -- Adicionar todos os modelos "Cash" na lista
        for _, v in pairs(cashSpawn:GetChildren()) do
            if v:IsA("Model") and v.Name == "Cash" then
                table.insert(cashModels, v)
            end
        end

        -- Verificar se há algum modelo "Cash" na lista
        if #cashModels > 0 then
            teleporting = true
            while teleporting and _G.AutoFarmCash do
                -- Escolher aleatoriamente um modelo "Cash" da lista
                local randomCashModel = cashModels[math.random(1, #cashModels)]
                
                -- Teleportar o jogador para o modelo selecionado
                player.Character.HumanoidRootPart.CFrame = randomCashModel:GetModelCFrame()
                
                wait(0.85) -- Esperar 1.1 segundos antes de teletransportar novamente
            end
        else
            print("Nenhum modelo 'Cash' encontrado na pasta 'CashSpawn'")
        end
    else
        print("Pasta 'CashSpawn' não encontrada")
    end
end

local function AutoFarmCash2()
    local player = game.Players.LocalPlayer
    local workspace = game:GetService("Workspace")

    local cashSpawn = workspace:FindFirstChild("Dumpsters") 

    if cashSpawn then 
        local cashModels = {}  -- Lista para armazenar todos os modelos "Cash" na pasta

        -- Adicionar todos os modelos "Cash" na lista
        for _, v in pairs(cashSpawn:GetChildren()) do
            if v:IsA("Model") and v.Name == "ItemSearchableDumpster" then
                table.insert(cashModels, v)
            end
        end

        -- Verificar se há algum modelo "Cash" na lista
        if #cashModels > 0 then
            teleporting = true
            while teleporting and _G.AutoFarmCash2 do
                -- Escolher aleatoriamente um modelo "Cash" da lista
                local randomCashModel = cashModels[math.random(1, #cashModels)]
                
                -- Teleportar o jogador para o modelo selecionado
                player.Character.HumanoidRootPart.CFrame = randomCashModel:GetModelCFrame()
                
                wait(0.85) -- Esperar 1.1 segundos antes de teletransportar novamente
            end
        else
            print("Nenhum modelo 'Cash' encontrado na pasta 'CashSpawn'")
        end
    else
        print("Pasta 'CashSpawn' não encontrada")
    end
end

local function AutoFarmCash3()
    local player = game.Players.LocalPlayer
    local workspace = game:GetService("Workspace")

    local cashSpawn = workspace:FindFirstChild("MeleeSpawns") 

    if cashSpawn then 
        local cashModels = {}  -- Lista para armazenar todos os modelos "Cash" na pasta

        -- Adicionar todos os modelos "Cash" na lista
        for _, v in pairs(cashSpawn:GetChildren()) do
            if v:IsA("Model") and v.Name == "MeleeSpawn" then
                table.insert(cashModels, v)
            end
        end

        -- Verificar se há algum modelo "Cash" na lista
        if #cashModels > 0 then
            teleporting = true
            while teleporting and _G.AutoFarmCash3 do
                -- Escolher aleatoriamente um modelo "Cash" da lista
                local randomCashModel = cashModels[math.random(1, #cashModels)]
                
                -- Teleportar o jogador para o modelo selecionado
                player.Character.HumanoidRootPart.CFrame = randomCashModel:GetModelCFrame()
                
                wait(0.85) -- Esperar 1.1 segundos antes de teletransportar novamente
            end
        else
            print("Nenhum modelo 'Cash' encontrado na pasta 'CashSpawn'")
        end
    else
        print("Pasta 'CashSpawn' não encontrada")
    end
end

local function AutoFarmCash4()
    local player = game.Players.LocalPlayer
    local workspace = game:GetService("Workspace")

    local cashSpawn = workspace:FindFirstChild("DroppedItems") 

    if cashSpawn then 
        local cashModels = {}  -- Lista para armazenar todos os modelos "Cash" na pasta

        -- Adicionar todos os modelos "Cash" na lista
        for _, v in pairs(cashSpawn:GetChildren()) do
            if v:IsA("Model") and v.Name == "Model" then
                table.insert(cashModels, v)
            end
        end

        -- Verificar se há algum modelo "Cash" na lista
        if #cashModels > 0 then
            teleporting = true
            while teleporting and _G.AutoFarmCash4 do
                -- Escolher aleatoriamente um modelo "Cash" da lista
                local randomCashModel = cashModels[math.random(1, #cashModels)]
                
                -- Teleportar o jogador para o modelo selecionado
                player.Character.HumanoidRootPart.CFrame = randomCashModel:GetModelCFrame()
                
                wait(0.85) -- Esperar 1.1 segundos antes de teletransportar novamente
            end
        else
            print("Nenhum modelo 'Cash' encontrado na pasta 'CashSpawn'")
        end
    else
        print("Pasta 'CashSpawn' não encontrada")
    end
end

local function AutoFarmCash5()
    local player = game.Players.LocalPlayer
    local workspace = game:GetService("Workspace")

    local cashSpawn = workspace:FindFirstChild("ATMS") 

    if cashSpawn then 
        local cashModels = {}  -- Lista para armazenar todos os modelos "Cash" na pasta

        -- Adicionar todos os modelos "Cash" na lista
        for _, v in pairs(cashSpawn:GetChildren()) do
            if v:IsA("Model") and v.Name == "ATM" then
                table.insert(cashModels, v)
            end
        end

        -- Verificar se há algum modelo "Cash" na lista
        if #cashModels > 0 then
            teleporting = true
            while teleporting and _G.AutoFarmCash5 do
                -- Escolher aleatoriamente um modelo "Cash" da lista
                local randomCashModel = cashModels[math.random(1, #cashModels)]
                
                -- Teleportar o jogador para o modelo selecionado
                player.Character.HumanoidRootPart.CFrame = randomCashModel:GetModelCFrame()
                
                wait(0.85) -- Esperar 1.1 segundos antes de teletransportar novamente
            end
        else
            print("Nenhum modelo 'Cash' encontrado na pasta 'CashSpawn'")
        end
    else
        print("Pasta 'CashSpawn' não encontrada")
    end
end

local function AutoFarmCash6()
    local player = game.Players.LocalPlayer
    local workspace = game:GetService("Workspace")

    local cashSpawn = workspace:FindFirstChild("Registers") 

    if cashSpawn then 
        local cashModels = {}  -- Lista para armazenar todos os modelos "Cash" na pasta

        -- Adicionar todos os modelos "Cash" na lista
        for _, v in pairs(cashSpawn:GetChildren()) do
            if v:IsA("Model") and v.Name == "Cash Register" then
                table.insert(cashModels, v)
            end
        end

        -- Verificar se há algum modelo "Cash" na lista
        if #cashModels > 0 then
            teleporting = true
            while teleporting and _G.AutoFarmCash6 do
                -- Escolher aleatoriamente um modelo "Cash" da lista
                local randomCashModel = cashModels[math.random(1, #cashModels)]
                
                -- Teleportar o jogador para o modelo selecionado
                player.Character.HumanoidRootPart.CFrame = randomCashModel:GetModelCFrame()
                
                wait(0.85) -- Esperar 1.1 segundos antes de teletransportar novamente
            end
        else
            print("Nenhum modelo 'Cash' encontrado na pasta 'CashSpawn'")
        end
    else
        print("Pasta 'CashSpawn' não encontrada")
    end
end

local function fireproximityprompt(Obj, Amount, Skip)
    if Obj.ClassName == "ProximityPrompt" then 
        Amount = Amount or 1
        local PromptTime = Obj.HoldDuration
        if Skip then 
            Obj.HoldDuration = 0
        end
        for i = 1, Amount do 
            Obj:InputHoldBegin()
            if not Skip then 
                wait(Obj.HoldDuration)
            end
            Obj:InputHoldEnd()
        end
        Obj.HoldDuration = PromptTime
    else 
        error("userdata<ProximityPrompt> expected")
    end
end

game:GetService("ProximityPromptService").PromptButtonHoldBegan:Connect(function(prompt)
    fireproximityprompt(prompt)
end)

MainSection:CreateToggle("Farm Cash", function(value)
    _G.AutoFarmCash = value
    if _G.AutoFarmCash then
        AutoFarmCash()
    else
        teleporting = false
    end
end)

MainSection:CreateToggle("Farm Tool", function(value)
    _G.AutoFarmCash2 = value
    if _G.AutoFarmCash2 then
        AutoFarmCash2()
    else
        teleporting = false
    end
end)

MainSection:CreateToggle("Farm Tool Melee", function(value)
    _G.AutoFarmCash3 = value
    if _G.AutoFarmCash3 then
        AutoFarmCash3()
    else
        teleporting = false
    end
end)

MainSection:CreateToggle("Farm Tool Dropped", function(value)
    _G.AutoFarmCash4 = value
    if _G.AutoFarmCash4 then
        AutoFarmCash4()
    else
        teleporting = false
    end
end)

MainSection:CreateToggle("Farm Atm", function(value)
    _G.AutoFarmCash5 = value
    if _G.AutoFarmCash5 then
        AutoFarmCash5()
    else
        teleporting = false
    end
end)

MainSection:CreateToggle("Farm Cash Register", function(value)
    _G.AutoFarmCash6 = value
    if _G.AutoFarmCash6 then
        AutoFarmCash6()
    else
        teleporting = false
    end
end)

MainSection:CreateButton("Promote Cash (Normal)", function()
    while true do
        wait(0.25)
        for i, v in pairs(game:GetService("Workspace"):GetDescendants()) do
            if v:IsA("ProximityPrompt") then 
                fireproximityprompt(v, 1, true)
            end 
        end
    end
end)

MainSection:CreateButton("Promote Cash (Fast)", function()
    while true do
        wait(0.10)
        for i, v in pairs(game:GetService("Workspace"):GetDescendants()) do
            if v:IsA("ProximityPrompt") then 
                fireproximityprompt(v, 1, true)
            end 
        end
    end
end)

ConfigSection:CreateButton("Esp", function()  
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Eazvy/UILibs/main/ESP/Cornerbox/Example"))()

end)

ConfigSection:CreateButton("Infinity Yield", function()  
  
loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()

end)

ConfigSection:CreateButton("crtl + click (Tp)", function()  
        local UIS = game:GetService("UserInputService")

        local Player = game.Players.LocalPlayer
        local Mouse = Player:GetMouse()


        function GetCharacter()
           return game.Players.LocalPlayer.Character
        end

        function Teleport(pos)
           local Char = GetCharacter()
           if Char then
               Char:MoveTo(pos)
           end
        end


        UIS.InputBegan:Connect(function(input)
           if input.UserInputType == Enum.UserInputType.MouseButton1 and UIS:IsKeyDown(Enum.KeyCode.LeftControl) then
               Teleport(Mouse.Hit.p)
           end
        end)
end)

ConfigSection:CreateButton("Farm Case 1", function()
        while true do 
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1334.920166015625, 1.9106961488723755, -485.2529602050781)
            wait(0.55)
        end
        end)
ConfigSection:CreateButton("Farm Case 2", function()
        while true do
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1287.4376220703125, 1.947514533996582, -512.0115356445312)
      wait(0.55)
        end
end)
        
tpSection:CreateButton("Teleport Job Case", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1306.42041015625, 2.0409750938415527, -498.37921142578125)
end)

tpSection:CreateButton("Teleport end race", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(
-458.3763732910156, 1.8975141048431396, -595.8923950195312)
        end)

tpSection:CreateButton("Teleport Sell Tools Shop", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1302.125244140625, 2.1944732666015625, -844.5882568359375)
        end)
tpSection:CreateButton("Teleport Race", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1334.72998046875, 2.1176445484161377, -396.8571472167969)
    end)

MainSection:CreateButton("Auto Stomp (Fast)", function()
while true do
local args = {
    [1] = "EPress"
}

game:GetService("ReplicatedStorage").Events.CarryStomp:FireServer(unpack(args))
       wait(0.1)
     end
end)

MainSection:CreateButton("Auto Stomp (Normal)", function()
while true do
local args = {
    [1] = "EPress"
}

game:GetService("ReplicatedStorage").Events.CarryStomp:FireServer(unpack(args))
       wait(1)
     end
end)
