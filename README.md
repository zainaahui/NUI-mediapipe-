# NUI & MediaPipe · experiencias interactivas en tiempo real

Este repositorio reúne experiencias de **Interfaz Natural de Usuario (NUI)** desarrolladas con tecnologías web y **MediaPipe**, permitiendo interactuar con elementos visuales y personajes mediante gestos de manos, postura corporal y guiños faciales a través de la cámara web.

## Conceptos clave

* **Interfaz Natural de Usuario (NUI):** paradigma de interacción donde el usuario se comunica con el sistema mediante acciones humanas intuitivas (gestos, movimientos del cuerpo o expresiones faciales) en lugar de depender únicamente de teclado o ratón.
* **MediaPipe:** marco de trabajo de visión por computadora de Google que permite detectar puntos clave (*landmarks*) en tiempo real directamente en el navegador para reconocer manos, postura corporal y rostro.

## Estructura del repositorio

* **`index.html`:** portal principal del proyecto. Explica los conceptos de NUI y MediaPipe y permite navegar hacia las distintas experiencias interactivas.
* **`jellybaby.html` (Manos):** utiliza **MediaPipe Hands** y **Three.js** para controlar a *Jellybaby* en una escena 3D[cite: 1]. Permite moverlo, hacerlo saltar abriendo la mano, aplastarlo cerrando el puño, hacer *pop* pellizcando y variar el tono según la altura de la mano (con respaldo de ratón y teclado)[cite: 1].
* **`indexcuerpo.html` (Cuerpo):** utiliza **MediaPipe Pose** y **HTML5 Canvas** para detectar el cuerpo completo[cite: 2]. Al formar un corazón con los brazos genera corazones, y al levantar la pierna izquierda o derecha activa lluvias de estrellas[cite: 2].
* **`indexcara.html` (Cara):** utiliza **MediaPipe Face Mesh** y el cálculo de apertura ocular (**EAR**) para alternar entre **Modo Ángel** (halo dorado, alas y partículas) y **Modo Demonio** (cuernos, brillo rojizo y chispas) al guiñar el ojo izquierdo o derecho[cite: 3].

## Requisitos y ejecución

1. Subir todos los archivos (`index.html`, `jellybaby.html`, `indexcuerpo.html`, `indexcara.html` y este `README.md`) a la raíz del repositorio[cite: 1, 2, 3].
2. Abrir el proyecto en un entorno servido por **HTTPS** (como **GitHub Pages**) o en **`localhost`**, ya que los navegadores exigen un contexto seguro para otorgar permisos de acceso a la cámara web[cite: 1].
3. Al ingresar, activar la cámara y conceder los permisos correspondientes en el navegador[cite: 1, 2, 3].

## Tecnologías utilizadas

* **HTML5, CSS3 y JavaScript**[cite: 1, 2, 3]
* **MediaPipe** (Hands, Pose y Face Mesh)[cite: 1, 2, 3]
* **Three.js**[cite: 1]
* **HTML5 Canvas y Tailwind CSS**[cite: 2, 3]
