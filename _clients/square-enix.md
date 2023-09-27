---
name: Square Enix
subtitle: Advanced Technology Division
start_date: 2021-06-01
end_date: Present
external_url: 'https://www.square-enix.com/'
image_path: /images/clients/square_enix/square_enix_logo_black_thumb.png
---

# ![](/portfolio/images/clients/square_enix/square_enix_logo_black.png){: width="800" height="414"}

# Square Enix

## Employment Overview

From June 2021 up to present, I have been working as an **Engineer** in the [Advanced Technology Division](http://www.jp.square-enix.com/tech/#) at [Square Enix](https://www.square-enix.com/) in Shinjuku, Tokyo.

&nbsp;

## Facial Animation Technology Project

### Overview

At Square Enix, I have worked on developing in-house Maya tools as well as game engine editor tools for Luminous Engine and Unreal Engine 5.

### Tool Development

#### Maya Facial Animation Exporter (In-House Tech)

I added several new features to an existing Facial Animation Exporter tool for Maya, such as the selective export of:
- facial motions
- motion catalogs
- motion libraries
- character rig data.

I also upgraded the Python 2 tool source code to Python 3 in order to support newer versions of Maya.

For tool documentation, I used [Material for MK Docs](https://squidfunk.github.io/mkdocs-material/) and wrote the tool's user guide in both English and Japanese.

Later, I created a Maya tool for mixing facial motions from different motion catalogs and libraries in order to create custom ones.

##### &nbsp;

#### Facial Animation Debug Tools For Luminous Engine

As a part of a facial animation project, I created debugging tools for testing character facial rig controls in the Luminous Editor.

I created a panel that displayed a list of the rig controls, which could be text filtered in real time by control name, or by the control type.

The tool featured slider UI for both single and triple channel (.x .y .z) rig controls, allowing the user to test any control movement.

I also created a tool for testing the playback of the facial motions in-editor.

&nbsp;

#### Facial Animation Debug Tools For Unreal Engine 5

Later, it was decided to port the tools from Luminous Engine to Unreal Engine 5.

So, I ended up porting all of the above mentioned facial animation debug tools to Unreal Editor.

I also added support for saving and restoring the current debug settings, so that the user could continue working where they last left off.

&nbsp;

## Unreal Engine 5 GPS Mobile Game Project

### Overview

While at Square Enix, I also participated on the development of a GPS location based mobile game title.

The game features a procedural building generation and spawn system, and I was tasked with upgrading the systems to also work with regular static mesh building models.

#### Static Model Loading and Spawning

For this feature, I needed to study and analyze the procedural building system and the spawn systems, which were bigger and more complex than anticipated.

I was able to make the necessary changes to the source, and adapt the system to work with regular static meshes.

I added a UI toggle to the game settings in order to be able to switch between procedural and static mesh spawning.

I also created an Unreal Data Asset file to load the static mesh buildings from, and set it up with support for different themes / building skins.

&nbsp;