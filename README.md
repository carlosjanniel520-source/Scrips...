game.Players.PlayerAdded:Connect(function(p)
	local ls = Instance.new("Folder", p)
	ls.Name = "leaderstats"

	for _,n in ipairs({"Kills","Deaths","Cash"}) do
		local v = Instance.new("IntValue", ls)
		v.Name = n
	end
end)
