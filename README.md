

# Shader Redstone 3 MANUAL (2019-11-28)
![enter image description here](https://i.imgur.com/OERAqmX.png)
## Changes from Shader Redstone 2:
* Improved UI (WIP).
* Full 3D world to edit.
* AA and AO effects.
* Instant energy propagation through Redstone dust (like Minecraft, allows for accurate clocks).
* Player movement.
## Notes:
* Currently Buffer A **Can't compile on Windows** because ANGLE's *DirectX 9* (Used by default on Chrome and Firefox on Windows) backend doesn't fully implement *WebGL 2*. It tries to force unroll loops which are impossible to unroll in the pathfinding function.
* Cannot power a stone block using Redstone dust yet.
* This was partly inspired by [Javascript Redstone Simulator](https://mordritch.com/mc_rss/).
* I used RNG code from [Hash Without Sine 2 (WebGL 2)](https://www.shadertoy.com/view/XdGfRR).
* I used a SDF font code for the UI from [Shadertext Proportional Spacing](https://www.shadertoy.com/view/4s3XDn).
## Rules:
* Anything which is bright red is lit and anything which is dark red is unlit.
* Torches are lit by default. 
* Dust is unlit by default.
* Energy from torches spreads through dust (*OR* operator).
* If a stone block is powered, any torch attached to the block will be off (*NOT* operator).
## Default Controls:
* You can move around in the XY plane using WASD by default.
* You can zoom up or down using Q and E by default.
* You can move quicker using LSHIFT.
* You can place blocks using F, and remove using R.
* You can switch selected item using LEFT and RIGHT (arrows).
* You can change Z layer using DOWN and UP (arrows).
## Creating Basic Logic Gates:
### The *OR* gate:

![OR Gate](https://i.imgur.com/Iasfby2.png)
### The *NOT* gate (unary):
![NOT gate](https://i.imgur.com/iyprINi.png)

### The *AND* gate:
Output should be true only when both inputs are true.
![enter image description here](https://i.imgur.com/uU7l3mj.png)
