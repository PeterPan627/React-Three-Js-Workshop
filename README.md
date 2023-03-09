# React-Three-Js-Workshop

<h1>Introduction</h1>
Salut !<br>
Bienvenue dans notre Workshop. Aujourd'hui vous allez aborder les bases de React ThreeJS.<br>
Pour éviter de vous y perdre, suivez les différentes étapes unes par unes :).

<br>
<br>
<h2>Etape 1 :</h2>
Cloner le repo !<br><br>

```
git clone git@github.com:RayanBn/React-Three-Js-Workshop.git
```
Etapes a suivre pour compiler :

```
npm install
```

```
npm run dev
```

<h2>Etape 2 :</h2>
<br>
Commencons par apprendre a creer des objets. (Experience.js)<br><br>

```js
<mesh>
    <boxBufferGeometry></boxBufferGeometry>
    <meshStandardMaterial></meshStandardMaterial>
</mesh>
```

A vous de jouer avec les parametre de l'objet, pour obtenir le resultat qui vous plait !
Une fois l'objet créé, vous pourrez constater que sa couleur ne s'apliquera pas.
Pour régler ce soucis, vous devez ajouter des lumières a votre scene.<br><br>
https://docs.pmnd.rs/react-three-fiber/getting-started/your-first-scene#adding-lights

<h2>Etape 3 :</h2><br>

Mouvement de la camera, dans votre objet Canva du fichier index.js, une camera a deja été ajouté a la scene. A vous de vous informer sur celle-ci et de pouvoir la modifier et la manipuler a votre guise !

```js
camera={ {
    fov: 45,
    near: 0.1,
    far: 200,
    position: [ -4, 3, 6 ]
} }
```
Le but ici est de pouvoir creer un controle de camera, ce qui va vous permettre de tourner au tour de votre scene ! (OrbitControl)


<h2>Etape 4 :</h2><br>

Essayons maintenant de faire bouger les objects present sur notre scene. Pour pouvoir interagir avec les objets de notre scene en react, nous avons besoin d'utiliser des Hooks.
Le Hook le plus utilisé en React Three est UseFrame, celui-ci va prendre en parametre une fonction qui va etre appelé a chaque frame de votre scene. Voici un lien qui va vous permettre d'apprendre à l'utiliser:<br><br>
https://docs.pmnd.rs/react-three-fiber/api/hooks#useframe
<br>
```js
import { useFrame } from '@react-three/fiber'

function Foo() {
  useFrame((state, delta, xrFrame) => {
    // This function runs at the native refresh rate inside of a shared render-loop
})
```

<h2>Etape 5:</h2><br>
Amusez vous ! Si ce workshop vous a plus, hésitez pas a star le repo ! :)
