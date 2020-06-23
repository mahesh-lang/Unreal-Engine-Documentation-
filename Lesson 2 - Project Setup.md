# Lesson 2
# Project Setup

1. Create the project named 'SteamProject'.
2. Go to marketplace and import some characters. 
3. We will import 'Infinity Blade:Warriors' pack.
4. Set the folder structure. 
- Content - New Folder - Name that folder 'Blueprints' - This folder will hold all the blueprints of our project.
-   New Folder - Name this folder 'Maps' - This folder will hold all the maps of our project.
-   New Folder - Name this folder 'Textures' - This folder will hold all the thumbnails of our maps and characters of the character select screen.
-   New Folder - Name this folder 'UI' - This folder will hold all the UI content of our project.

5. Now, the 'Blueprints' and UI folders will contain some sub-folders. 
- Blueprints Folder 
1. 'AllLevels' - This will contain the blueprints used across all the levels. 
2. 'AllLevels' - This will contain all the characters blueprints.
3. 'Gameplay' - This will contain all the gameplay related blueprints.
4. 'Lobby' - This will contain all the lobby related blueprints.

- UI Folder

1. 'AllLevels'
2. 'Lobby'
3. 'MainMenu'


6. Now, we will create some assets we are going to be needing. 
- Assets in Blueprints folder (AllLevels) 
1. Right click - Bluprint Class- search 'gameinstance' select  and name it 'GameInfoInstance' - Spawned at game creation and it is never destroyed. 
2. Right click - Blueprints - Structure - 'PlayerInfo' - this will hold all the information of our project such as name, avatar, etc. 
3. Right click - Blueprints - Blueprint class - search 'gamesave' select and name it 'PlayerSaveGame' - This will save information of the player locally and then upload that information to our server who will distribute that to all of the clients and then our clients will know our names, our characters etc. 

- Assets in Blueprints folder (Characters) 
1. Go to 'ThirdPersonBP', select the 'Third person character' and drag it into our 'Characters' folder. Rename this as '0_Base' - this will be our base character.
2. Create child blueprint from this base character so it will inherit all of that movement functionality, and also other changes we make to this will be passed on to this children. So it will be easier to have different characters down the road. 
 Right click - 'create child Blueprint class', name it 'Barbarous'
3. Dupliate this with ctrl+w and name it 'Forge'. Do this again and create these characters - Frosty, Natural, Pit, Robo, Tusk, Warrior. We should have total 9 characters. 0_Base is a base character. We will have eight playable characters that you choose from. 

- Assets in Blueprints folder (Gameplay) 

1. Right click - Bluprint class - Game mode - name it 'GameplayGM'
2. Right click - Bluprint class - player Controller - name it 'GameplayPC'

- Assets in Blueprints folder (Lobby)
 Select both of the above items of Character folder and drag them into Lobby folder and rename them as 'LobbyGM' and 'LobbyPC' One for actual gameplay and another for when we are inside of the lobby. 

7. Now, Lets create some maps. 
 Arena01, Arena02, Lobby map,Travel map(this is the map we are going to use when we travel from the lobby to actual gameplay.) menu map, transitional map

- Assets in UI folder (AllLevels)
1. Right click - UI Interface - Widget Bluprint. name it 'ChatText' -  for the text that appear on our chat window. 
 2. Ctrl+w 'ChatWindow'  - Actual window with all our chat text lines.
 3. Ctrl+w 'GameplayChat' -  for game play chat
 4. Ctrl+w 'LoadingScreen'

- Assets in UI folder (Lobby)
1. CharacterSelect - for character select screen
2. ConnectedPlayer - for playercard when someone joins the lobby
3. GameSettings -   game settings menu that the server can define. 
4. LobbyMenu
5. PlayerButton -  Used by the server only, this will allow server to kick someone from the lobby

- Assets in UI folder (MainMenu)
1. ErrorDialogue - for error messages on the front end
2. HostMenu
3. MainMenu
4. OptionsMenu
5. ServerMenu


8. Some project settings.
9. Set up the animation blueprint for our characters.   