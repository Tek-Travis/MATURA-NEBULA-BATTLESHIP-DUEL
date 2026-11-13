MUTARA NEBULA DUEL — MULTI-MAP UPDATE

INSTALL
Back up your current Mutara_Duel.html. Replace it with the included HTML in your existing game folder. Keep all PNGs and MP3s beside it, unchanged. Open the HTML and click New Battle. No installation or server required. ai-worker.js is not used.

LAYOUT
Title and compact sound/AI/map toolbar on top. No visible round counter. Bottom controls: arrows, weapons, FIRE. Status panels keep their established content sizing; the battlefield square matches their height when horizontal space permits. Smaller screens use an adaptive, width-limited layout.

MAPS
25x25, 50x50 and 100x100. Settings apply on New Battle. Ships always occupy 5x5 squares, move one square per round and have a one-square visibility border. Larger maps show smaller ships and grid squares in the same window. No magnifier.
Random spawns have at least ten empty squares separating footprint edges along at least one map axis. Initial directions allow in-bounds moves.
Battlefield ships rotate with movement; status images stay bow-up. Hit locations are transformed back to the correct bow-up status square.
Both ships move each round, stay in bounds and avoid intersecting paths. Conflicts trigger alternate legal movement, preserving your direction when possible.

COMBAT
Torpedo 15 hull percentage points; phasers 5. No splash or shields/engineering bonuses. Both ships move before simultaneous fire. Damage markers are visual impact indicators, not movement restrictions. Red until the next committed round, then green for two seconds. Hull never repairs. Enemy damage telemetry is always visible in Sensors.
Fog is 38 percent opaque; hidden enemy artwork is not drawn outside detection. Bridge loops; all other sounds play once per event. Critical warning once at 25 percent or lower. Offline sound is an incoming impact effect, not a shutdown.
Click to target. Focus the canvas and use arrow keys for keyboard targeting. Coordinates extend beyond Z (AA ... CV). Historical marks are not current contacts.

REQUIRED ASSETS (beside HTML)
USS ENTERPRISE.png
USS RELIANT.png
Mutara Nebula 1.png
BRIDGE.mp3
CLICK.mp3
CRITICAL HULL HEALTH.mp3
DEATH.mp3
HIT.mp3
PHASER.mp3
SYSTEM OFFLINE.mp3
TORPEDO.mp3

VERIFICATION
JavaScript syntax, randomized spawns and movement on all three map sizes, AI corner movement on all difficulties, rotated damage mapping and extended coordinates checked with Node.js. Canvas avoids thousands of DOM cells; Hard AI uses a difference-array map accumulation.
No browser playtest here: check local layout, image alignment and audio with your assets.


Star Trek and all related properties are trademarks and copyrights of Paramount Skydance Corporation and CBS Studios Inc. All Rights Reserved. Unofficial, non-commercial fan project.
