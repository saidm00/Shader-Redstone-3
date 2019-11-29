# Shader Redstone 3 MANUAL (2019-11-28)
## Changes from Shader Redstone 2:
* Improved UI (WIP).
* Full 3D world to edit.
* AA and AO effects.
* Instant energy propagation through redstone dust (like Minecraft).
* Player movement.
## The basic rules of this system is:
* Anything which is bright red is lit and anything which is dark red is unlit.
* Torches are lit by default. 
 ![Redstone Torch](https://i.imgur.com/QWSDgPO.png)
* Dust is unlit by default.
 ![Redstone Dust](https://i.imgur.com/npKr3zK.png)
* Energy from torches spreads through dust (*OR* operator).
![OR gate](https://i.imgur.com/AmRckyF.png)
* If a stone block is lit, any torch attached to the block will be off (*NOT* operator).
![NOT gate](https://i.imgur.com/IMXgrBW.png)
## Default Controls:
* You can move around in the XY plane using WASD by default.
* You can zoom up or down using Q and E by default.
* You can move quicker using LSHIFT.
* You can place blocks using F, and remove using R.

## Creating Basic Logic Gates:

### The *OR* gate:

![OR Gate](https://i.imgur.com/Iasfby2.png)
### The *NOT* gate (unary):
![NOT gate](https://i.imgur.com/iyprINi.png)

### The *AND* gate:
Output should be true only when both inputs are true.
![enter image description here](https://i.imgur.com/uU7l3mj.png)
