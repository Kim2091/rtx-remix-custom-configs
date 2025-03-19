# Kim2091's Custom RTX Remix Configs

These presets should allow lower end 20 and 30 series GPUs to play Remix games reasonably well, without giving up Transformer RR or lowering DLSS too far in general

To use these, simply:
1. Download the latest [release](https://github.com/Kim2091/rtx-remix-custom-configs/releases)
2. Navigate to the game folder
  - If you're following this for HL2 RTX: In Steam, right click HL2 RTX, Browse Files
3. Open the `rtx.conf` file that you wish to modify
4. Open the conf file in the zip that you want to apply
5. Copy the contents into the game's `rtx.conf`
6. Press Save

Presets:
"Low" - prioritizes visuals while improving performance. Uses Transformer Ray Reconstruction (RR)

"Ultra Low" - gives up a bit more in visual quality to improve performance further. Uses Transformer RR

"Potato" - is for the absolute lowest end hardware, but still tries to maintain a clear image using Transformer RR

"PurePotato" - is for straight up potato hardware that needs as much performance as it can get. This one sacrifices all extra visuals, excluding path tracing itself. Things like volumetrics, bloom, DLSS Transformer Ray Reconstruction, etc. are thrown away

"HL2_RTX_Darker" - For HL2 RTX Only. Changes the tonemapper and eye adaptation settings to be a bit darker, more like the original game 

-------------

Tips:

- If you need a bit more performance on 20 and 30 series GPUs, open the Alt+X Menu, and change Transformer to CNN. This will harm visuals quite a lot, but will boost performance quite a bit.

- You can use [OptiScaler](https://github.com/cdozdil/OptiScaler) on AMD GPUs to switch out DLSS for FSR 3. 
  - If you do this, you have to put this line in the final rtx.conf: `rtx.enableRayReconstruction = False`
