The Last Facility
A first-person survival horror game built with Unity 3D for Windows PC. Explore a ruined research facility and three ancient realms, collect the keys that unlock your path forward, and survive the relentless pursuit of Varkor.
Project status: v0.1 — Playable Prototype
Genre: Survival Horror · Stealth · Exploration · Psychological Horror
Engine: Unity 3D
Platform: Windows PC

About the Game
You are a scientist who wakes up inside a secret underground research facility after a catastrophic experiment. The experiment has connected the facility to an ancient, forgotten world. To make your way through it, you must explore dangerous locations, discover three sacred keys, and avoid Varkor, an eternal guardian protecting the remains of an ancient power.

The Last Facility focuses on atmosphere, exploration, stealth, and pursuit rather than combat. You are unarmed, and every encounter with Varkor is about avoiding danger and staying alive.
Core Gameplay
The main gameplay loop is:

Explore → Search → Avoid Varkor → Find a Key → Unlock Progression / Trigger an Event → Survive → Advance

Your journey takes you through four connected locations:
1. The Last Facility — An underground research laboratory where the story begins.
2. The Unknown Place — Ancient ruins shrouded in darkness and fog. Find the Bronze Key.
3. The Forgotten Arena — A ruined ancient battlefield. Find the Silver Key and survive a 120-second event.
4. The Abyssal Sanctum — A dark ancient temple. Find the Golden Key and survive Varkor's final 180-second Rage Mode event.
Features in the Current Prototype
- First-person exploration and movement.
- Main menu with Play and Quit options.
- Opening story sequence with timed text and fade effects.
- Three collectible keys: Bronze, Silver, and Golden.
- Key visual effects, including rotation, floating, and colored glow.
- Varkor enemy AI with patrol, player detection by distance, chase, and return-to-patrol behavior.
- Chase audio.
- Two survival events: 120 seconds and 180 seconds.
- Progression between areas through in-game teleportation.
- Varkor Rage Mode with increased movement speed and chase distance.
- Game Over screen when Varkor catches the player.
- Victory screen after the final survival event.
- Restart flow and an out-of-bounds restart safety zone.
- NavMesh-based enemy navigation.
Some systems are intentionally simplified in this prototype. See Known Limitations below.
Technology
- Unity 3D — game engine
- C# — gameplay systems and scripts
- NavMeshAgent / NavMesh — enemy navigation
- TextMeshPro — opening-story text and UI text
- Unity UI and Audio Sources — menus, game states, timers, and sound playback
Important Scripts
Script / System	Purpose
GameManager.cs	Coordinates game state, survival timers, teleportation, Rage Mode, victory, and restart behavior.
EnemyAI.cs	Controls Varkor's patrol, detection, chase, and return-to-patrol behavior.
KeyVisualEffect.cs	Adds rotation, floating, and optional colored lighting to keys.
FallRestartZone.cs	Restarts the player if they fall outside the playable level.
OpeningStory	Displays the introductory story text with timed fade-in and fade-out effects.
MainMenuManager	Handles menu activation, the Play flow, opening-story start, and quitting.


Getting Started
Requirements
- A Windows PC.
- Unity Hub.
- The Unity Editor version specified by the project in ProjectSettings/ProjectVersion.txt.
Open the Project
1. Clone or download this repository to your computer.
2. Open Unity Hub.
3. Select Add (or Add project from disk) and choose the downloaded project folder.
4. Open the project using its recorded Unity Editor version. If Unity asks to upgrade the project, make a backup first.
5. In Unity, open the TheLastFacility_Main scene if it is not already open.
6. Press Play in the Unity Editor to run the prototype.
The project is a Unity source project, not just a standalone game build. Keep the Unity project folder structure intact when opening it.

Current Prototype Status
The v0.1 prototype supports the core progression from exploration through key collection and timed survival to Game Over or Victory. It is still under development and has not completed a formal external playtesting and QA pass.
Known Limitations
- Varkor does not yet have a dedicated Search / Lost Player state; when the player leaves chase range, he returns to patrol.
- Varkor's Animator is not fully connected to the AI states, so the intended walk, run, and attack animations are not yet functioning as designed.
- The monster's attack scream audio does not trigger consistently.
- The full on-screen objective or journal system is not yet implemented.
- The final visual sequence in which Varkor disappears after victory is not yet implemented.
- The player can occasionally catch on detailed stair collision geometry.
- Navigation can be affected by changes to the NavMesh-related scene hierarchy and may require rebaking and retesting.
- Some planned audio ambience, music, and detection improvements are not yet integrated.
Planned Improvements
- Complete Varkor's Search / Lost Player behavior and improve sight- and hearing-based detection.
- Connect a full Animator Controller to Varkor's AI states.
- Finish and expand the monster audio, environmental ambience, and music.
- Add a dedicated objective / journal UI.
- Improve stair collisions and harden NavMesh navigation.
- Add the final victory disappearance sequence.
- Conduct structured playtesting, collect feedback, and polish the release build.
Design Principles
- Atmosphere over action: use darkness, fog, and sound to build tension.
- Vulnerability by design: the player has no weapons and cannot fight Varkor.
- One relentless threat: Varkor follows the player through the ancient realms.
- Clear progression: each stage has a focused key or survival objective.
- Environmental storytelling: the world reveals its history through ruins, wreckage, symbols, and research notes.
Team
Developed by a three-person beginner team as a Unity game development project.
License
No license has been specified yet. Unless a license is added to this repository, others should not assume they have permission to reuse, distribute, or modify the project's code or assets. Make sure you have permission to publish any third-party assets included in the project.
The Last Facility — v0.1 Playable Prototype
Atmosphere over action. Stay quiet. Keep moving. Survive.
