---
name: Square Enix
subtitle: Advanced Technology Division
start_date: 2021-06-20
end_date: Present
external_url: 'https://www.square-enix.com/'
image_path: /images/clients/square_enix/square_enix_logo_black_thumb.png
---

# ![](/portfolio/images/clients/square_enix/square_enix_logo_black.png){: width="800" height="414"}

# Square Enix

## Employment Overview

From June 2021 up to present, I am working as an **Engineer** in the [Advanced Technology Division](http://www.jp.square-enix.com/tech/#) on the Tools and Workflow team at [Square Enix](https://www.square-enix.com/) in Shinjuku, Tokyo.

&nbsp;

## Facial Animation Technology Project

### Overview

At Square Enix, I have worked on developing Maya tools for an in-house facial animation technology, as well as game engine editor tools for Luminous Engine and Unreal Engine 5.

The game engine editor tools were initially being built for Luminous Engine, but we ended up switching to Unreal Engine 5 later.

### Tool Development

#### Maya Facial Animation Exporter (In-House Tech)

I added several new features to the existing Facial Animation Exporter for Maya, such as the selective export of:
- facial motions
- motion catalogs
- motion libraries
- character rig data.

I updated the tool source code in order to support Python 3 and newer versions of Maya.

For tool documentation, I recommended using [Material for MK Docs](https://squidfunk.github.io/mkdocs-material/) and wrote the tool's user guide in both English and Japanese.

Later, I created a Maya tool for mixing facial motions from different motion catalogs and libraries in order to create custom ones.

##### &nbsp;

#### Facial Animation Tools For Luminous

As a part of a project involving a realtime talking AI 3D avatar,

I created debugging tools for testing facial rig controls on a character model.

I created a panel that displayed a list of the rig controls, which could be filtered in real time by control name, or by the control type.

Each rig control listed either had a single channle (.x) or a triple channel (.x .y .z) slider UI control for testing it.

I also created a tool for testing the playback of facial motions from the exported facial motion libraries.

&nbsp;

#### Facial Animation Tools For Unreal Engine 5

Later in development of the AI avatar project, we decided to switch from Luminous Engine to Unreal Engine.

I ended up porting all of the above mentioned Facial Animation tools from Luminous to Unreal 5.

I also added support for saving and restoring the current user session and all current tool settings, so that the user could pickup where they left off next session.

&nbsp;

## Unreal Engine 5 GPS Mobile Game Project

### Overview

While at Square Enix, I also particpated on the development of a GPS location based mobile game title.

The game features a procedural building generation system, and I was tasked with adding support so that regular pre-made building models could also be displayed in the game.

#### Static Model Loading and Spawning

For this feature, I needed to analyze the procedural building system and the spawn systems, which were bigger and more complex than anticipated.

Then, I needed to add new functions for loading static mesh assets from a list of meshes stored in an Unreal Data Asset file.

I also created a developer setting so that the loading and spawning of buildings could be switched between procedural and static meshes.

Finally to load and spawn static meshes, I put in additional logic and function calls in all the areas where the procedural buildings were generated and spawned.

&nbsp;