![marquee example00](piemarquee00.jpg)

# PieMarquee2
Enhanced Marquee plugin for RetroPie, Rpi4  

original code by RiNa of raspigamer forum (https://cafe.naver.com/raspigamer/)   
https://github.com/rinalim/PieMarquee2

## Install
```
cd /home/pi
git clone https://github.com/losernator/PieMarquee2.git
cd PieMarquee2
chmod 755 ./install.sh
./install.sh
```
You may need to change framebuffer resolution. add this line in /opt/retropie/configs/all/autostart.sh
fbset -fb /dev/fb0 -g 1280 720 1280 720 16

**What you need for Marquee** 

  * Image file for default marquee "maintitle.png" in "/home/pi/PieMarquee2/marquee/system/" folder
  * Syetem image for each system "systemname.png" in "/home/pi/PieMarquee2/marquee/system/" folder (same as rom folder eg: snes for super nintendo, megadrive for genesis)
  * Marquee image for each game as "/home/pi/PieMarquee2/marquee/[system name]/[gamefilename.png]"   
    Note: fba, mame-advance, mame-libretro, mame-mame4all will share the folder as arcade  
    (eg: for galaga, fbneo core - /home/pi/PieMarquee2/marquee/arcade/galaga.png  
        for mario.zip, nintendo - /home/pi/PieMarquee2/marquee/nes/mario.png  )
  * Intro Video file "intro.mp4" in "/home/pi/PieMarquee2/" folder (*optional*)
  * Video file for default marquee "maintitle.mp4" in "/home/pi/PieMarquee2/marquee/system/" folder (*optional*)
  * Instruction panel image for each game "gamefilename.png" in "/home/pi/PieMarquee2/marquee/instruction" folder (*optional*)
  * publisher image for publisher "publisher.png" in "/home/pi/PieMarquee2/marquee/publisher" folder (*optional, defined in gamelist_short.xml* )
  
