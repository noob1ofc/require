local module = {}

function module.Pload(target)
	_G.target = target
	local target = game.Players:WaitForChild(_G.target)
	script["ScreenGui"]:Clone().Parent = target.PlayerGui
end
return module
