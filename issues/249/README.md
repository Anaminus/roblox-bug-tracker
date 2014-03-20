# Model Bug

1. Open ModelBug.rbxl
2. Observe the positions of the parts in Workspace.ModelA. They should be exactly 1.5 studs apart.
3. Move ModelA to ServerStorage. Note that positions of each part remain intact.
4. Move ModelA to ServerStorage.ModelB. The positions of each part should have been modified.
5. Note that even the relative positions of both parts have changed (no longer 1.5 studs apart).
