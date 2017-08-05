---
title: "Analyzed"
menu:
    main:
        name: "analyzed"
        parent: "apps"
        pre: "fa fa-angle-right"
date: 2014-05-04T00:00:00+02:00
---

Analyzed is a simple plugin for Windows Media Player written to be compact and minimalistic.
It is a upgrade to the old Barr plugin which is not supported anymore.

It was tested and is working on Windows Media Player 10, 11 and 12 (both 32-bit and 64-bit versions).
It should work on older versions of the player but you might encounter problems like error messages appearing
after you try to close Windows Media Player so I suggest that you [upgrade](http://windows.microsoft.com/en-us/windows/download-windows-media-player) to one of the tested versions if you haven’t already.

# Download

[Download Analyzed version 0.6.0](/downloads/Analyzed.exe) and start the installation application. The installer should automaticaly detect
the folder in which Windows Media Player is installed and install the plugin into that folder. You should now see a
new entry called Analyzed when you right click on the Visualization area in Windows Media Player.

# Screenshots

{{< figure src="/screenshots/Analyzed1.jpg" >}}
{{< figure src="/screenshots/Analyzed2.jpg" >}}

Two screenshots showing Analyzed in action. The first visualzation used in the screenshots is simply called Bars while the second one is Digital Bars.

# Advanced

For most people the default settings will be just fine, but if you want, you can customize some parts of the
visualization. To open the **Analyzed** options property sheet open the **Tools** menu and select **Options…**. Now click on
the **Plugins** tab and select **Analyzed** in the visualization list. To see the property sheet click on **Properties**. A
window should apear on which you can select the desired resolution of the visualization, color preset and special effects.

Resolutions:

- **256×192**
- **384×288**
- **512×384** – Recommended
- **1024×768**

The higher the visualiazion resolution the more video memory and time it takes to render the visualziation but the sharper the final image.

Color presets:

- **Blue** – Default
- **Red**
- **Green**
- **Custom** – Selected if custom color values are used in the registry keys

To use custome colors you need to know how to edit the registry using RegEdit or any other registry editing tool.
Open the key *HKEY_CURRENT_USER\Software\Miha Software\Analyzed Visualization.* Here you will find the folowing color related values:

- **ColorBackground** – Represents the color of the background (will ony be used if the Blur effect is disabled)
- **ColorTop** – Represents the color of the top left bar
- **ColorTopEnd** – Represents the color of the top right bar
- **ColorBottom** – Represents the color of the bottom left bar
- **ColorBottomEnd** – Represents the color of the bottom right bar
- **ColorPeak** – Represents the color of the peaks

Color values are in standard hex format. Groups of two digits from left to right represent the folowing 8-bit values: **Alpha**, **Red**, **Green**, **Blue**.