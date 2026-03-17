![marquee example01](piemarquee01.jpg)
![marquee example02](piemarquee02.gif)
*Cabinet by Justin Fite*

# PieMarquee2 (Based on original script)
Enhanced Marquee plugin for RetroPie, Non-Rpi

Original code by RiNa from raspigamer forum (https://cafe.naver.com/raspigamer/)   
https://github.com/rinalim/PieMarquee2
All the credits goes to RiNa.
## Install
```
cd /home/pi
git clone --depth 1 --branch playbox-nonpi https://github.com/2play/PieMarquee2.git
cd PieMarquee2
chmod 755 ./install.sh
./install.sh
```
If you use different display as second monitor, You may need to change framebuffer resolution.  
Add this line to /opt/retropie/configs/all/autostart.sh  
`fbset -fb /dev/fb0 -g 1280 720 1280 720 16`

## PieMarquee2 integrated EmulationStation
You can use PieMarquee2 in ES gamelist screen
```
cd /home/pi/PieMarquee2
chmod 755 ./install-pi4es.sh
./install-pi4es.sh
```
**NOTE :** Pi4 only. It will overwrite original ES

**What you need for Marquee** 

  * Default marquee file is "**maintitle.png**" in "`/home/pi/PieMarquee2/marquee/system/`" folder  
  
  * You can set default marquee as video.  
    Copy video file "**maintitle.mp4**" to "`/home/pi/PieMarquee2/marquee/system/`" folder (*optional*)
    
  * Marquee image for each game should be in "`/home/pi/PieMarquee2/marquee/[system name]/[gamefilename.png]`"   
    **Note**: fba, mame-advance, mame-libretro and mame-mame4all will share the system folder name as `arcade`  
    (eg: for galaga in fba folder - /home/pi/PieMarquee2/marquee/arcade/galaga.png  
         for mario.zip in nes folder - /home/pi/PieMarquee2/marquee/nes/mario.png )
         
  * If there is no game marquee file then PieMarquee2 will show system marquee.  
    Place for system marquee "**systemname.png**" is "`/home/pi/PieMarquee2/marquee/system/`" folder  
    (eg: **snes** for super nintendo, **megadrive** for genesis and megadrive )
    
  * Video boot intro can be set. Copy video file "**intro.mp4**" to "`/home/pi/PieMarquee2/`" folder (*optional*)
  
  * instruction panel image for each game "**gamefilename.png**" goes to "`/home/pi/PieMarquee2/marquee/instruction`" folder (*optional*)
  * publisher image for publisher "**publishername.png**" goes to "`/home/pi/PieMarquee2/marquee/publisher`" folder (*optional, defined in gamelist_short.xml* )  
    **NOTE :** Setting instruction or publisher images makes PieMarquee2 to show marquee of game, instruction and publisher sequentially.)
