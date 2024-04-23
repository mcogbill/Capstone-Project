# Capstone-Project

Hoplite Tactics Online is a two player real-time strategy game. Click 'Play Hoplite Challenge' to start a game against AI opponents, and compete with other players for a top position on the Leaderboard. Online PvP will be added at a later date. Future updates and development plans will be posted to the 'Dev Log' page.

## How the game works

- Players start game with three hoplite units to command.
- Hoplite units have individual Status Bars, Stances, Abilities, and Controls.
  - Status Bars
        - Health - Green represents remaining health. Red fills bar as unit receives damage. Unit dies when bar is 100% red.
        - Stamina (Endurance) - Blue represents remaining endurance stamina. Used for unit 'Movement', 'Fight', and 'Push' Abilities. Stamina recovers over time. Recovery rate depends on stance and current actions.
        - Stamina (Explosive) - Purple represents remaining explosive stamina. Used for 'Strike' attack. Stamina recovers over time. Recovery rate depends on stance and current actions.
  - Stances
        - Idle - Each unit will begin the game in this stance. Increased movement speed to change position quickly. Increased stamina recovery speed. Most vulnerable to all attacks.
        - Phalanx - Toggle into defensive stance against hoplite units. Reduced movemnt speed. Least vulnerable to hoplite attacks. Vulnerable to archer attacks. Requires Stamina (Endurance) >= 1% to remain active. If Stamina is below 1%, unit will return to Idle stance.
        - Turtle - Toggle into defensive stance against archer units. Reduced movment speed. Vulnerable to hoplite attacks. Least vulnerable to archer attacks.
  - Abilities
        - Strike - Quick attack. Deals most damage. Takes 50% Stamina (Endurance), and 100% Stamina (Explosive)
        - Fight - Toggle attack mode. Deals minimal damgage, and takes minimal Stamina (Endurance) while active. Requires Stamina (Endurance) >= 10% to remain active.
        - Push - Forcefully move enemy hoplite unit. Activated while in Phalanx stance, moving forward, and colliding with enemy hoplite unit.Takes maximum Stamina (Endurance) while active.

## Controls (Keyboard)

- Unit Selection - 'x'
- Movement:
       - Up - 'w'
       - Down - 's'
       - Left - 'a'
       - Right - 'd'
- Stance:
      - Idle - 'z'
      - Phalanx - 'r'
      - Turtle - 't'
- Attack:
      - Strike - 'f'
      - Fight - 'c' (Only in phalanx stance)

## Gameplay

- Victory Conditions:
	1. Domination
    	- Eliminate all enemy units.
	2. Capture the Flag
		- Each player has a capture point on the oposite side of the map.
    	- Whichever player occupies their capture point first will win the match.
    	- Occupy capture point after hoplite unit holds capture point position for 15 seconds.
    	- Strategy: Game mechanics allow for a variety of approaches to gameplay. Including: Defensive, Offensive, and Balanced strategies. Core gameplay is hoplite unit close combat. Players will need to manage health, stamina, and attack timing to succeed in combat. Archers are used to control the battle space. Players can control Archers targeting by capturing Archers position.

- Obstacles:
	- Map Boundaries: Units will not be able to move beyond the Top, bottom, left, and right borders of the map.
    - Terrain: Rock formations create choke points, and protection from flanking enemies.
    - Archers: Archers are positioned at the top of the map and are hostile to all units. Archer position may be captured by a single hoplite unit, providing freedom of movement for all friendly units. In Player vs. AI matches, Archers will only attack enemy AI if player is occupying Archer capture point. Hoplite units may enter a 'Turtle' stance to prevent damage from Archer attacks. However, 'Turtle' stance reduces hoplite movement speed and offensive abilities.

## User flow

![Capstone_Flow_Diagram](https://github.com/mcogbill/Capstone-Project/assets/9150602/1f25e882-a769-4453-9037-d018970d514e)

## Database

![Capstone_Database_Schema](https://github.com/mcogbill/Capstone-Project/assets/9150602/0d86bf78-604c-45d8-b421-6b5e3f07e91f)
