![Reactor Logo](static/img/Reactor_logo.png)

# Reactor Anywhere&trade; v5.0

> Roadmap Draft 1 (2026-09-15)  
> Written by: [Andrew Hazelden](mailto:andrew@andrewhazelden.com)  

What would it look like, if you could have the identical “Reactor Package Manager” user experience but access it purely via a web browser session? After the literal shock, awe, (and honestly sheer horror) that was IBC 2026's BMD product launches: A design concept emerged for the next evolution of the WSL Fusion Community based [Reactor project](https://gitlab.com/WeSuckLess/Reactor).

We will continue to work hard, every day, in our long-term quest to support the ~500K plus active users of [Reactor Classic](https://gitlab.com/WeSuckLess/Reactor) / [Reactor Standalone](https://github.com/Kartaverse/Reactor-Standalone). We will do this today, tomorrow, [the day-after-tomorrow](https://www.youtube.com/watch?v=HUBDFoMNXzA), and beyond, by delivering the "extended" Fusion community made content to the web in new ways. This requires us to keep moving forward to adopt new Reactor application designs, and to roll out ever improving download mechanisms.

Additionally, over the last year and a bit Reactor's core repository management functionality was expanded to be able to work with the latest Resolve/Fusion releases, and to start slowly at serving the broader creative software spaces like Assimilate Scratch and LiveFX, OpenFX, JangaFX, SideFX Houdini, and LightWave.

[![Watch the video](https://img.youtube.com/vi/mklCsf8yOUk/maxresdefault.jpg)](https://www.youtube.com/playlist?list=PLVDcRvd92hcgtYFgiiJtWUWEKJH0Op8W9)
(Click to play the Youtube Video)

## Concept

The working concept today with the new Reactor Anywhere repo, is to build the next generation of web-browser session operated Reactor tools with responsive, slick, well thought out user interfaces that react automatically to the active device you are using to view the Reactor web app.

This app redesign process will allow the end user to entirely skip the need to install a Reactor Standalone desktop application locally on their laptop or workstation. And it further builds on the base 2018 version of Reactor that we all know and love. That original edition is today known colloquially as "Reactor Classic", as it uses a "Reactor.lua" file that requires LuaJIT scripting capability to exist in the host Resolve/Fusion DCC application...

![Resolve Free v21.1 Note](static/img/The-Wizard-Of-Oz-The-Great-Oz-Has-Spoken.jpg)

## Resolve Studio for iPad Compatible

With Reactor Anywhere you will be able to run the Reactor WebUI on an iPad's Safari or Chrome browser. You can download your favorite packaged content. Then the Files app will allow you to install the Atom packaged content that makes sense to use with [Resolve Studio for iPad](https://apps.apple.com/us/app/davinci-resolve-for-ipad/id1581363826). Now, how cool is that?

![Resolve on iPad](static/img/Resolve-on-iPad.jpg)

A special Reactor Anywhere compatible version of the "KickAss Shaderz for iPad" atom package is also being prepared. This will help to bring the classic "[KAS shaders](https://kartaverse.github.io/Reactor-Docs/#/com.wesuckless.KickAssShaderZ?id=kickass-shaderz)" over to tablet based artists. It is something that will be optimized to support the use of the Resolve Studio for iPad's (WIP) Fusion page environment.

# What will the new Reactor WebUI it look like?

With the upcoming Reactor Anywhere release, it will feel a lot like a supercharged, fast, browser based remake of Reactor Standalone's existing UI. Gone are the initial Reactor Standalone beta application's pokey startup times, slow atom package syncing speed, and the extra bit of lag like delays when switching categories and clicking around in the user interface. 

We want Reactor Anywhere to set a newly improved standard of running smooth-as-butter. That is the major goal for the web-hosted experience, as you navigate your way across the full Reactor user interface.

We plan to take the best parts of the Reactor Classic/Reactor Standaline user interface elements, and carry that forward with the help of modern HTML5/Javascript/REST based technology. The working concept is to be able to deliver what is called a "Single-File Web App" to the Reactor end user, as well. This is also known in other circles as a "Standalone HTML" setup.

Here is what the current Reactor Standalone desktop app user interface looks like for reference: 

![Reactor Standalone](static/img/Reactor-Standalone.png)

# What Atom Content Will Reactor Anywhere Support Initially

The new JSON-based Reactor atom package files will allow you to easily install:

Content:
- Macros .setting
- DCTLs .dctl
- LUTS
- Audio
- Movies
- RAW Video Formats
- Images / Image Sequences
- 3D Geometry
- Point Clouds
- Camera Tracking Data
- ST Map Warping Templates
- Roto Shape Data
- Resolve:
	- Projects .dra, .drp
	- Timelines .drt
	- Bins .drb
	- Grades .drx
- Fusion:
	- Composites .comp
	- Custom PathMaps
	- Custom Variable Maps
	- Custom Toolbars
	- Custom Guide Grids .guide
	- Confg Files .fu, .zfu based Menus/Hotkeys/Events/Actions
	- Fusion Render Manager Queues

Mograph:
- Effects Templates .drfx, .setting
- OGraf .json
- Lottie .lottie
- Fonts .ttf, etc…
- JSON .json, .jsonc
- Spreadsheets .csv, .tsv, .xls, etc.

Plugins:
- Fuses .fuse
- FusionSDK C+ .plugin
- OpenFX C++ Plugin Bundle
- Workflow Integrations / Deliver Page Exporters
- VST Audio Plugin .vst

## Why is this Reactor migration to the web even required?

BMD has made it clear at [Resolve v21.1](https://www.blackmagicdesign.com/support/readme/59dd4eef1f4941c29fb8dc48b33f5c8) that 3rd party developers should respect the core tenants of BMD's Freemium business model wishes.

That in effects means that we (the Reactor project) need to immediately and permanently stop trying to use Python scripting, PySide, or even LuaJIT advanced scripting functionality on the Reactor Package Manager's own GUI, as the toolset is actively aimed at the Resolve Free userbase. Just don’t do it.

The WeSuckLess&trade; developers, meaning specifically the two person team behind the Reactor core project, Andrew and SecondMan, want to be good corporate citizens in the BMD community. So in good faith, we are biting-the-bullet and are going to have to tow that line as well in, solidarity with the mothership at BMD SG. Yesh. 🙈🙊🙉
