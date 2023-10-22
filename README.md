[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://github.com/mulfvik/OpenUIforCforUE/blob/main/LICENSE)

# OpenUIforCforUE

Open UI for Cesium for Unreal Engine

## What is OpenUIforCforUE?

OpenUIforCforUE is a open source, blueprint based, UI for use together with the [Unreal Engines](https://github.com/EpicGames/UnrealEngine) plugin [Cesium for Unreal](https://github.com/CesiumGS/cesium-unreal).

## Features (more is to come)

 * Settings - Fog and Time/Month
 * Layers - Show/Hide and Fly To
 * Metadata infowindow
 * Screenshot

## How to get started

Follow Cesium for Unreal Quickstart [tutorial](https://cesium.com/learn/unreal/unreal-quickstart/).

Download the latest [release](https://github.com/mulfvik/OpenUIforCforUE/releases/) and put in your projects plugins folder. Restart project and check so that OpenUIforCforUE plugin is activated. In project settings under Maps and Modes configure as follows:
 * Default Game Mode choose BP_GameMode
 * Default Pawn Class choose DynamicPawn
 * Player Controller Class choose BP_PlayerController

Add Exponential height fog to the level, you find it under Visual Effects.
For each 3D Tiles Tileset you need to add the Cesium Globe Anchor component to it and make it "movable". ["Read more"](https://cesium.com/learn/unreal/unreal-flyto/#step-5-fly-to-geo-markers).
It is possible to render a image in the metadata infowindow if the 3D Tileset has an attribute named "image_url" with a stored url to an image eg. https://img.com?q=my-image.png.

## Want to contribute?
Contributions are more than welcome. Start with an ["Issue"](https://github.com/mulfvik/OpenUIforCforUE/issues) and reference it in your pull request.

## Found an issue?
For all bugs and feature requests please use ["Issues"](https://github.com/mulfvik/OpenUIforCforUE/issues).
