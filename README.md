# Debiddos Open Macros


## Dependências
Para uso desse repositório, você precisará:

  * **[Blender 3D](https://www.blender.org) 2.80.75** *ou mais novo* para modelagem e animação com algum **Addon** compatível para manipular, importar e exportar os arquivos necessários. 
  * *[Blender Source Tools](http://steamreview.org/BlenderSourceTools/archives/)* 
  * **studiomdl.exe** da **Source Engine 2013**, para compilar os modelos. Esse está na pasta `bin` do seu Jogo.  
  
  
  
E um mínimo conhecimento sobre:  
 * Source Engine  
 * Quake Code  
 * Blender  
 * Shape Key & Flex Animation  
 * Euler Rotation  
 * Gimbal Rotation  
 * Quaternion Rotation  
 * Rotações & Posições relativas  
  
  
> Ou seja, se você é algum **iniciante**, vai entender praticamente nada do que tem aqui.



## Referências para construção de expressões faciais  

#### Dentro dessa teia:
Video Showcase (Test) | Character (project) | Description (details)
------------ | ------------- | -------------
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [digimon_kyuukimon_v1.5](digimon_kyuukimon_v1.5) | Meu primeiro modelo e mod com sucesso que não era apenas um simples "prop" ou uma gambiarra pura *(ele até tem, mas são poucas)*
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [kr_scarlet](kr_scarlet) | Minha amada Scalet foi meu primeiro projeto a usar com sucesso deversos [$bodygroups](https://developer.valvesoftware.com/wiki/$bodygroup) que muda drasticamente sua aparência, junto de "EyeRefract" de forma aceitável e percebi que contando que um flexcontroller tenha um nome correto, ele vai ser executado pelo runtime se for solicitado por uma sequência. Ao perceber isso, fui ter alguns estudos com o Source code da [Carbon Miku](vocaloid_carbon_miku) do [CaptainBigButt](https://steamcommunity.com/id/CaptainBigButt)
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [digimon_ordinemon](digimon_ordinemon) | Primeiro modelo a usar com sucesso o sistema de FACS, ele serviu de base para criar outros presets e foi evoluindo até ser o que é hoje em [FACS.dmx](mesh/FACS.dmx)
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [digimon_rosemon](digimon_rosemon) | Primeiro modelo a usar com sucesso o Jigglebones que se movem em XYZ ao invés de apenas rotacionar, isso serviu de base para criar os [macros de jigglebones de mesmo nome](includes/macro/jiggle_tiferet.qci)
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [digimon_rie_kishibe](digimon_rie_kishibe) | Primeiro modelo a usar com sucesso **DMXEyelid**, posteriomente fui implementando para os demais.
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [digimon_nokia_shiramine](digimon_nokia_shiramine) | Meu primeiro modelo com proceduralbones complexos e completamente reestruturados, serviram para criar meu esqueleto de referência e inspiração para fazer os procedurals de [sfiv_ibuki](sfiv_ibuki) que é nada mais que uma versão aperfeiçoada da Nokia.
 [![HLMV 2021-08-09](http://img.youtube.com/vi/vC-3qAdi8f8/0.jpg)](https://www.youtube.com/watch?v=vC-3qAdi8f8 "HLMV 2021-08-09") | [honkai_bianka_ataegina](honkai_bianka_ataegina) | O mais ambicioso projeto onde coloquei meus conhecimentos ao limite. Durandal, foi meu experimento e desafio de até quantos $bodygroups eu poderia manter dentro do limite de 255 bones! Também, foi meu *[MMD to FACS](includes/Flex_MMD.qci)* da source e seu preset serviu-me para outras commissions e criar um preset de HWM
  [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [nep_purple_sister](nep_purple_sister) | Meu primeiro HWM *(tecnicamente foi a Scarlet, mas na epoca não sabia)*. Aqui foi onde coloquei o que apreendi com a [Durandal](honkai_bianka_ataegina/includes/Flex_MMD.qci) e coloquei em prática numa commission de forma discreta.
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [xenosaga_kos-mos](xenosaga_kos-mos) | com explicações sobre l4d2 durante meus experimentos em lidar com a proportion trick e custom animations. Ao mesmo tempo que eu tentava manter o menor número de arquivos.an
 [![2021-07-28 23:32:23](http://img.youtube.com/vi/AxhNadt_OmY/0.jpg)](https://www.youtube.com/watch?v=AxhNadt_OmY "2021-07-28 23:32:23") | [rockman_xdive_x](rockman_xdive_x) | Um do primeiros projetos em larga escala a receber multiplas atualizações, foi a partir daqui que eu vi uma obrigação em manter os arquivos de forma satisfatória para serem usados em diversos compiladores diferentes e comportar um menor numero de pastas e arquivos repetidos. Acabando por ser um modelo com mais de 30 bodygroups.
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [Debiddos-Animations](Debiddos-Animations) | Onde você encontra as bases para criar seus mods de Garry's Mod e Left 4 Dead 2.
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [0xdigimon](0xdigimon) | Onde você encontra bases para portar modelos de Digimon LinkZ, CyberSleuth e ReArise para a Source.
 [![IMG_ALT_TEXT](http://img.link.jpg)](https://youtube.link.com "Alt Tittle") | [0xscripts](scripts) | Onde você pode encontrar scripts que em breve serão movidos para [Debiddos-Animations](https://github.com/LoveRenamon/Debiddos-Animations-private).
  
  
  
### Referências para FACs  
Para [Facial Action Coding System](https://wikipedia.org/wiki/Facial_Action_Coding_System)) há [esse site](https://imotions.com/blog/facial-action-coding-system) que serve para construir e usar de referência as expressões faciais ou até mesmo o prórpio Starter Kit do Left 4 Dead 2  

#### ./mesh/FACS.dmx
  Segue o sistema de **[Facial Action Coding System](https://developer.valvesoftware.com/wiki/Flex_animation)** para mapear as expressões facis. Sendo esse o método mais rápido de se fazer expressões facias na Source, e o mais difícil de customizar.  

* **[iMotions](https://imotions.com/blog/facial-action-coding-system)**  
* **[Carnegie Mellon’s School of Computer Science](https://www.cs.cmu.edu/~face/facs.htm)** de **Ekman** and **Friesen** *(1978)*   


### Referências para HWM
Para Hadware Morphs, temos o [HWMToolkit](https://github.com/revzin/HWMToolkit) de revzin, *(apesar de haver meu padrão prórpio, por compatibilidade é recomendado seguir o padrão da Valve)*

#### .mesh/HWM.dmx
  Esse arquivo segue o padrão novo de **[Hardware Morph](https://developer.valvesoftware.com/wiki/SFM/Introduction_To_HWM)** para movimentar partes da malha, isso o deixa mais próximo dos padrões atuais de de animação. É super versátil e permite **[normals](https://en.wikipedia.org/wiki/Normal_mapping)** serem realinhadas, melhor suporte a **[wrinkle maps](https://developer.valvesoftware.com/wiki/Wrinkle_maps)**, e exeistem **[corrective shapes](https://developer.valvesoftware.com/wiki/Flex_animation#Corrective_shapes)** para deformar a malha.  
  Super fácil de customizar, porém exige bastante tempo posicionando cada shape/flex.  


## Referências de Estudo e Inspiração para esse projeto  
[oficial repo da Facepunch](https://github.com/robotboy655/gmod-animations)  
[HWMToolkit](https://github.com/revzin/HWMToolkit)  
[reanims_helpers-l4d2](https://github.com/xDShot/reanims_helpers-l4d2)  
[blender_l4d2_ik_rig](https://github.com/xDShot/blender_l4d2_ik_rig)  
[blender_gmod_ik_rig](https://github.com/xDShot/blender_gmod_ik_rig)  
