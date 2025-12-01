---
name: Crooz
subtitle: 'Final Fantasy Grandmasters, ACR Drift'
start_date: 2014-01-01
end_date: 2016-10-31
external_url: 'https://crooz.co.jp/'
image_path: /images/clients/crooz/ffgm/Final-Fantasy-Grandmasters_thumb.jpg
---
## ![](/portfolio/images/clients/crooz/crooz-logo-large.jpg){: width="1800" height="971"}

# CROOZ

2014/01 ~ 2016/10 <br/>
Lead Technical Artist <br/>
Unity Game Development Team <br/>
Tokyo, Japan <br/>

## Game Titles

| Final Fantasy Grandmasters                                                                           | ACR Drift                                                                                       |
| ---------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| ![](/portfolio/images/clients/crooz/ffgm/Final-Fantasy-Grandmasters.jpg){: width="640" height="480"} | ![](/portfolio/images/clients/crooz/acr-drift/acr-drift-splash.jpg){: width="640" height="480"} |
| ---                                                                                                  | ---                                                                                             |

## Overview
At CROOZ I worked on various unity mobile game projects, developed DCC tools and game engine tools, created shaders and post effects, and also performed research and development work. <br/>
Tools and effect systems I developed were featured in a presentation at the Unite Tokyo 2016 game developer conference.
I also received an award from the company president for improving development productivity and efficiency, and reducing development costs.

### Material Animation System For Unity 5
At the request of the Art Director, I researched and developed a method for animating Unity 5 materials using custom shaders, custom scripts and custom animation data exported from Maya.  <br/>
The material animation was used to animate magic effects in a fantasy RPG game for mobile.
The animated material properties included: Color, Alpha, UV Translation, UV Rotation, UV Scaling and UV Offsets.
I created custom unity asset importers to import the material animation from FBX file and automatically setup the unity game assets, such as animation clips, animator controllers, material shaders and prefabs. <br/>

| ![](/portfolio/images/clients/crooz/unite-2016-tokyo/Maya_Material_Anim_Exporter_3.png){: width="320", height="240"} | ![](/portfolio/images/clients/crooz/unite-2016-tokyo/Maya_Material_Anim_Exporter_4.png){: width="320", height="240"} |
|---------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
|                                                                                                                     |                                                                                                                     |

### Material Animation Exporter For Maya
Artists were required to create magic effects for a fantasy RPG game and wanted to create the effects in Maya using material animation.  <br/>
To export the material animation data, I extended the Maya FBX model exporter and marked the data as custom Unity asset data.  <br/>
The extended FBX exporter was written in C++ using the Autodesk FBX SDK.

| ![](/portfolio/images/clients/crooz/unite-2016-tokyo/Maya_Material_Anim_Exporter_1.png){: width="320", height="240"} | ![](/portfolio/images/clients/crooz/unite-2016-tokyo/Maya_Material_Anim_Exporter_2.png){: width="320", height="240"} |
|-----------------------------------|---------------------------------------------------------------------------------------------------------------------|
|                                   |                                                                                                                     |

### Asset Setup Tools For Unity 5
Initially the game development team was setting up Unity game assets by hand, and it was taking a lot of time. <br/>
To improve the art and game asset pipeline, I created various tools to automatically handle import of art assets and automatically setup game assets, such as animation clips, animation controllers, models, material shaders and prefabs.  <br/>
I also created an automated asset import batching tool to handle large processing large volumes of FBX assets.  <br/>
The tools helped to drastically cut the amount of time spent on setting up the game assets in Unity. <br/>

| ![](/portfolio/images/clients/crooz/unite-2016-tokyo/Batch_Prefab_Tool_Intro.png){: width="320", height="240"} | ![](/portfolio/images/clients/crooz/unite-2016-tokyo-2/ffgm_prefab_creator_batch_tool.jpg){: width="320", height="240"} | ![](/portfolio/images/clients/crooz/unite-2016-tokyo-2/Unity_Prefab_Creaton_Tool.png){: width="320", height="240"} | ![](/portfolio/images/clients/crooz/unite-2016-tokyo-2/Unity_Animation_Controller_Creator_Tool.png){: width="320", height="240"} |
|---------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
|                                                                                                               |                                                                                                             |                                                                                                        |                                                                                                                      |

### Prefab Update Tools For Unity 5
Artists working on the fantasy rpg game required a way to update existing Unity prefabs when a model’s geometry or animation changed.  <br/>
To automate this task, I created a Unity prefab update tool that would locate the prefab’s FBX resource and then automatically update the prefab’s model geometry and animation clips. <br/>

| ![](/portfolio/images/clients/crooz/unite-2016-tokyo/Batch_Prefab_Updater_Tool.png){: width="320", height="240"} |
|-----------------------------------------------------------------------------------------------------------------|
|                                                                                                                 |

### Animation Preview Player For Unity 5
Artists required a way to preview and check animated game assets in Unity 5 without entering play mode, because entering play mode was taking too much time.  <br/>
To speed up game model animation review, I created a custom animation player tool that was able to playback animated unity game assets without entering play mode.  <br/>
This allowed artists to perform their animation quality check work more efficiently. <br/>

| ![](/portfolio/images/clients/crooz/unite-2016-tokyo-2/Unity_Animator_Controller_Playback_Tool.png){: width="320", height="240"} |
|---------------------------------------------------------------------------------------------------------------------------------|
|                                                                                                                                 |

### Look-Dev Tools For Unity 5
To help artists efficiently check large volumes of game assets, I created custom preview tools that allowed artists to quickly filter and load game prefab’s, such as characters, equipment and weapons, enemies, backgrounds, magic effects and battle scenes.  <br/>
The character preview tool allowed artists to rapidly switch and preview character parts, such as hair, faces and bodies, as well as different kinds of equipment and weapons.  <br/> 
All preview tools featured the ability to select and preview different animations for animated prefabs.  <br/>
The battle scene preview tool setup a mock battle scene with character’s and enemies placed on a battle field. <br/>

| ![](/portfolio/images/clients/crooz/unite-2016-tokyo-2/ffgm_chara_viewer_tool.jpg){: width="320", height="240"} | ![](/portfolio/images/clients/crooz/unite-2016-tokyo-2/ffgm_enemy_viewer_tool.jpg){: width="320", height="240"} | ![](/portfolio/images/clients/crooz/unite-2016-tokyo-2/ffgm_map_viewer_tool.jpg){: width="320", height="240"} | ![](/portfolio/){: width="320", height="240"} |
|----------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|----------------------------------------------|
|                                                                                                                |                                                                                                                |                                                                                                              |                                              |

### Shader And Post Effects Development For Unity 5
I created all shader and post effects for a fantasy RPG mobile game, such as character skin shaders, as well as bloom and glow post effects. <br/> 
I performed graphics performance analysis and tuning using the Unity profiler tool. <br/> 
After I optimized shader code, I would check the graphics performance on various mobile devices with different GPU specs. <br/>

| ![](/portfolio/images/clients/crooz/unite-2016-tokyo-2/ffgm_shader_chara_skin.jpg){: width="320", height="240"} | ![](/portfolio/images/clients/crooz/unite-2016-tokyo-2/ffgm_shader_fade.jpg){: width="320", height="240"} | ![](/portfolio/images/clients/crooz/unite-2016-tokyo-2/ffgm_shader_crystal.jpg){: width="320", height="240"} |
|-----------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|
|                                                                                                                 |                                                                                                           |                                                                                                              |

### GUI Development Work

Some of my time was spent working on creating and setting up game screen GUI elements using the NGUI UI system. 
NGUI was the most popular UI system for Unity at the time.

### Gameplay Tuning

I assisted with gameplay testing for game projects I was assigned to, including a car racing game. 
Various aspects of the car race were quality checked, such as collision issues, the travel path of the CPU controlled racing car and fairness of the race.
