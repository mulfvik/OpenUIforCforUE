[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://github.com/mulfvik/OpenUIforCforUE/blob/main/LICENSE)

# Open UI for Cesium for Unreal Engine

## What is OpenUIforCforUE?
OpenUIforCforUE is an open source, blueprint based, UI for use together with the plugin [Cesium for Unreal](https://github.com/CesiumGS/cesium-unreal).
It is created to make the Cesium for Unreal plugin even more readily available with a UI for the main functionality. Goal is to have an UI where layers and so on is configurable and can be saved in game.
The design is "webmap" inspired.

## Features (more is to come, see ["Issues"](https://github.com/mulfvik/OpenUIforCforUE/issues))

 * Settings - Fog and Time/Month
   ![ui_cesium_unreal2](https://github.com/mulfvik/OpenUIforCforUE/assets/24228538/aeb192fe-e7e6-4c6e-9341-12350d4b7743)
 * Layers - Show/Hide and Fly To
   ![ui_cesium_unreal3](https://github.com/mulfvik/OpenUIforCforUE/assets/24228538/3ae3f832-1531-4aa4-a793-1fd9eb258d3e)
 * Metadata infowindow
   ![ui_cesium_unreal1](https://github.com/mulfvik/OpenUIforCforUE/assets/24228538/5dbcdf01-194c-47cc-8f31-a52f2ac501b6)
 * Take high resolution screenshots is available

## How to get started
Follow Cesium for Unreal Quickstart [tutorial](https://cesium.com/learn/unreal/unreal-quickstart/).

Download proper [release](https://github.com/mulfvik/OpenUIforCforUE/releases/) for your project versions of UE and Cesium for UE and put in your projects plugins folder. If there is no such folder create it in project root. Restart project and check so that OpenUIforCforUE plugin is activated. In project settings under Maps and Modes configure as follows:
 * Default Game Mode choose BP_GameMode
 * Default Pawn Class choose DynamicPawn
 * Player Controller Class choose BP_PlayerController

Add Exponential height fog to the level, you find it under Visual Effects.\
Set an accurate sun ["Follow tutorial"](https://cesium.com/learn/unreal/unreal-geospatially-accurate-sun/).\
For each tileset you need to add the Cesium Globe Anchor component to it and make it "movable" for the fly to functionality. ["Read more"](https://cesium.com/learn/unreal/unreal-flyto/#step-5-fly-to-geo-markers).\
It is possible to render a image in the metadata infowindow if the 3D Tileset has an attribute named "image_url" with a stored url to an image eg. https://img.com?q=my-image.png.

## Want to contribute?
Contributions are more than welcome. Start with adding an ["Issue"](https://github.com/mulfvik/OpenUIforCforUE/issues) and reference it in your pull request.

## Found an issue?
For all bugs and feature requests please use ["Issues"](https://github.com/mulfvik/OpenUIforCforUE/issues).
