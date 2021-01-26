# Construct a Minecraft:JAVA Edition Server

------

## Build Minecraft Server

1. Purchase a server that meet your need
   
   *Linux is recommended, it won't take up much system resources. However, Windows 2008 server have GUI so you can operator on it easily.*

> LESS system take up means GOOD game server performance !

   ![pic1.png](res\pic1.png)

2. Write down the **Public IP**  which we will use later.

3. Download Minecraft Server jar file (server.jar) from [Minecraft official website](https://www.minecraft.net/en-us/download/server/) , write down the command provided.
   *Server edition should match your game edition*
   
   ![pic2.png](res\pic2.png)

4. Start the server you have purchased, use any methods you can to connect to the server.

> Here I provide Windows method.

   (1)Press WIN button and R button to get this window

   ![pic3.png](res\pic3.png)

   (2)Do the following steps

   ![pic4.png](res\pic4.png)

   ![pic5.png](res\pic5.png)

   ![pic6.png](res\pic6.png)

5. After you connect to the server, in server download jre (dowload jre varys from different Operating System according to your Server) and install to your computer.
   
   *ensure you have the "java" command in your system environment variables*

6. Create a folder named "MC", put server.jar file in it. Rename the "server.jar" to "minecraft_server.1.16.4.jar" (the name same as the command provided)

7. Open cmd and navigate to "MC" folder, execute command as followed(The command in Minecraft official site, whose parameters can be modified according to your server capacity)
   
   `java -Xmx2G -Xms2G -jar minecraft_server.1.16.4.jar nogui`

8. The first time you run the command, it will meet an error and stop. Open the "MC" folder and you can see several files has been generated. Find a file "eula.txt", open it and reset the eula value to true. Re-execute the command, it will run correct and the server can be found in game.
   
   ![pic7.png](res\pic7.png)
   
   ![pic8.png](res\pic8.png)

> Everytime you want to start the server, you will need to execute the command. (The server need not close everytime you exit the game, it can keep running)

## Mod a server

#### On server part:

1. Create another folder "MC_forge"

2. Download forge from [Forge Official website](https://files.minecraftforge.net/) , put "minecraft_server.1.16.4.jar"(initial named "server.jar") and forge installer file together in it.

![pic9.png](res\pic9.png)

2. Execute the jar file to install forge

![pic10.png](res\pic10.png)

3. Wait for the download(need network), it automatically prepares things you need.

4. The following steps are same as run native minecraft server, except you should use this command
   
   `java -Xmx2G -Xms2G -jar forge-1.16.4-35.1.4.jar`

5. The modded server can be found in game. To add mods, you can place .jar file mods in the folder called mods. 

#### On client part:

1. Download the forge installer same version as the server uses.

2. Execute the jar file to install forge, choose "Install client"

3. Wait download to complete.

4. Open Minecraft Launcher and you will see the forge version exist.

![pic11.png](res\pic11.png)

5. (**Option**)To avoid native minecraft conflict with your modded one, you can specify another folder to hold the forge version game. this folder should have name ".minecraft"
   
   ![pic12.png](res\pic12.png)
   6. Find your game directory, you will see a folder named "mods". Here you can put .jar mod files to add mods to your game.



> Although server hold the mods, the client have to use forge minecraft equipted with the same mods in local so that the mods can be used in game 
