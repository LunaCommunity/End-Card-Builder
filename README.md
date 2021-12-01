# Interactive End Card Builder
## Overview

The Interactive End Card Builder is a tool developed by Luna for the Playable plug-in. Game developers can create and customize end cards for their playables instantly in the Unity editor.

## Getting Started
1.  [Install Luna Playable](https://docs.lunalabs.io/docs/playable/code/interactive-end-card-builder)  into your Unity project.

2.  Download and import the Interactive End Card Builder into your Unity project.

You can now see the  **Interactive End Card Builder**  folder in your Unity assets. If you want to test the builder, or have a play around with it, you can select the  _Scenes_  folder and open the the  _Example Scene_.

The  `CanvasWithEndCard`  prefab can be dragged and dropped into your project hierarchy and integrated with your work. You can find it in the End Card folder, in the prefabs sub-folder.
## End Card Call

It is necessary to call the end card in order for it to appear in the scene. Therefore, you can use the  `OpenEndCard()`  method in your script to instantiate the end card.

An example is available in the  _scripts_  folder:  **Example End Card Call**

## Configuration
To configurate your end card drag & drop the `CanvasWithEndCard` prefab in your project, select the `LunaEndCardContainer` child, and open the inspector.
### End Card Settings
Use this settings to modify the basic features of your end card.
| Field | Description |
|--|--|
| **Always show EndCard** | Mainly used for testing. Tick this option to make your end card to stay fixed in play mode. |
|Background Texture|You may upload a custom image to use for the end card. If your image includes text already on it be sure to set the End Card text color to transparent.|
|Background Color|The background colour and opacity of the end card. If you do not need a background you can set the alpha value to  **0**.|
|Icon Texture|The image used for the icon in the end card.|
|Icon Color|The background colour and opacity of the end card icon.|
|Button Texture|The image used for the icon in the end card.|
|Button Color|The background colour and opacity of the end card button.|

### End Card Orientation Settings
These settings are also divided between  **Portrait Settings**  and  **Landscape Settings**  according to what orientation is being used. These settings work in the same way, they are only split in two groups in order to get different behaviors according to the considered orientation.

With these field you can modify the size and the position of you playable description by using these fields:
| Field | Description |
|--|--|
| Description Font Size | The size of the description text, the larger the value entered the larger the text will be. |
| Center Description X | Tick this box to **center** the description text along the X axis.|
| Center Description Y |Tick this box to **center** the description text along the Y axis. |
| Description Position X |Use the slider to translate the description text along the X axis. |
| Description Position Y |Use the slider to translate the description text along the Y axis. |

Similar fileds are available for the CTA Button and the Icon:

**CTA Button:**
|Field|Description|
|--|--|
| CTA Font Size | The size of the CTA button text, the larger the value entered the larger the text will be. |
| Center Button X | Tick this box to **center** the button along the X axis.|
| Center Button Y |Tick this box to **center** the button along the Y axis. |
| Button Position X |Use the slider to translate the CTA button along the X axis. |
| Button Position Y |Use the slider to translate the CTA button along the Y axis. |

**Icon:**
|Field|Description|
|--|--|
|Icon Size|Move the slider to change the size the icon.|
| Center Icon X | Tick this box to **center** the Icon along the X axis.|
| Center Icon Y |Tick this box to **center** the Icon along the Y axis. |
| Icon Position X |Use the slider to translate the Icon along the X axis. |
| Icon Position Y |Use the slider to translate the Icon along the Y axis. |
|Round Edged On Icon| Tick this box to round the edges of your icon.|

### Clickable options
In this field, you can specify which part of the end card will be clickable and linked to the app store. You can select:
* **CTA Button only**: only the CTA button will be clickable in the end card.
* **Fullscreen**: the entire screen will be clickable.
* **Fire App Store Click On Show**: this options will automatically click on the end card when it is shown for the first time.

### Animation Settings
The end card can perform different animations once it appears based on your selections.

These animations are available for both Portait and Landscape mode:
* **Slide Top To Bottom**
* **Slide Bottom To Top**
* **Scale**

There are also button animations available:
* **Wobble**
* **Scale**
* **Opacity**

If you need more info about our End Card builder you can check our [documentation](https://docs.lunalabs.io/docs/playable/code/interactive-end-card-builder).
