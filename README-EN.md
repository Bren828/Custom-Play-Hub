# Custom-Play-Hub

_A system for creating custom game lobbies with a built-in map editor.
Players can create their own maps for the following modes: **Race, Deathmatch, Team Deathmatch, Counter-Strike, Duel, and Derby.**_

### Reference
* [Modes](https://github.com/Bren828/Custom-Play-Hub#Modes)
* [Editor](https://github.com/Bren828/Custom-Play-Hub#Editor)
* [Options](https://github.com/Bren828/Custom-Play-Hub#Options)
* [Information](https://github.com/Bren828/Custom-Play-Hub#Price)


# Main menu

_Interaction with game lobbies is carried out through the main menu.
The menu is implemented using TextDraw and consists of four pages: **Lobbies, Playlists, Create, and Editor.**_


## Lobbies
All lobbies created by players are displayed here.

## Playlists
This section displays playlists created by players.
Players can create their own playlists, add various projects to them, set a name and description, and make the playlist private.

## Create
In this section, players can create their own lobbies using ready-made projects published by other players.
Project search, search by personal project code, and sorting by popularity are available.
After the match ends, players can rate other players' projects by giving a rating from 1 to 5 stars.

## Editor
In the editor, you can create your own game modes.
Settings for various aspects of gameplay are available, including spawn points, vehicles, objects, pickups, NPCs, weapons, and much more.
Tutorials for all modes and a guide on how to use the editor are provided.

![Screenshot](https://github.com/Bren828/Custom-Play-Hub/blob/main/menu-1.jpg)
![Screenshot](https://github.com/Bren828/Custom-Play-Hub/blob/main/menu-2.jpg)

---

# Modes

### Race
In racing mode, players compete against each other, trying to be the first to reach the finish line.

#### Gameplay
- At the start of the race, players can use a dash that accelerates their vehicle at launch.
- On the track, you can collect acceleration, vehicle repair, and jump pickups.
- Rockets are available to attack opponents.
- Players who finish earlier than others enter spectator mode.
- A leaderboard is available to players, displaying current positions in the race.


### Deathmatch
In Deathmatch mode, players fight each other in a free-for-all format, trying to get the highest number of kills.

#### Gameplay
- A weapon store is available to players where they can choose the necessary weapons.
- A leaderboard is available to players, displaying current positions in the match.
- Assist system.


### Team Deathmatch
In Team Deathmatch mode, players are divided into two teams — blue and red — and fight each other.
The team that first depletes the opponent's points to zero or maintains the highest number of points when the match time expires wins.

#### Gameplay
- Each team is given a certain number of points at the beginning of the round (e.g., 200).
- For every kill of an enemy player, 1 point is deducted from the opposing team.
- A weapon store is available to players where they can choose the necessary weapons.
- A leaderboard is available to players, displaying current positions in the match.
- Assist system.


### Counter-Strike
In Counter-Strike mode, players are divided into two teams: terrorists and counter-terrorists.

#### Team Objectives
- Counter-terrorists - defuse the bomb or eliminate all terrorists.
- Terrorists - plant and explode the bomb or eliminate all counter-terrorists.

#### Gameplay
- Rounds last until one team wins or time expires.
- Money is awarded for wins and kills depending on the weapon and method of elimination.
- Money can be used to buy weapons and equipment.
- The losing team receives a loss streak bonus.
- Mechanics for defuse kits, helmets, assists, round MVP, weapon drop upon death, buy phase at the start of the round, and side swapping at the midpoint of the match.
- Eliminated players enter spectator mode for their team.
- A leaderboard is available to players, displaying current positions.
- The bomb is automatically dropped if a player is inactive for a long time.

![Screenshot](https://github.com/Bren828/Custom-Play-Hub/blob/main/kit.jpg)

### Counter-Strike Economy
Accrual of money for specific actions in the match.

<details>
<summary>Economy</summary>

#### Basics
- Starting money: $800
- Maximum money: $16000

#### Team Reward
- Won round: $3250
- Bomb explosion: $3500
- Bomb defusal: $3500
- Elimination of all enemies: $3250

#### Individual Reward
- Planting the bomb: $300
- Defusing the bomb: $300
- Killing the bomb planter: $50
- Killing the bomb defuser: $50
- Killing the bomb carrier (before planting): $50

#### Loss Bonus (Loss streak)
- First loss: $1400
- Second loss: $1900
- Third loss: $2400
- Fourth loss: $2900
- Fifth loss: $3400

#### Money for kill with specific weapon
- Pistol: $300
- Shotgun: $900
- SMG: $600
- Assault Rifle: $300
- Sniper Rifle: $100
- Grenade: $300
- Melee weapon: $400

#### Penalties
- Team kill: $300
- Suicide: $300
</details>


### Duel
In Duel mode, players are divided into two teams — blue and red — and fight each other.
The goal is to win a certain number of rounds to win the match.

#### Gameplay
- Rounds last until one team wins or time expires.
- Eliminated players enter spectator mode for their team.
- A weapon store is available to players where they can choose the necessary weaponry.
- A leaderboard is available to players, displaying current positions in the match.
- Helmet mechanics, assists, round MVP, buy phase at the start of the round, side swapping at the midpoint of the match.


### Derby
In Derby mode, players deal damage to each other using vehicles.

#### Gameplay
- Each player has a limited number of lives.
- Repair, acceleration, and rocket pickups can be scattered around the arena.
- Players who lose all their lives are eliminated and enter spectator mode for the remaining participants.
- A dash is available at the start of the derby, which accelerates the vehicle at launch.
- Rockets are available to attack opponents.
- A leaderboard is available to players, displaying current positions in the derby.

---

# Editor

_Various gameplay settings are available in the editor, including spawn points, vehicles, objects, pickups, and much more.
The editor also provides tutorials for all modes and a complete usage guide._


### Element Selector

This is a tool in the mode editor that allows adding various elements to the project.
Depending on the selected mode, corresponding elements for addition will be displayed.

![Screenshot](https://github.com/Bren828/Custom-Play-Hub/blob/main/selector.jpg)


### Checkpoints
Checkpoints are used in racing mode to mark the route that players must follow.

#### Checkpoint Properties
Each point has customizable properties.

- Type - regular or aerial checkpoint
- Width - defines the width of the checkpoint
- Vehicle change - allows changing the player's vehicle when passing through the checkpoint
- Vehicle speed - sets the vehicle speed when passing through the checkpoint


### Vehicle Spawn Points
Vehicle spawn points determine the locations where players can appear in a vehicle in racing mode or other modes.

#### Vehicle Properties
Each vehicle has customizable properties.

- Model - the vehicle that will be used (car, motorcycle, bicycle, etc.)
- Paint - vehicle color and paint job
- Nitro - set the presence of nitro for the vehicle
- Accessibility - determines who can use this vehicle (all players or only specific teams)
- Doors - management of the vehicle door state (open or closed)
- Respawn delay - after the player exits the vehicle, a countdown to respawn will begin

![Screenshot](https://github.com/Bren828/Custom-Play-Hub/blob/main/color.jpg)

### Objects
Objects allow adding various environmental elements to the project, such as buildings, trees, roads, etc.
There are two ways to add objects: using the standard GUI editor or via camera aiming.

The ColAndreas plugin is used for collision detection.

![Screenshot](https://github.com/Bren828/Custom-Play-Hub/blob/main/submenu.png)

### Player Respawn Points
Player respawn points determine the locations where players appear after death in certain modes.

#### Respawn Point Properties
Each point has customizable properties.

- Team - determines which team the point is intended for (used in team mode)


### Bomb Plant Sites
Bomb plant sites are used in Counter-Strike mode to mark locations where players can plant bombs.


## Pickups
Pickups are used to provide players with various bonuses and resources during the game.

#### Pickup Properties
Each pickup has customizable properties.

- Type - defines the type of pickup (health, armor, weapons, ammo, adrenaline, etc.)
- Number of uses - the number of times the pickup can be used before disappearing
- Pickup recovery delay - the time after which the pickup will become available for use again
- Delay effect action - determines for whom the recovery delay applies (all players or only a specific one)
- Pickup accessibility - determines how the pickup can be used (player or vehicle)
- Pickup purpose - determines who can use this pickup (all players or only specific teams)

#### Pickup Types
- Health — restores the player's health.
- Armor — adds armor to the player.
- Weapon — gives the selected weapon.
- Ammo — adds ammunition.
- Adrenaline — gives temporary bonuses (speed boost).
- Lethal — the player dies upon pickup.
- Explosive — explodes on contact.
- Jump — launches the vehicle or player upwards.
- Vehicle repair — restores a damaged vehicle.
- Vehicle acceleration — gives a short-term speed boost.
- Vehicle rocket — allows launching rockets from the vehicle.

![Screenshot](https://github.com/Bren828/Custom-Play-Hub/blob/main/pickup.png)

### NPC
NPCs are used to create background crowds and interact with lobby stages.

#### NPC Properties
Each NPC has customizable properties.

- Skin - the NPC's appearance
- Animation - defines the NPC's pose or action (sitting, standing, lying down, etc.)
- Animation loop - determines whether the animation will repeat cyclically
- Animation trigger action - determines how the NPC animation will be triggered (during the pre-game countdown or at game completion)

#### Animation Trigger Actions
This function allows triggering NPC animations depending on the lobby game stages.
For example, you can set an NPC to perform a certain animation during the countdown before the game starts or when it ends.

---

# Options

### Weapon Store
In some game modes, players can buy weapons and equipment at the weapon store.
The store assortment is configured in the project parameters.

#### Weapon Return
- When buying or choosing a weapon, a player can return it to the store and get back the money spent.

#### Limitations
- The weapon store can only be used within a 5-meter radius of the last spawn point.
- After spawning, there is a purchase time limit of 30 seconds.
- A player cannot get a refund for a weapon if it was issued for free at spawn.
- A player cannot get a refund for a weapon if it was received from another player.

![Screenshot](https://github.com/Bren828/Custom-Play-Hub/blob/main/store.png)


### Leaderboard
The leaderboard displays the best players, sorted by their results.

![Screenshot](https://github.com/Bren828/Custom-Play-Hub/blob/main/table.png)


### Tags
Tags help other players find your project using specific keywords.


### Camera Position
The camera determines where the player will look at certain moments of the game.

#### Starting Camera
- Used in the lobby while waiting for players
- Displayed during the countdown before the start
- Helps players see the map before starting

#### Ending Camera
- Shown after the match/race ends
- Displayed during the results reveal


### Project Rating/Review
Project rating allows players to rate your project after finishing the game.

#### How it works
- Players give a rating from 1 to 5 stars
- The average rating is displayed in the list of projects and lobbies
- A high rating helps the project rise in search results

You can view detailed rating statistics for your project in the statistics section.


### Project Views
Views show how many times players have launched your project.

#### What counts as a view
- Every time a player enters a lobby with your project
- A high number of views helps the project rise in search results

#### Project Launches
- Shows how many times a player has created a lobby with your project

You can view detailed view statistics in the statistics section.


### Personal Project Code
A personal project code is a unique identifier for your project, used for identification and access.

#### Code Generation
- The code is generated automatically when the project is saved
- Includes the project ID and random characters

#### Code Usage
- Allows other players to find your project using this code

You can find your project's personal code in the statistics section.


### Project Publication
Publishing a project makes it available to other players in the project list.
Certain requirements must be met to publish a project.

#### Requirements Example
- Place checkpoints
- Set vehicle spawn points
- Set respawn points
- Place bomb plant sites
- Choose the lobby camera position

After fulfilling all requirements, the project can be published via project options.

![Screenshot](https://github.com/Bren828/Custom-Play-Hub/blob/main/publication.png)

---

## Price

Price: **80,000 RUB**

Review server: IP: **185.223.168.92:7777**
#### _For a full test, you need to install a mod for the game - [KeyListener](https://github.com/CyberMor/keylistener)_

---

## Contacts for communication:

- Telegram: **[@Bren828](https://t.me/Bren828)**
- VK: **[@Bren828](https://vk.com/bren828)**


## Dependencies

- ColAndreas
- [KeyListener](https://github.com/CyberMor/keylistener) **Required!**
- streamer 
- mysql R41-4
- pawnraknet 
- pawnregex 
- sscanf 
- rustext
