# Capstone-Project

## How the game works

- Two player Real Time Strategy game
- Each player will start the game with three hoplite units to command
- Each hoplite unit has individual Status Bars, Stances, Abilities, and Controls
  - Status Bars
        1. Health - Green represents remaining health. Red fills bar as unit receives damage. Unit dies when bar is 100% red.
        2. Stamina (Endurance) - Blue represents remaining endurance stamina. Used for unit 'Movement', 'Fight', and 'Push' Abilities. Stamina recovers over time. Recovery rate depends on stance and current actions.
        3. Stamina (Explosive) - Purple represents remaining explosive stamina. Used for 'Strike' attack. Stamina recovers over time. Recovery rate depends on stance and current actions.
  - Stances
        1. Idle - Each unit will begin the game in this stance. Increased movement speed to change position quickly. Increased stamina recovery speed. Most vulnerable to all attacks.
        2. Phalanx - Toggle into defensive stance against hoplite units. Reduced movemnt speed. Least vulnerable to hoplite attacks. Vulnerable to archer attacks. Requires Stamina (Endurance) >= 1% to remain active. If Stamina is below 1%, unit will return to Idle stance.
        3. Turtle - Toggle into defensive stance against archer units. Reduced movment speed. Vulnerable to hoplite attacks. Least vulnerable to archer attacks.
  - Abilities
        1. Strike - Quick attack. Deals most damage. Takes 50% Stamina (Endurance), and 100% Stamina (Explosive)
        2. Fight - Toggle attack mode. Deals minimal damgage, and takes minimal Stamina (Endurance) while active. Requires Stamina (Endurance) >= 10% to remain active.
        3. Push - Forcefully move enemy hoplite unit. Activated while in Phalanx stance, moving forward, and colliding with enemy hoplite unit.Takes maximum Stamina (Endurance) while active.
  - Controls
        1. Select Unit - 'z' key to toggle selection between three hoplite units. Only selected unit is controlled.
        2. Movement - Arrow keys to move selected unit up, down, left, or right.
        3. Idle - 'z' key to activate stance. All units begin game in Idle stance.
        4. Phalanx - 'g' key to activate stance.
        5. Turtle - 't' key to activate stance.
        3. Strike - 'r' key (quick attack) from any stance.
        4. Fight - 'f' key to activate from Phalanx stance only.
        5. Push - Arrow keys while Phalanx stance is active, and colliding with enemy hoplite unit.
- Victory Conditions
    1. Capture enemy flag
        - Whichever player occupies their capture point first will win the match.
        - Both players will have capture points on the oposite side of the map.
        - A hoplite unit occupies thier capture point by remaining on the capture point position for 15 seconds.
    2. Eliminate all enemy units
        - Whichever player reduces all enemy unit health bars to 0% will win the match.
- Obstacles
    1. Map edges: Player's units will not be able to move beyond the Top, bottom, left, and right borders of the map.
    2. Rocks: Two rock formations in the middle of the map to create choke points and protection from Archer attacks.
    3. Archers: Archers are positioned at top of map preventing freedom of movement for hoplite units looking to rush accross the map to capture points. Strategy is required to out maneuver archers while maintinaing hoplite offense and defense against oppoising player. Archer position may be captured by a single hoplite unit, providing freedom of movemnt for other units. Archer attack range is limited to top half of the map, allowing for hoplite units to move through narrow paths created by rock formations at the bottom of the map.

## User flow

1. Install app
2. Open app in browser to homepage
3. From homepage, select local play, online play, or ranking
4. If select local play
    - Two players use same keyboard
    - Return to homepage following player victory
5. If select online play
    - Player will select username
    - Player matchmaking
    - Match start when matchmaking complete
    - When match is complete, rankings will update with match results
    - Player can select rematch, view rankings, or return to homepage
6. If select rankings
    - Player views match stats associated with username

## Database (User Rankings)

Columns (data scheme) relational database diagram. Game status, team1 and 2, score. Create search date/time and team name (ex. redFlag1). **SQL alchemy or Express. Add a table.

### Columns

1. Player ID
2. Player Username
3. Player team (1 or 2)
4. Match date time group
5. Match results (victory for team 1 or 2)
6. Match details (victory condition, unit stats, match duration, etc.)

-database sql schema
-user flow diagram: https://app.diagrams.net/