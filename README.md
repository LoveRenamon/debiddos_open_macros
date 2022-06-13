# Debiddos Open Macros
A bunch of presets and macros writen by [Debiddo](https://github.com/LoveRenamon) to aid my own workflow by create playermodel, custom animations and file replacements

## Dependencies
To use this repository, you will need:

   * **[Blender 3D](https://www.blender.org) 2.80.75** *or newer* for modeling and animation with some compatible **Addon** to manipulate, import and export the necessary files.
   * *[Blender Source Tools](http://steamreview.org/BlenderSourceTools/archives/)*
   * **studiomdl.exe** from **Source Engine 2013**, to compile the models. This is in your Game's `bin` folder.


A minimum knowledge of:
  * Source Engine
  * Quake Code
  * Blender
  * Shape Key & Flex Animation
  * Euler Rotation
  * Gimbal Rotation
  * Quaternion Rotation
  * Rotations & Location Relative/Absolute Positions


> That is, if you are a **beginner**, you will basically don't understand what is here



## References for Loverenamon/Source

#### Inside this web messy repo:
Video Showcase (Test) | Character (project) | Description (details)
------------ | ------------- | -------------
[![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [digimon_kyuukimon_v1.5](digimon_kyuukimon_v1.5) | My first successful model and mod that wasn't just a simple "prop" or a pure hack *(he has, but there are few)*
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [kr_scarlet](kr_scarlet) | My beloved Scalet was my first project to successfully use various [$bodygroups](https://developer.valvesoftware.com/wiki/$bodygroup) which drastically change its appearance, along with "EyeRefract" in an acceptable way and I found that counting a flexcontroller has a correct name, it will be executed by the runtime if requested for a string. When I realized this, I went to have some studies with the Source code of [Carbon Miku](vocaloid_carbon_miku) from [CaptainBigButt](https://steamcommunity.com/id/CaptainBigButt)
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [digimon_ordinemon](digimon_ordinemon) | The first model to successfully use the FACS system, it served as the basis for creating other presets and evolved into what it is today in [FACS.dmx](mesh/FACS.dmx)
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [digimon_rosemon](digimon_rosemon) | First model to successfully use Jigglebones that move in XYZ instead of just rotating, this served as the basis for creating the [jigglebones macros of the same name](includes/macro/jiggle_tiferet.qci)
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [digimon_rie_kishibe](digimon_rie_kishibe) | First model to successfully use **DMXEyelid**, later I was implementing it for the others.
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [digimon_nokia_shiramine](digimon_nokia_shiramine) | My first model with complex and completely restructured proceduralbones served to create my reference skeleton and inspiration to make the [sfiv_ibuki](sfiv_ibuki) procedurals which is nothing more than an improved version of Nokia.
 [![HLMV 2021-08-09](http://img.youtube.com/vi/vC-3qAdi8f8/0.jpg)](https://www.youtube.com/watch?v=vC-3qAdi8f8 "HLMV 2021-08-09") | [honkai_bianka_ataegina](honkai_bianka_ataegina) | The most ambitious project where I put my knowledge to the limit. Durandal, it was my experiment and challenge of how many $bodygroups I could keep within the limit of 255 bones! Also, it was my *[MMD to FACS](includes/Flex_MMD.qci)* from source and its preset served me for other commissions and to create a HWM preset
  [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [nep_purple_sister](nep_purple_sister) | My first HWM *(technically it was Scarlet, but at the time I didn't know)*. This is where I put what I learned from [Durandal](honkai_bianka_ataegina/includes/Flex_MMD.qci) and put it into practice in a discreet commission.
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [xenosaga_kos-mos](xenosaga_kos-mos) | with explanations about l4d2 during my experiments dealing with proportion trick and custom animations. At the same time I tried to keep the least number of .an files
 [![2021-07-28 23:32:23](http://img.youtube.com/vi/AxhNadt_OmY/0.jpg)](https://www.youtube.com/watch?v=AxhNadt_OmY "2021-07-28 23:32:23") | [rockman_xdive_x](rockman_xdive_x) | One of the first large-scale projects to receive multiple updates, it was from here that I saw an obligation to maintain the files satisfactorily to be used in several different compilers and to support a smaller number of folders and repeated files. Ending up being a model with more than 30 bodygroups.
 [![IMG_ALT_TEXT](http://img.youtube.com/vi/natSBxzEDro/0.jpg)](https://www.youtube.com/watch?v=natSBxzEDro "Hudiemon dynamic envmap and emission (test)") | [digimon_hudiemon](digimon_hudiemon) | Thanks to [Cuba](https://steamcommunity.com/id/TheRealMeatyMate) providing me with some examples of the [Proxy Pupil](https://developer.valvesoftware.com/wiki/List_Of_Material_Proxies#Texture_manipulation) was the first model to have their materials vary according to the lighting.
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [Debiddos-Animations](Debiddos-Animations) | Where do you find the foundation to create your mods for Garry's Mod and Left 4 Dead 2.
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [0xdigimon](0xdigimon) | Where you find bases to port models from Digimon LinkZ, CyberSleuth and ReArise to Source.
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [0xscripts](scripts) | Where you can find scripts that will soon be moved to [Debiddos-Animations](https://github.com/LoveRenamon/Debiddos-Animations-private).



### FACs References  
  For [Facial Action Coding System](https://wikipedia.org/wiki/Facial_Action_Coding_System)) there is [this site](https://imotions.com/blog/facial-action-coding-system) that serves to build and reference facial expressions or even the Left 4 Dead 2 Starter Kit  

#### ./mesh/FACS.dmx
  It follows the **[Facial Action Coding System](https://developer.valvesoftware.com/wiki/Flex_animation)** system to map the facial expressions. This being the fastest method of making facial expressions on Source, and the hardest to customize.

* **[iMotions](https://imotions.com/blog/facial-action-coding-system)**  
* **[Carnegie Mellon’s School of Computer Science](https://www.cs.cmu.edu/~face/facs.htm)** from **Ekman** and **Friesen** *(1978)*   


### HWM References  
For Hardware Morphs, we have revzin's [HWMToolkit](https://github.com/revzin/HWMToolkit), *(although there is my own standard, for compatibility, it is recommended to follow the Valve standards)*

#### .mesh/HWM.dmx
  This file follows the new **[Hardware Morph](https://developer.valvesoftware.com/wiki/SFM/Introduction_To_HWM)** defaults for mesh flexing parts, it brings it closer to current animation standards. It's super versatile and allows **[normals](https://en.wikipedia.org/wiki/Normal_mapping)** to be realigned, there is support for **[wrinkle maps](https://developer.valvesoftware.com/wiki/Wrinkle_maps)**, and there are **[corrective shapes](https://developer.valvesoftware.com/wiki/Flex_animation#Corrective_shapes)** to deform the mesh in quadratic, cubic or even more curves.
 Super easy to customize, but it takes a lot of time to position each shape/flex.


## References for this project
[Facepunch's official gmod repo](https://github.com/robotboy655/gmod-animations)  
[HWMToolkit](https://github.com/revzin/HWMToolkit)  
[reanims_helpers-l4d2](https://github.com/xDShot/reanims_helpers-l4d2)  
[blender_l4d2_ik_rig](https://github.com/xDShot/blender_l4d2_ik_rig)  
[blender_gmod_ik_rig](https://github.com/xDShot/blender_gmod_ik_rig)  
