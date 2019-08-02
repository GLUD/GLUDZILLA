# Inicia con A-Frame

[glitch]: http://glitch.com/~aframe
[glud]: http://glud.org

Puedes empezar con A-Frame desde un archivo de html común y corriente sin tener que instalar ninguna aplicación adicional. Un buen lugar para comenzar con el desarrollo con esta herramienta es con el ejemplo que realizamos con **[Glitch][glitch]**, que es un editor de código en la web que permite el desarrollo de forma gratuita. También de forma alternativa se puede crear un archivo .html e incluir en el `<head>` CDN de A-Frame.

```html
<html>
  <head>
    <script src="https://aframe.io/releases/0.9.2/aframe.min.js"></script>
  </head>
  <body>
    <a-scene>
      <a-box position="-1 0.5 -3" rotation="0 45 0" color="#4CC3D9"></a-box>
      <a-sphere position="0 1.25 -5" radius="1.25" color="#EF2D5E"></a-sphere>
      <a-cylinder position="1 0.75 -3" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
      <a-plane position="0 0 -4" rotation="-90 0 0" width="4" height="4" color="#7BC8A4"></a-plane>
      <a-sky color="#ECECEC"></a-sky>
    </a-scene>
  </body>
</html>
``` 

[Instalación]: ./installation.md
[Escuela de A-Frame]: https://aframe.io/school/

La página de  [Instalación] te puede dar mas opciones para empezar con A-frame. Para empezar a aprender como puedes usar este framework, puedes mirar la [Escuela de A-Frame] para empezar paso por paso de una forma más gráfica y visual, lo puedes usar también para complementar la guía actual.

# ¿Qué es A-Frame?
[github]: https://github.com/aframevr/
[community]: https://aframe.io/community/

![A-Frame](https://cloud.githubusercontent.com/assets/674727/25392020/6f011d10-298c-11e7-845e-c3c5baebd14d.jpg)

:a:-Frame Es un framework orientado hacia la web que permite al usuario construir experiencias con realidad virtual.
A-Frame se basa en la estructura de HTML, haciendo que este sea más simple para empezar. Pero A-Frame
no es solo un gráficador de escenas en 3D o a lenguaje de etiquetas; el núcleo del framework es muy poderoso el paradigma Entidad-Componente ya que provee una paradigma apto para declarar, extender, y
con una estructura modificable en el [three.js].

Originalmente fue concebido en una colaboración entre Mozilla y ahora mantenido por los co-creadores de
A-Frame entre [Supermedium](https://supermedium.com), A-Frame fue desarrollado para
ser un fácil pero poderosa forma para el desarrollo de contenido orientado a la Realidad Virtual. Como un  [proyecto de codigo abierto][github], A-Frame ha crecido para ser una de las [comunidades mas grandes de realidad virtual][community].

A-Frame soporta los diferentes cascos VR tales como Vive, Rift, Windows Mixed Reality,
Daydream, GearVR, Cardboard, Oculus Go, e incluso se puede utilizar para la realidad aumentada.  Aunque A-Frame soporta el  espectro, A-Frame tiene como objetivo definir una experiencia de realidad virtual que va  mas allá de  lo básico con contenido de 360&deg;, logrando un control total de el uso de controles y seguimiento de la posición del objeto que se cuestión.

<div class="docs-introduction-examples">
  <a href="https://supermedium.com/supercraft">
    <img alt="Supercraft" target="_blank" src="https://user-images.githubusercontent.com/674727/41085457-f5429566-69eb-11e8-92e5-3210e4c6c4a0.gif" height="190" width="32%">
  </a>
  <a href="https://aframe.io/a-painter/?url=https://ucarecdn.com/962b242b-87a9-422c-b730-febdc470f203/">
    <img alt="A-Painter" target="_blank" src="https://cloud.githubusercontent.com/assets/674727/24531388/acfc3dda-156d-11e7-8563-5bd75252f70f.gif" height="190" width="32%">
  </a>
  <a href="https://supermedium.com">
    <img alt="Supermedium" target="_blank" src="https://user-images.githubusercontent.com/674727/37294616-7212cd20-25d3-11e8-9e7f-c0c61074f1e0.png" height="190" width="32%">
  </a>
  <a href="https://aframe.io/a-blast/">
    <img alt="A-Blast" target="_blank" src="https://cloud.githubusercontent.com/assets/674727/24531440/0336e66e-156e-11e7-95c2-f2e6ebc0393d.gif" height="190" width="32%">
  </a>
  <a href="https://aframe.io/a-saturday-night/">
    <img alt="A-Saturday-Night" target="_blank" src="https://cloud.githubusercontent.com/assets/674727/24531477/44272daa-156e-11e7-8ef9-d750ed430f3a.gif" height="190" width="32%">
  </a>
  <a href="https://github.com/googlecreativelab/webvr-musicalforest">
    <img alt="Musical Forest by @googlecreativelab" target="_blank" src="https://cloud.githubusercontent.com/assets/674727/25109861/b8e9ec48-2394-11e7-8f2d-ea1cd9df69c8.gif" height="190" width="32%">
  </a>
</div>


## Features

:eyeglasses: **Realidad Virtual lo hace todo más simple **: Con tan solo poner dentro del `<script>` la etiqueta `<a-scene>`.
A-Frame puede crear un escenario 3D, una instalación de Realidad Virtual, y unos controles predeterminados. Nada de instalar, ni procesos de construcción.

:heart: **HTML Declarativo**: El lenguaje HTML es fácil de leer, entender, y realizar una copia y pegado mas simple. ya que es basado en HTML, A-Frame es accesible para todos:
desarrolladores web, entusiastas de Realidad Virtual, artistas, diseñadores, educadores, creadores y niños.

:electric_plug: **Arquitectura Entidad-Componente**: A-Frame es un poderoso
[three.js] framework, dando una semántica declarativa, manejable, re utilizable
[arquitectura entidad-componente][ecs]. HTML es solo la punta del iceberg;
los desarrolladores tienen acceso ilimitado al JavaScript, DOM APIs, three.js, WebVR, y
WebGL.

:globe_with_meridians: **Plataforma cruzada Realidad Virtual**: La construcción de aplicaciones con Realidad Virtual  para Vive, Rift, Windows Mixed Reality, Daydream, GearVR, y tarjetas con soporte para
todos los respectivos controles. Si no tienes estos artilugios? No hay problema!
A-Frame también trabaja en entornos de web de escritorios y teléfonos inteligentes.

[ecs]: ./entity-component-system.md

[A-Painter]: https://github.com/aframevr/a-painter
[Tilt Brush]: https://www.tiltbrush.com/

:zap: **Rendimiento**: A-Frame está optimizado para el ground up for WebVR. Mientras A-Frame usa el DOM,estos elementos no tocan el motor de diseño del navegador. 
La actualización de los objetos 3D son todos realziados en la memoria con colector de basura  y sobrecarga. La mayor interacción y muy gran escala. Las aplicaciones WebVR más interactivas y de gran escala se han realizado en A-Frame funcionando a 90 fps sin problemas

[inspector]: ./visual-inspector-and-dev-tools.md

:mag: **Inspector Visual**: A-Frame proporciona una incorporación practica de [visual 3D
inspector][inspector].Abrir *cualquier* escena en A-frame, pulse `<ctrl> + <alt> + i`, y volar alrededor para visualizar debajo de la cúpula.


![Inspector](https://cloud.githubusercontent.com/assets/674727/25377018/27be9cce-295b-11e7-9098-3e85ac1fe172.gif)

[augmented reality]: https://github.com/jeromeetienne/AR.js#augmented-reality-for-the-web-in-less-than-10-lines-of-html
[environment]: https://github.com/supermedium/aframe-environment-component
[multiuser]: https://github.com/haydenjameslee/networked-aframe
[oceans]: https://github.com/donmccurdy/aframe-extras/tree/master/src/primitives
[particle systems]: https://github.com/IdeaSpaceVR/aframe-particle-system-component
[physics]: https://github.com/donmccurdy/aframe-physics-system
[state]: https://npmjs.com/package/aframe-state-component
[super hands]: https://github.com/wmurphyrd/aframe-super-hands-component
[teleportation]: https://github.com/fernandojsg/aframe-teleport-controls

:runner: **Componentes**: Arranca a toda velocidad con los componentes centrales con A-Frame como las  geometrías , materiales, luces, animaciones, modelos, 

Comience a codificar con a A-Frame's con los componentes de el framework 
tales como figuras geométricas, materiales, luces, animaciones, modelos, raycasters (intersección rayo-superficies),sombras,audio posicioinal, texto, controles pocicionales, texto, 
y controladores para la mayoría de gafas de realidad virtual. La comunidad a aportado con varios de los componentes como [el medio ambiente],el [estado], [sistemas de particulas],
 [Físicas], [varios usuarios], [océanos], [tele-transportación], [controles de manos], y
[realidad aumentada].

:earth_americas: **Probado y escalable**: A-Frame ha sido utilizado por compañías
como Google, Disney, Samsung, Toyota, Ford, Chevrolet, Amnesty
International, CERN, NPR, Al Jazeera, The Washington Post, NASA. Algunas de estas
compañías como Google, Microsoft, Oculus, y Samsung también han hecho contribuciones a
 A-Frame.

## Inicia!

[Discord]: https://supermedium.com/discord

Si es tu primera vez con A-Frame, hay un plan de inicio para ti:

1. Para inspirarte, podrías mirar lo que otras personas han construido con A-Frame en el
[Blog](https://aframe.io/blog/) o el [Directorio WebVR](https://webvr.directory).

2. Lee la documentación para entender mejor el código.
[Glitch](https://glitch.com/~aframe) lo puedes utilizar como un entorno de desarrollo para 
aplicativos desarrollados con A-Frame.

3. Ejecuta la escuela de [A-Frame](https://aframe.io/school/), Es un pequeña guía gráfica
`para el desarrollo paso a paso de entornos con A-Frame.

4. [Unetenos a Slack](https://aframe.io/slack-invite) o [Discord] y si tienes
alguna pregunta, [busca y pregunta en
StackOverflow](http://stackoverflow.com/questions/ask/?tags=aframe), y alguien intentara
ayudarte o comunicarse con usted!

5. Cuando crees algo, comparte tu proyecto en la web y podria aparecer en 
el top semanal de A-Frame [*A Week of A-Frame*](https://aframe.io/blog/)!

Esto también te ayuda a mejorar tus habilidades de JavaScript y
three.js. Diviértete!
