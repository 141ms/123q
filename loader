local repo = 
local function LoadScript(ScriptName)
	pcall(function()
		t = 0
		repeat
			local s, r = pcall(function()
				loadstring(game:HttpGet(repo .. ScriptName))()
			end)
			if not s then
				spawn(function()
					error(r)
				end)
			end
			t = t + 1
			wait(60)
		until getgenv().Executed or t >= 30
	end)
end
local Id = game.PlaceId
local PlaceIds = {
	["AA"] = { 8304191830 },
	["AA2"] = { 8349889591 }
}
if table.find(PlaceIds["AA"], Id) then -- Anime Adventures
	LoadScript("Anime%20Adventures.lua")
elseif table.find(PlaceIds["AA2"], Id) then -- Blox Fruits
	LoadScript("BloxFruits.lua")
	end
end
