# Steps

1. With Roblox Studio, open [`Move() bug repro.rbxl`](Move() bug repro.rbxl).
2. Create a test server with 1 player.
3. After your player has loaded, walk your character towards the "Bob" character.
4. Observe that, once Bob is within your client's SimulationRadius, Bob stops walking.
5. Also observe that Bob will resume walking if he is outside of your client's SimulationRadius.
