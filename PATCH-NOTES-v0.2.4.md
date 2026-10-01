# Himinn v0.2.4 — Fleet, stations and equipment

## Factions and visual direction
- Renamed the human faction to the Tiresias Empire, the traders to the Loreai Free Traders Guild, and the corsairs to the Eleutheros Freemen; expanded faction lore, including the Ash Collective.
- Added detailed Tiresias artwork for small, medium and heavy fighters, haulers and miners, medium and large logistics ships, the escape capsule and emergency mining drone.
- Built mining emitters into the mining hulls; the emergency mining drone has no defense turret.
- Integrated turret bearings, straight forward gun housings and appropriately sized missile cradles into the approved hull designs. Corrected weapon scale across ship sizes and relocated the medium logistics launchers.
- Added the approved Loreai heavy-fighter design, integrated ruby weapon mounts and five thrust-responsive ruby engines. This artwork is retained for later faction-specific development.
- All factions temporarily use Tiresias ship, station and equipment visuals. Ownership, diplomacy, faction names and saved construction identity remain separate. Missile boats still use the earlier Tiresias hull artwork pending their detailed art pass.
- Ship names use faction prefixes, such as Tir Medium Fighter.

## Weapons and missiles
- Added detailed S1, S2 and S3 ballistic and laser equipment: single-barrel cannons, twin alternating autocannons and single-cluster rotary miniguns, with separate fixed and turret fittings.
- Added efficient recoil and firing effects using shared artwork and existing pooled effects.
- Completed S1/S2 missile racks based on the approved S3 rack. Smaller rack sizes have smaller physical housings.
- Downsized missiles share one rack housing: an S3 mount carries one S3, two S2 or four S1 missiles; an S2 mount carries one S2 or two S1 missiles.
- Individual visible rounds follow loaded ammunition. Launched missiles use the same artwork, scale and physical launch channels as their rack contents.
- Missiles can turn toward an off-axis target during their initial acquisition window, up to two seconds. Normal seeker-cone limits apply once acquired or the window expires, allowing missiles to be dodged.

## Stations and defenses
- Completed detailed station artwork for Imperial Command, trade exchanges, refineries, fabrication complexes, standard and capital shipyards, military bastions, defense platforms, claim beacons and both makeshift facilities.
- Integrated station weapons into authored mounts, corrected rack alignment and scaled equipment consistently with large ships. Simplified structural collision preserves major bays and openings.
- Bastions support defense platforms with small/medium-ship defenses and use the corresponding platform building rules.
- Trade exchanges carry four S1 and four S3 turrets; fabrication stations carry four S1 turrets; refineries carry three S2 turrets.
- Station shields now follow the hull envelope and use ship-style energy visuals and impact feedback. Charged shields regenerate under fire; collapse starts the reboot delay, and subsequent hull hits do not restart it.

## Interface and fixes
- Applied the purple celestial main-menu direction throughout the UI, with static lightning-green Himinn-style lettering and thicker strokes for readability.
- Shipyard, purchase, hangar and refitting previews show actual hull and mounted-equipment artwork. Fixed missing armor layers in missile-boat previews.
- Station mission boards now show the same faction-wide mission pool as faction AI chat. Issuing stations remain identified, and mission destinations and completion requirements are unchanged.
- Removed obsolete Tiresias assets and moved earlier Loreai proposals out of the game asset folder while preserving approved designs.

## Additional v0.2.4 fixes
- Fixed the docked Missions tab's collapsed scrolling area and refresh on tab selection. Verified the faction-wide mission list at every station belonging to each faction.
- Shipyards now buy back products they manufacture, including sensor satellites. Blocked sales show their reason directly in the trade row.
- Selling now uses ship cargo first, then personal storage at the docked station. The trade list shows both counts and keeps owned items visible even when the station does not buy them, with a reason on the disabled Sell button. Other stations' storage is excluded.
- Trade buttons now read You Buy and You Sell; price columns read You Pay and You Receive.
- Leaving map mode explicitly restores the current ship's camera, including after a stale camera reference. Movement follows interpolated ship positions, zoom smooths each frame, and map scrolling no longer changes the hidden flight camera's zoom.
- The piloted ship now appears in Fleet Manager. Lead selected fleet joins that fleet as its player leader and orders its ships to follow you.
- Player hyperspace jumps include only members of the player's named fleet in the current sector. Unassigned owned ships stay behind; an unassigned player jumps alone.
- Reduced small missile boat acceleration by 25% in all movement directions, with maximum speed unchanged.

## Validation and known limits
- Checked ship/station art, mount counts, shield behavior, equipment, refitting, saves, general gameplay, UI and faction mission visibility.
- Local rendered benchmarks at 1600×900 on an RTX 5070: about 302 FPS fresh start, 284 FPS normal fleet flight, 180 FPS sector map and 173 FPS patrol-area dragging. These are local measurements, not hardware guarantees.
- The fleet-cap concentrated battle stress test averaged about 10.6 FPS and slowed simulation to roughly half speed. Large-battle optimization remains pending. Fresh-start sector initialization can also cause brief frame-time spikes.
- A full ten-hour progression soak has not been completed for this patch.

## Installation
Download Himinn-Setup-v0.2.4.exe and run it. Windows x64; local AI setup follows the existing installer flow. Saves are preserved, but compatibility with every older save state has not been exhaustively tested. This is an unsigned development playtest.
