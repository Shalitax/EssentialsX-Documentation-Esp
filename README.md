<h2> EssentialsX </h5>
<h3> Features </h3>


 - Kits 
 - VoteDayNight
 - AutoClearConfig
 - AntiSpam
 - NoName
 - SpawnProtectionConfiguration
 - DeathMessages
 - Duty
 - TPA
 - Home
 - ItemBlock
 - Warps
 - BlockDamage
 - CheckLag
 - Stats
 - NoGlobalMessages
 - TextCommands
 - Block Repair
 - Decal Remover
 - Ranks
 - Vaults
 - AntiAdminAbuse
 - OldGravity
 - JoinMessages
 - Lobby (/SETLOBBY)
 - SalvageModifier
 - AnnouncerConfig
 - CommandHelper


<h2>Kits</h2>



<h4>Commands</h4>

1. /createkit, /ckit, /kicreate  <b>[[Syntax]] /createkit [name] [cooldown] [permission]</b>
   - With this command, you can create kits (Copy your inventory at the time of creating the kit).
2. /deletekit, /delkit /dkit  <b>[[Syntax]] /createkit [name]</b>
   - With this command, you can delete the kit that is inside /kits.
3. /kit  <b>[[Syntax]] /kit [name]</b>
   - With this command, you can select a kit created using /kit <name>.
4. /kitcooldown, /kitcd  <b>[[Syntax]] /kitcooldown [kit]</b>
   - With this command, you can set a different cooldown for a kit.
5. /kiteconomy, /kiteco, /kite, /kitexperience /kitex <b>[[Syntax]] /kiteconomy [kit] [balance]</b>
   - With this command, you can set a different cooldown for a kit.
6. /kits <b>[[Syntax]] /kits[kit]</b>
   - With this command, you can see a list in the in-game chat of all the kits that the player has access to.
7. /kitvehicle, /kitv  <b>[[Syntax]] /kitvehicle [kit] [vehicleId]</b>
   - With this command, you can view a list in the in-game chat of all the kits that the player has access to.
8. /migratekit <b style=color:red>WARNING: </b>
     - <p style=color:red>This command is only used in case you have your kits in AviKits and want to migrate them to <b>EssentialsX</b>, but it's not 100% accurate. Some kits may generate incorrectly and lose some items. It is recommended to review them.</p>

<hr />
<h5>Configuration</h5>

```xml
<?xml version="1.0" encoding="utf-8"?>
<EnvyKitsConfiguration xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
  <UseEconomy>false</UseEconomy>
  <icon>url here</icon>
</EnvyKitsConfiguration>
```

<h5>Translations</h5>

```xml
<?xml version="1.0" encoding="utf-8"?>
<Translations xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
  <Translation Id="kit:exist" Value="The kit already exists" />
  <Translation Id="kit:nokits" Value="Unable to Find Kits" />
  <Translation Id="kit:list" Value="Kits: {0}" />
  <Translation Id="kit:notfound" Value="The kit {0} does not exist" />
  <Translation Id="kit:nopermissions" Value="You do not have sufficient permissions to use any kit" />
  <Translation Id="kit:nopermission" Value="You do not have sufficient permissions to use this kit." />
  <Translation Id="kit:delete" Value="The kit {0} has been removed" />
  <Translation Id="kit:nomoney" Value="You don't have enough money to buy: {0}" />
  <Translation Id="kit:create" Value="You have created the kit {0}" />
  <Translation Id="kit:give:admin" Value="You have received the kit {0} by the administrator" />
  <Translation Id="kit:give" Value="Has obtenido el kit {0}" />
  <Translation Id="kit:cooldown" Value="You have to wait {0} seconds to use the kit again" />
</Translations>
```

<h3>Auto Clear Config</h3>
Enabling this function deletes the items on the ground or those configured within the settings.
<hr />


<h5>Configuration</h5>

1. <b>Time_Barricades / Barricades</b>
   - Activating this option for the configured time will remove barricades (Lockers, Signs, Beds, etc).
2. <b>Time_Items / Items</b>
   - Activating this option for the configured time will remove all objects from the floor of the map.
3. <b>Time_Vehicles / Vehicles</b>
   - Enabling this option for the configured time will remove all items from the floor of the map
4. <b>Time_Structures / Structures</b>
   - Activating this option for the configured time will remove structures (Wooden floors, metal floors, pillars, etc).
<h3>Anti Spam</h3>
This prevents users from sending the same message repeatedly and spamming the chat.

<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable
2. <b>Interval</b>
   - The waiting time to be able to send a message after another.



<h3>NoName</h3>
The users within the server cannot see the name of another person's character. <br/>
 <p style="color: red"> Use For  Roleplay</p>
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable
2. <b>Bypass</b>
   - When you activate the bypass, administrators will only be able to see the names of the players.
<h3>SpawnProtection</h3>
When you respawn, you appear with a spawn protection.
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable
2. <b>Vanish Mode</b>
   - This option allows players to appear invisible.
3. <b>Expire On Execute Command</b>
   - When any command is used, the protection is removed.
4. <b>Protection Seconds</b>
   - The time a player has for protection.
<h3>Death Messages</h3>
It displays messages of player deaths or their killers, and everything can be configured, from the images to the colors.
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable
2. <b>Show Location</b>
   -  Enable/Disable
<h3>Duty</h3>
Allows players to remove their administrator powers using a command ("/DUTY").
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable
2. <b>Permission</b>
   -  Set Permission
<h3>TPA</h3>
Allows sending teleportation requests to other players, and they can choose to accept or decline them.
<hr />

<h4>Commands</h4>

1. /tpa  <b>[[Syntax]] /tpa [player] </b>
   - With this command, you can send TPA to other players
2. /tpa  <b>[[Syntax]] /tpa mode [group/global]</b>
   - If you enter "/tpa mode group," only players in your group can send you teleportation requests, and if you enter "/tpa mode global," anyone can send you requests.

<h5>Configuration</h5>

1. <b>Interval</b>
   - Set Interval Time
2. <b>Expiration</b>
   - Set Expiration Time
<h3>Home</h3>
Allows you to teleport to your bed.
<hr />

<h4>Commands</h4>

1. /home

<h5>Configuration</h5>

1. <b>Interval</b>
   - Set Interval Time
2. <b>Block Moving</b>
   - If the player moves while in the cooldown or interval period, the teleportation is canceled.

<h3>Item Block</h3>
This option is in <b>BETA</b> state, but it allows blocking the items that the user picks up.
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable

```
    <Items>
      <Item ID="363" Permission="bypass.363" />
    </Items>
```

<h3>Warp</h3>
Allows you to set teleportation locations.
<hr />

<h4>Commands</h4>

1. /createwarp, /cwarp, /setwarp <b>[[Syntax]] /createwarp [name] [permission] [interval] </b>
   - With this command, you create a point where you are standing so that players can teleport to it using "/warp [name]."
2. /deletewarp, /delwarp <b>[[Syntax]] /deletewarp [name]</b>
   - Delete warp
2. /warp<b>[[Syntax]] /warp [name]</b>
   - With this command, you can teleport to a specific point.
2. /warps
   - With this command, you can view a list of teleportation points available and use "/warp [name]" to teleport to a specific one.

<h5>Configuration</h5>

1. <b>Interval</b>
   - Set Interval Time
2. <b>Expiration</b>
   - Set Expiration Time
<h3>Block Damage</h3>
Allows blocking raid damage to configured entities, including damage to structures, barricades, and wheeled vehicles.
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable
1. <b>BlockDamageOfBarricades</b>
   - Enable/Disable
1. <b>BlockDamageOfVehicles</b>
   - Enable/Disable
1. <b>BlockDamageOfStructure</b>
   - Enable/Disable
1. <b>BlockDamageOfVehicles_Tire</b>
   - Enable/Disable

<h3>CheckLag</h3>
Allows the server to perform a restart when the TPS (Ticks Per Second) falls below 20 or 10. This is a common occurrence when the server has been running for an extended period without restarting, leading to a significant drop in TPS.
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable
1. <b>AutoShutdown</b>
   - Enable/Disable
1. <b>Seconds</b>
   - Set Seconds

<h3>Stats</h3>
Allows you to have a record of all the statistics of players within the server, including kills, deaths, etc.
<hr />


<h4>Commands</h4>

1. /stats <b>[[Syntax]] /stats [player] </b>
   - With this command, you can view the statistics of another player.
2. /stats 
   - With this command, you can view your statistics.
2. /ranking
   - With this command, you can see TOP players


<h5>Configuration</h5>

1. <b>Enable</b>
2. <b>Top Max</b>
<h3>No Global Messages</h3>
Allows users, except administrators, to write in WORLD; they can only write in AREA or GROUP.  <br />
<p style="color:red">(This is for roleplay purposes.)</p>
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable

<h3>TPA</h3>
Allows sending teleportation requests to other players, and they can choose to accept or decline them.
<hr />

<h4>Commands</h4>

1. /tpa  <b>[[Syntax]] /tpa [player] </b>
   - With this command, you can send TPA to other players
2. /tpa  <b>[[Syntax]] /tpa mode [group/global]</b>
   - If you enter "/tpa mode group," only players in your group can send you teleportation requests, and if you enter "/tpa mode global," anyone can send you requests.

<h5>Configuration</h5>

1. <b>Interval</b>
   - Set Interval Time
2. <b>Expiration</b>
   - Set Expiration Time
<h3>Home</h3>
Allows you to teleport to your bed.
<hr />

<h4>Commands</h4>

1. /home

<h5>Configuration</h5>

1. <b>Interval</b>
   - Set Interval Time
2. <b>Block Moving</b>
   - If the player moves while in the cooldown or interval period, the teleportation is canceled.
<h3>Item Block</h3>
This option is in <b>BETA</b> state, but it allows blocking the items that the user picks up.
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable

```
    <Items>
      <Item ID="363" Permission="bypass.363" />
    </Items>
```

<h3>Warp</h3>
Allows you to set teleportation locations.
<hr />

<h4>Commands</h4>

1. /createwarp, /cwarp, /setwarp <b>[[Syntax]] /createwarp [name] [permission] [interval] </b>
   - With this command, you create a point where you are standing so that players can teleport to it using "/warp [name]."
2. /deletewarp, /delwarp <b>[[Syntax]] /deletewarp [name]</b>
   - Delete warp
2. /warp<b>[[Syntax]] /warp [name]</b>
   - With this command, you can teleport to a specific point.
2. /warps
   - With this command, you can view a list of teleportation points available and use "/warp [name]" to teleport to a specific one.

<h5>Configuration</h5>

1. <b>Interval</b>
   - Set Interval Time
2. <b>Expiration</b>
   - Set Expiration Time
<h3>Block Damage</h3>
Allows blocking raid damage to configured entities, including damage to structures, barricades, and wheeled vehicles.
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable
1. <b>BlockDamageOfBarricades</b>
   - Enable/Disable
1. <b>BlockDamageOfVehicles</b>
   - Enable/Disable
1. <b>BlockDamageOfStructure</b>
   - Enable/Disable
1. <b>BlockDamageOfVehicles_Tire</b>
   - Enable/Disable

<h3>CheckLag</h3>
Allows the server to perform a restart when the TPS (Ticks Per Second) falls below 20 or 10. This is a common occurrence when the server has been running for an extended period without restarting, leading to a significant drop in TPS.
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable
1. <b>AutoShutdown</b>
   - Enable/Disable
1. <b>Seconds</b>
   - Set Seconds


<h3>Stats</h3>
Allows you to have a record of all the statistics of players within the server, including kills, deaths, etc.
<hr />


<h4>Commands</h4>

1. /stats <b>[[Syntax]] /stats [player] </b>
   - With this command, you can view the statistics of another player.
2. /stats 
   - With this command, you can view your statistics.
2. /ranking
   - With this command, you can see TOP players


<h5>Configuration</h5>

1. <b>Enable</b>
2. <b>Top Max</b>
<h3>No Global Messages</h3>
Allows users, except administrators, to write in WORLD; they can only write in AREA or GROUP.  <br />
<p style="color:red">(This is for roleplay purposes.)</p>
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable


<h3>Block Repair</h3>

Allows users to be unable to repair barricades, vehicles, or structures, all of which are configurable.
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable
1. <b>Barricades</b>
   - Enable/Disable
1. <b>Structures</b>
   - Enable/Disable
1. <b>Vehicles</b>
   - Enable/Disable
<h3>Decal Remover</h3>

This option allows you to clean up unnecessary effects within the game, such as tree leaves, wood particles, smoke, bullet impacts, and more.
<b>+FPS</b>
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable
<h3>Vaults</h3>

Allows users to have additional chest spaces using commands.
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable

```
Example.
    <Vaults>
      <Vault Name="VIP" Permission="vault.vip" SizeX="50" SizeY="50" />
      <Vault Name="USER" Permission="vault.user" SizeX="10" SizeY="10" />
    </Vaults>
```
<h3>CommandHelper</h3>

With this enabled, whenever a person enters a command like "/wa," they will see that they have access to "/warps" or "/warp" (provided they have the necessary permissions for those commands).
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable

<h3>Announcer</h3>

Allows sending announcements at regular intervals within the server to inform users.
<hr />


<h5>Configuration</h5>

1. <b>Enable</b>
   - Enable/Disable

```
<Messages>
      <Message Message="#1 - No Hacks" Image="url here" />
      <Message Message="#1 - No Toxic" Image="url here" />
      <Message Message="#1 - No Bugs" Image="url here" />
    </Messages>
```

<h3>Commands EssentialX</h3>

Generally, it has all the most commonly used commands from Avi and Essentials, and I've only added a few that I found useful.
<hr />


<h5>Commands</h5>

1. <b>/catch [player]</b>
   - With this command, you can view a player's inventory as if it were a chest and loot or remove their weapons, similar to Minecraft's "/invsee."
1. <b>/door</b>
   - With this command, you can open doors of any player (provided you have permissions and are looking at the door).
1. <b>/storage </b>
   - With this command, you can open storages of any player (provided you have permissions and are looking at the storage).

1. <b>/speed [number]</b>
   - With this command, you can increase your speed.
1. <b>/sudo [player] or [*]</b>
   - If you use *, you are executing this command for all users on the server, for example: /sudo * "/tpa Margarita".
   - You can also send messages using /sudo * "hello world," and everyone will write "hello world."
   - You can execute the command for a single person using, for example: /sudo Margarita "/kit maplestrike."






<h3>TextCommands</h3>

With this option, you can enable text commands, create commands that only return useful text for creating rules
<hr />

```
  <TextCommand Name="rules" Icon="" Help=":V">
      <Messages>
        <string>No Hack</string>
        <string>No Bug - No Toxic</string>
        <string>FUN :P</string>
      </Messages>
    </TextCommand>
```



<h3>Anti Admin Abuse</h3>

When enabling this option, all administrators, while using GOD, VANISH, or AERIAL CAMERA, will send a message to the general chat indicating that the administrator is abusing their power.
<hr />


<h3>Old Gravity</h3>

Enabling this option allows you to configure the player's gravity
<hr />

```  
<OldGravityConfig Enabled="false">
    <GravityMultiplier>0.97</GravityMultiplier>
  </OldGravityConfig>
```



<h3>Join Messages</h3>

You can enable player entry/exit messages
<hr />

```  
  <JoinMessagesConfig Enabled="true" />
```


<h3>Lobby</h3>

By placing a 'SetLobby' command at the point where you put this command, all players will appear in the Lobby when they connect or respawn.
<hr />

<h5> Commands </h5>

 - /setlobby

```  
  <LobbyConfiguration Enabled="true" PositionCoords="" />
```

<h3>Ranks</h3>

It allows you to create ranks within the server and grant ranks to users as a reward for achieving an accomplishment
<hr />

<h4> Usage </h5>

 1. If you enable '**RankConfig**' in the configuration and set it to **True**, and then execute 

 

>        /rocket reload essentialsX

 Go  **Rocket/Plugins/EssentialsX** folder, a file named 'Ranks.json' will be generated.

 2.  Ranks Default:

```xml
    {
    "Rank": [
      {
        "Name": "rango1",
        "Reputation": -1000,
        "Crafting": 0,
        "Zombies": 0,
        "MegaZombies": 0,
        "FoundedItems": 0,
        "FoundedPlants": 0,
        "Fishing": 0,
        "Animals": 0,
        "GroupToWin": "rango1"
      },
      {
        "Name": "rango2",
        "Reputation": -2000,
        "Crafting": 0,
        "Zombies": 0,
        "MegaZombies": 0,
        "FoundedItems": 0,
        "FoundedPlants": 0,
        "Fishing": 0,
        "Animals": 0,
        "GroupToWin": "rango2"
      },
      {
        "Name": "rango3",
        "Reputation": -3000,
        "Crafting": 0,
        "Zombies": 0,
        "MegaZombies": 0,
        "FoundedItems": 0,
        "FoundedPlants": 0,
        "Fishing": 0,
        "Animals": 0,
        "GroupToWin": "rango3"
      }
    ]
  }
]
```
<h4> Information</h5>

The rank system, those listed within **'Ranks.json'** in the **Rocket/Plugins/EssentialsX** folder, will automatically create ranks within the **Permissions.xml** when you restart using 

    /rocket reload essentialsX

 or when you start the server. ***It's important to note that it generates the default three sample ranks, so it's necessary to delete them if you don't want them***

<h3>Salvage Modifier</h3>

With this option, you can change the speed of building structures or barricades within the game, and you can configure it so that different users have different speeds
<hr />



*The lower the '**Force**' value, the faster it will remove structures. It allows decimals*


```  
   <SalvageRanks>
      <SalvageRanks Permission="marga.vipalto" Force="3" />
      <SalvageRanks Permission="marga.vipnoob" Force="5" />
    </SalvageRanks>
```


<h3>Command Helper</h3>

Enabling this option allows users that when they execute a command that doesn't exist, it provides them with help. For example, if a user enters /tpe, and it doesn't exist but /tpa does, it will show that /tpa is a valid command
<hr />

```  
   <CommandHelperConfig Enabled="true" Icon="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3f/Logo_informations.svg/1024px-Logo_informations.svg.png" />
```


