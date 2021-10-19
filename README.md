# Debiddos Open Macros
Esse repo é parte da build de animações feitos no blender para Source Engine, especificamente, para Garry's Mod em 9-Way em criaturas não humanóides com multiplos braços, pernas, cabeças, ou sem membros *(como lâmias, nagas, sereias, monstruosidades em geral)*
Seu propoósito é servir de uma atualização na automação para criar modelos e animações customizadas

> Por quê?
> Ora, para permitir um método além do tradicional Proportion-Trick do CaptainBigButt onde as kinemáticas invertidas (IK) ficam quebradas facilmente em de personagens com proporções muito pequenas ou digitigrades.
Isso serve de de alternativa para fazer PlayerModels, Survivors e NPCs com maior diversidade de movimentos de forma não tão destrutiva com outros Addons.



## Wiki
Para facil manuseio, temos a [Wiki](https://github.com/LoveRenamon/Debiddos-Animations-private/wiki) explicando melhor as aplicações e uso desse repositório



## Dependências
Para uso desse repositório, você precisará:

**[Blender 3D](https://www.blender.org) 2.80.75** *ou mais novo* para modelagem e animação com algum **Addon** compatível para manipular, importar e exportar os arquivos necessários. *Recomendo [Blender Source Tools](http://steamreview.org/BlenderSourceTools/archives/)* pois funciona no Linux sem muitos problemas e tem suporte à ***Source 2***  

Adicionalmente **studiomdl.exe** da **Source Engine 2013**, para compilar os modelos. Esse está na pasta `bin` do seu Jogo.  

Se não sabe ao certo como usar essas ferramentas ou alguma que substitua, recomendo procurar apreender o básico através da [wiki](https://github.com/LoveRenamon/Debiddos-Animations-private/wiki).  



## Referências para construção de expressões faciais  

#### Dentro dessa teia:
  - [digimon_kyuukimon_v1.5](digimon_kyuukimon_v1.5) Meu primeiro modelo e mod com sucesso que não era apenas um simples "prop" ou uma gambiarra pura *(ele até tem, mas são poucas)*
  - [kr_scarlet](kr_scarlet) Minha amada Scalet foi meu primeiro projeto a usar com sucesso deversos [$bodygroups](https://developer.valvesoftware.com/wiki/$bodygroup) que muda drasticamente sua aparência, junto de "EyeRefract" de forma aceitável e percebi que contando que um flexcontroller tenha um nome correto, ele vai ser executado pelo runtime se for solicitado por uma sequência. Ao perceber isso, fui ter alguns estudos com o Source code da [Carbon Miku](vocaloid_carbon_miku) do [CaptainBigButt](https://steamcommunity.com/id/CaptainBigButt)
  - [digimon_ordinemon](digimon_ordinemon) Primeiro modelo a usar com sucesso o sistema de FACS, ele serviu de base para criar outros presets e foi evoluindo até ser o que é hoje em [FACS.dmx](mesh/FACS.dmx)
  - [digimon_rosemon](digimon_rosemon) Primeiro modelo a usar com sucesso o Jigglebones que se movem em XYZ ao invés de apenas rotacionar, isso serviu de base para criar os [macros de jigglebones de mesmo nome](includes/macro/jiggle_tiferet.qci)
  - [digimon_rie_kishibe](digimon_rie_kishibe) Primeiro modelo a usar com sucesso **DMXEyelid**, posteriomente fui implementando para os demais.
  - [digimon_nokia_shiramine](digimon_nokia_shiramine) Meu primeiro modelo com proceduralbones complexos e completamente reestruturados, serviram para criar meu esqueleto de referência e inspiração para fazer os procedurals de [sfiv_ibuki](sfiv_ibuki) que é nada mais que uma versão aperfeiçoada da Nokia.
  - [honkai_bianka_ataegina](honkai_bianka_ataegina) O mais ambicioso projeto onde coloquei meus conhecimentos ao limite. Durandal, foi meu experimento e desafio de até quantos $bodygroups eu poderia manter dentro do limite de 255 bones! Também, foi meu *[MMD to FACS](includes/Flex_MMD.qci)* da source e seu preset serviu-me para outras commissions e criar um preset de HWM
  - [nep_purple_sister](nep_purple_sister) Meu primeiro HWM *(tecnicamente foi a Scarlet, mas na epoca não sabia)*. Aqui foi onde coloquei o que apreendi com a [Durandal](honkai_bianka_ataegina/includes/Flex_MMD.qci) e coloquei em prática numa commission de forma discreta.
  - [xenosaga_kos-mos](xenosaga_kos-mos) com explicações sobre l4d2 durante meus experimentos em lidar com a proportion trick e custom animations. Ao mesmo tempo que eu tentava manter o menor número de arquivos.
  - [Debiddos-Animations](Debiddos-Animations) Onde você encontra as bases para criar seus mods de Garry's Mod e Left 4 Dead 2.
  - [0xdigimon](0xdigimon) Onde você encontra bases para portar modelos de Digimon LinkZ, CyberSleuth e ReArise para a Source.
  - [0xscripts](scripts) Onde você pode encontrar scripts que em breve serão movidos para [Debiddos-Animations](https://github.com/LoveRenamon/Debiddos-Animations-private).


### Referências para FACs  
Para [Facial Action Coding System (imotions)](https://imotions.com/blog/facial-action-coding-system) há esse site que serve para construir e usar de referência as expressões faciais ou até mesmo o prórpio Starter Kit do Left 4 Dead 2  

#### ./mesh/FACS.dmx
  Segue o sistema de **[Facial Action Coding System]()** para mapear as expressões facis. esse é o método mais rápido de se fazer expressões facias na Source, e o mais difícil de customizar.  

* **[iMotions](https://imotions.com/blog/facial-action-coding-system)**  
* **[Carnegie Mellon’s School of Computer Science](https://www.cs.cmu.edu/~face/facs.htm)** de **Ekman** and **Friesen** *(1978)*   


### Referências para HWM
Para Hadware Morphs, temos o [HWMToolkit](https://github.com/revzin/HWMToolkit) de revzin, *(apesar de haver meu padrão prórpio, por compatibilidade é recomendado seguir o padrão da Valve)*

#### .mesh/HWM.dmx
  Esse arquivo segue o padrão novo de **[Hardware Morph]()** para movimentar partes da malha, isso o deixa mais próximo dos padrões atuais de de animação. É super versátil e permite **[normals]()** serem realinhadas, melhor suporte a **[wrinkle maps]()**, **[corrective shapes]()**.  
  Super fácil de customizar, porém exige bastante tempo posicionando cada shape/flex.  


## Referências de Estudo e Inspiração para esse projeto  
[oficial repo da Facepunch](https://github.com/robotboy655/gmod-animations)  
[HWMToolkit](https://github.com/revzin/HWMToolkit)  
[reanims_helpers-l4d2](https://github.com/xDShot/reanims_helpers-l4d2)  
[blender_l4d2_ik_rig](https://github.com/xDShot/blender_l4d2_ik_rig)  
[blender_gmod_ik_rig](https://github.com/xDShot/blender_gmod_ik_rig)  
