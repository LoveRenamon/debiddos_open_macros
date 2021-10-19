# Debiddos-Animations
Esse repo é sobre build de animações feitos no blender para Source Engine, especificamente, para Garry's Mod em 9-Way em criaturas não humanóides com multiplos braços, pernas, cabeças, ou sem membros *(como lâmias, nagas, sereias, monstruosidades em geral)*
Aos poucos, uma biblioteca de animações que seja compatível com o `Blender` e para fácil porte de animações customizadas que não diretamente dependam das originais do jogo.
Também, de forma mais simples e direta sobre como cada uma delas funcionam.
Para mais detalhes, cheque os arquivos individualmene e a secção "Wiki" onde os arquivos são melhores documentados

> Porque*?*
> Ora, para permitir um método além do tradicional Proportion-Trick do CaptainBigButt onde as kinemáticas *(IK)* ficam quebradas facilmente para animações de personagens com proporções muito pequenas ou digitigrades.
E, servir de alternativa para fazer PlayerModels, Survivors e NPCs com maior diversidade de movimentos de forma não tão destrutiva com outros Addons.



## Wiki
Para facil manuseio, temos a [Wiki](https://github.com/LoveRenamon/Debiddos-Animations-private/wiki) explicando melhor as aplicações e uso desse repositório



## Dependências
Para uso desse repositório, você precisará:

**[Blender 3D](https://www.blender.org) 2.80.75** *ou mais novo* para modelagem e animação com algum **Addon** compatível para manipular, importar e exportar os arquivos necessários. *Recomendo [Blender Source Tools](http://steamreview.org/BlenderSourceTools/archives/)* pois funciona no Linux sem muitos problemas e tem suporte à ***Source 2***  

Adicionalmente **studiomdl.exe** da **Source Engine 2013**, para compilar os modelos. Esse está na pasta `bin` do seu Jogo.  

Se não sabe ao certo como usar essas ferramentas ou alguma que substitua, recomendo procurar apreender o básico através da [wiki](https://github.com/LoveRenamon/Debiddos-Animations-private/wiki).  



## Referências para construção de expressões faciais  

### Referências para FACs  
Para [Facial Action Coding System (imotions)](https://imotions.com/blog/facial-action-coding-system) há esse site que serve para construir e usar de referência as expressões faciais ou até mesmo o prórpio Starter Kit do Left 4 Dead 2  

#### ./mesh/FACS.dmx
  Segue o sistema de **[Facial Action Coding System]()** para mapear as expressões facis. esse é o método mais rápido de se fazer expressões facias na Source, e o mais difícil de customizar.  

* **[iMotions](https://imotions.com/blog/facial-action-coding-system)**  
* **[Carnegie Mellon’s School of Computer Science](https://www.cs.cmu.edu/~face/facs.htm)** de **Ekman** and **Friesen** *(1978)*   

### Referências para HWM
Para Hadware Morphs, temos o [HWMToolkit](https://github.com/revzin/HWMToolkit) de revzin, *(apesar de haver meu padrão prórpio, por compatibilidade é recomendado seguir o padrão da Valve)*

#### .mesh/HWM.dmx
  Segue o padrão novo de **[Hardware Morph]()** para movimentar partes da malha, isso o deixa mais próximo dos padrões atuais de de animação. É super versátil e permite **[normals]()** serem realinhadas, melhor suporte a **[wrinkle maps]()**, **[corrective shapes]()**.  
  Super fácil de customizar, porém exige bastante tempo posicionando cada shape/flex.  



## Referências de Estudo e Inspiração para esse projeto  
[oficial repo da Facepunch](https://github.com/robotboy655/gmod-animations)  
[HWMToolkit](https://github.com/revzin/HWMToolkit)  
[reanims_helpers-l4d2](https://github.com/xDShot/reanims_helpers-l4d2)  
[blender_l4d2_ik_rig](https://github.com/xDShot/blender_l4d2_ik_rig)  
[blender_gmod_ik_rig](https://github.com/xDShot/blender_gmod_ik_rig)  
