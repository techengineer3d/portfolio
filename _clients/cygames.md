---
name: Cygames
subtitle: Project Awakening
start_date: 2017-09-01
end_date: 2021-02-28
external_url: 'https://www.cygames.co.jp/en/'
image_path: /images/clients/cygames/project-awakening/cygames_project_awakening_thumb.png
---
# ![](/portfolio/images/clients/cygames/cyagames-logo-2.png){: width="800" height="414"}

# Cygames

2017/09 ~ 2021/02 <br/>
Technical Artist <br/>
Technical Artist Department <br/>
Tokyo, Japan <br/>

## Game Titles

| [Project Awakening - Arise](https://projectawakening.com/en/)                                                      | [Anubis Zone of the Enders M∀RS](https://www.konami.com/games/zoe_mars/as/en/)                                                  |
| ------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------- |
| ![](/portfolio/images/clients/cygames/project-awakening/cygames_project_awakening.png){: width="640" height="480"} | ![](/portfolio/images/clients/cygames/zone-of-the-enders-anubis/anubis_zone_of_the_enders_large.jpg){: width="640" height="480"} |
| ---                                                                                                                | ---                                                                                                                              |

## Overview

At [Cygames](https://www.cygames.co.jp/en/), I worked on Unity game development, art pipeline tools for the AAA game title “Project Awakening – Arise”, and also internal tools used by the Technical Artist Team. <br/>

### Extension of Open Source Maya Tool "Studio Library"

[Studio Library](https://www.studiolibrary.com/){: target="_blank"} is a free tool for managing poses and animation in Maya. <br/>
I created a customized version of Studio Library for the character animator artists. <br/>
The artists had been using an internally created pose tool but wanted to switch to Studio Library. <br/>
I created an importer and converter tool to change all the existing old poses to Studio Library poses.  <br/>
This let the artists seamlessly change over to Studio Library and continue their work without interruption. <br/>
For file versioning support, I added [Perforce](https://www.perforce.com/) integration to Studio Library to allow the artists to update, checkout and submit their poses to the Perforce repo directly from Maya. <br/>
Perforce icons were added to all pose thumbnail previews to let artists know the current status of the files. <br/>
Poses in Studio Library are always created at the origin (0,0,0). But sometimes artists need to apply poses to characters in other locations.  <br/>
Support was added to make it possible to apply Studio Library poses to characters at world locations other than the origin. <br/>

### Extension of Open Source Maya Tool "Pyblish"

[Pyblish](https://pyblish.com/){: target="_blank"} is a free tool for checking and verifying that art assets comply with production guidelines, such as naming convention rules. <br/>
The tool can be used in various DCC software, such as Maya. <br/>
I implemented a custom version of Pyblish to help artists check, validate and fix 3D scene object names, such as the main model, LOD models, collision models, rig joints as well as materials and textures. <br/>
I also implemented an object hierarchy check, to make sure objects were properly parented. <br/>
Invalid object names were listed with red text in the Pyblish validation result window. <br/>

### Unreal Engine Game Map Data Export Tool

I wrote a C++ game map data export tool, which exported game model names and world locations to a data file. <br/>
The exported data file was used to import the game map models into a different game engine. <br/>

### Unreal Engine Character Hair Shading

I assisted with shading work the main character’s hair for a AAA Unreal Engine fantasy game project. <br/>
This work included researching methods for improving graphics quality of the hair shader, and also previewing and debugging the hair shader materials on game console. <br/>

### Localization Work

Some of my time was spent performing localization work for the PS4 release of the game Anubis Zone of the Enders - M∀RS, developed by Konami in conjunction with Cygames.
My tasks included proofreading and editing the game's English text, reviewing in-game spoken English dialog and written English text displayed in the game’s UI.
I also helped enter localized game text for the French, German, Italian and Spanish languages using an in-house localization editor tool.

### Technical Artist Team Internal Tool Development

The technical artist team required internal support for tracking tool usage frequency and receiving error reports. <br/>
To track the tool usage frequency, I setup a system for sending tool usage metrics logs to a python web application server, which displayed usage metrics as bar graphs and charts. <br/>
This helped the Technical Artist Team to determine which tools to retire, and which tools to put more development focus on. <br/>
To send tool error reports, I setup an error logging system that would send notifications to Slack and alert the Technical Artist Team of tool errors instantly. <br/>
This helped the Technical Artist Team to respond to tool error incidents more efficiently. <br/>
The tool metrics logging system and error logging system were put together using: <br/>
[Flask AppBuilder](https://flaskappbuilder.pythonanywhere.com/) as the python web app, [CherryPY](https://cherrypy.org/) as the python server, [JINJA2](https://palletsprojects.com/p/jinja/) templates, [SQL Alchemy](https://www.sqlalchemy.org/) and a [Postgres Database](https://www.postgresql.org/).

### Technical Artist Team Developer Operations Improvement

I conducted information research for improving developer source code quality and documentation, and discussed different strategies with the Technical Artist Team.
Some examples: <br/>

#### Source Code Analysis Tools

[Coverity](https://www.blackduck.com/static-analysis-tools-sast/coverity.html), [SonarLint](https://www.sonarlint.org/), [SonarQube](https://www.sonarqube.org/),

#### Coding Style Tools

[Unibeautify](https://unibeautify.com/)

#### Source Code Documentation Tools

Javascript : [Sphinx-JS](https://github.com/mozilla/sphinx-js), [TypeDoc](https://typedoc.org/), Python: [Sphinx](https://www.sphinx-doc.org/en/master/) , [PyCharm Doc Generation](https://www.jetbrains.com/help/pycharm/generating-reference-documentation.html), C/C++: [Doxygen](https://www.doxygen.nl/)

#### Source Code Documentation Integrations for Confluence

[Sphinx For Confluence](https://github.com/sphinx-contrib/confluencebuilder), [Doxygen For Confluence](https://docs.appfusions.com/display/DOXYGEN/Home)
