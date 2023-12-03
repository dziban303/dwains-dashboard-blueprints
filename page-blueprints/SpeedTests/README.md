# Speedtest Blueprint

This Blueprint is a blueprint version of Speetest page created by [eelcob](https://github.com/dwainscheeren/dwains-dashboard-addons/tree/for-dd-2.0/more_page/speedtest/).

## Installation of this Blueprint
- Install mini-graph-card from [HACS]

- Install Speedtest plugin in homeassistant (https://www.home-assistant.io/integrations/speedtestdotnet)

- Copy the content of the blueprint file `blueprint.yaml` into the Blueprint YAML code.

 ## Fields to define.
 None, the inputs were broken and caused the blueprint not to work. Set time period in the yaml, currently set to 168 hours (one week). Chart colors and their values can be changed in the yaml (see [Changelog\#1.1.3](https://github.com/dziban303/dwains-dashboard-blueprints/blob/main/page-blueprints/SpeedTests/README.md#113)).

### Screenshots
**Light theme:**<br>

No idea, didn't test it.

**Dark theme:**<br>

![image](https://github.com/dziban303/dwains-dashboard-blueprints/assets/7931765/ea551481-0c09-4c89-ba50-a560245457a7)

### Changelog
#### 1.0
- First release
#### 1.1 
- Stolen by dziban
#### 1.1.1
- Removed broken input selection for download/upload names, and time period. Now hardcoded to 168 hours (one week). Easily changeable in the blueprint. Thinned lines somewhat.
#### 1.1.2
- Changed chart heighths. Way too short originally for viewing on a monitor.
#### 1.1.3
- Fixed colors, from red (bad, 0Mbps, 200ms) through yellow, green, and blue (good, 1000Mbps, 0 ms). Values can be easily changed. Perhaps simplest is to set the maximum value to match your ISP max throughput, and delete other values (*not* colors) except for 0, which will automatically create a gradient. Or do whatever, it's fun.
