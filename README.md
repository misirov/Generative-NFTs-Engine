# Generative-Art-Engine
> Takes .png images as input in the ```/layers``` folder and outputs mixed images + json metadata in a ```/build``` folder. 

<br>

#### How to use: You need to have Node.js installed on your computer. Then, download this repository, open it on VSCode, open the terminal and type:
1) ```yarn install``` or ```npm install```
2) In  `src/config.js` change the ```layerConfigurations```:
    - ```growEditionSizeTo```: How many editions you want to generate. *note that it will depend on how many images are available*
    - ```layersOrder```: name of the folders containing the images in the order you want them to be layered. ex:

```Javascript
const layerConfigurations = [
    {
      growEditionSizeTo: 10,
      layersOrder: [
        { name: "background" },
        { name: "eyes" },
        { name: "mouth" },

      ],
    },
  ];
```
    
3) The name of the images must be made out of ```name``` + ```#``` delimiter + ```round number between 10-100``` to specify rarity. ex:
     - ```eyes#30.png``` , ```mouth#60.png``` ...
4) When ready, run ```node ./index.js``` or ```npm run build```

more at: https://github.com/HashLips/hashlips_art_engine

>I got several issues while testing this,<br>
if you were to have one feel free to ping me;<br>
P.M
  
