-- LocalScript (para enviar comandos do jogador)

local ReplicatedStorage = game:GetService("ReplicatedStorage")
local autoFarmEvent = ReplicatedStorage:WaitForChild("OnServerEvent")

local function ativarAutoFarm()
    autoFarmEvent:FireServer("ativar")
end

local function desativarAutoFarm()
    autoFarmEvent:FireServer("desativar")
end

-- Aqui você pode configurar botões ou outros métodos para ativar/desativar
-- Exemplo: quando o jogador clica em um botão, chama essas funções
