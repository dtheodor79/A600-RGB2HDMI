# A600 RGB2HDMI
Another one RGB to HDMI solution for the Amiga 600, based on information found on [c0pperdragon's](https://github.com/c0pperdragon/Amiga-Digital-Video/issues/37) and [hoglet67's](https://github.com/hoglet67/RGBtoHDMI/tree/master/kicad_AmigaAdapter/Small) Github pages.

# Solution
Towards intercepting the original Denise RGB siganls, certain solutions use a PCB with a flexbile cable that connects them to the [RGB adapter](https://github.com/hoglet67/RGBtoHDMI/tree/master/kicad_AmigaAdapter/Small) or a custom PCB with a [cut-off in the middle](https://github.com/c0pperdragon/Amiga-Digital-Video/issues/37). 

This solution somehow "merges" the previous approaches; it is based on a small PCB that is used to intercept RGB signals from the A600 Denise chip and deliver them to the Raspbery Pi zero. On its bottom side, the PCB houses a PLCC-52, and on its top side a set of pins for mouting the [Denise Amiga adapter PCB](https://github.com/hoglet67/RGBtoHDMI/tree/master/kicad_AmigaAdapter/Small) that is available on [hoglet67 Github page](https://github.com/hoglet67). As suggested, the adapter CLK signal is fed from Denise's 7MHz signal.

This is the PCB stack that enables the HDMI output:

![RGB2HDMI stack](/images/concept1.png)

And this is a 3D image from KiCAD:

![RGB2HDMI adapter](/images/a600_rgb2hdmi.png)

Finally, these are a few images that show how I successfully installed it on my A600:








