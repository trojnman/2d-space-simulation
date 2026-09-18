# 2D Space Simulation - latest session backup

Updated September 17, 2026, at the end of the development session. This replaces the earlier snapshot from today.

Download `2d-space-simulation-backup-2026-09-17.zip`, extract it, and import `2d-space-simulation/project.godot` in Godot 4.6.2. Press F5 (Run Project) in the editor. In the running game F5 is quicksave.

This is a source project backup, not a standalone Windows executable. A friend with repository access can download it and play through Godot. The repository is private; invite them as a collaborator before sharing its link. A standalone Windows release can be exported separately so players do not need Godot.

Latest work includes four active factions across ten sectors, faction economy and strategy priorities, 200-point faction ship supply limits, 60/120/300-second ship build times, empty starting station inventories, background simulation improvements, a continuous zoomable sector map, visible gates, seamless space background, and the expanding long-range scanner ping (L). Scan contacts include asteroids, last 60 seconds after the ring reaches them, and fade over 5 seconds.

Controls: WASD flight/map pan; M map; mouse wheel zoom; middle drag map pan; I inventory; Tab target; X clear target; E dock/jump; L scanner; P pause; Escape menu. This is a work-in-progress playtest.

Generated caches, logs, local savegames, and export binaries are excluded. The .sha256 file verifies the ZIP. Source, scenes, resources, documentation, and tests are included. Some older tests require fixture updates after the scenario changes; latest starting-region check passed 121 checks.
