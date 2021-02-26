# <img src="./art/logo.png" width="60px;"/> Educación Siglo XXI

[![Deploy](https://github.com/EducacionSiglo21/jekyll/actions/workflows/deploy.yml/badge.svg)](https://github.com/EducacionSiglo21/jekyll/actions/workflows/deploy.yml)

Repositorio de código de la página web del Ateneo Villa de Molina de Segura [https://educacionsiglo21.github.io](https://educacionsiglo21.github.io).

Este repositorio contiene un sitio web estático generado con [Jekyll](https://jekyllrb.com/). Gestionado como un proyecto open source desde su nacimiento y bajo una [licencia](./LICENSE) MIT este proyecto evolucionará gracias a los miembros de [nuestra organización](https://github.com/orgs/EducacionSiglo21/people).

Si quieres colaborar en la edición y mantenimiento de este proyecto no dudes en enviarnos tus pull requests o solicitar una invitación a la organización enviando un email a [jornadassiglo21@gmail.com](mailto://jornadassiglo21@gmail.com).

# ¿Cuándo y como se actualiza la web?

La web se actualiza de forma automática (puede tardar unos minutos) cada vez cualquier archivo cambia, se añade o elimina en la rama principal del proyecto. También se actualiza cada día de forma automática para dejar de mostrar en la página principal actividades pasadas. Si se edita el contenido de algún post desde la web de GitHub manualmente, se añade un commit a la rama ``master`` diréctamente o se envía una pull request contra ``master`` la web se actualizará automáticamente.

# Participar añadiendo o editando contenido

Lo primero que debemos tener en cuenta es que para poder añadir o modificar contenido en la web de Educación Siglo XXI es que debemos crear una cuenta gratuita en [GitHub](https://github.com/). Gracias a esta cuenta podremos tener control sobre las colaboraciones que se hacen al proyecto y los autores de las mismas manteniendo el espíritu open source del proyecto :smiley:

Puedes crear tu cuenta de GitHub desde este [enlace](https://github.com/join?source=header-home). Aunque se puede seleccionar un plan de pago en el proceso de registro, nosotros solo necesitaremos un plan gratuito.

![gitHubSignUp](./art/githubSignUp.png)

Tras el proceso de registro recibirás un email para verificar tu cuenta. **Recuerda verificar tu cuenta, este paso es obligatorio y si no lo haces no podrás contribuir al proyecto**. Si pones una foto de perfil y un nombre nos ayudará bastante a comunicarnos durante las diferentes etapas de la colaboración.

Lo último, pero no por ello lo más importante, debes enviar un email a [jornadassiglo21@gmail.com](mailto://https://github.com/join?source=header-home) solicitando la admisión en la organización que hemos creado para Educación Siglo XXI. Esto te permitirá colaborar diréctamente sobre el proyecto sin realizar ningún fork de nuestros repositorios. Si tienes conocimientso de informática suficientes como para mantener tu propio fork del proyecto y enviar pull requests al repositorio principal, you are ready to go :rocket:

Una vez te enviemos la invitación a la organización Educación Siglo XXI en GitHub estarás listos para añadir o editar contenido en el proyecto de nuestra página web que encontrarás aquí: [https://github.com/educacionsiglo21/jekyll](https://github.com/educacionsiglo21/jekyll/)

![repository](./art/repositorio.png)

# Estructura del proyecto

Este repositorio contiene un proyecto de Jekyll que podemos modificar desde la propia web de GitHub. Contiene una serie de archivos ``html``, ``png``, ``jpg`` y ``md`` que contienen la información que se muestar en la web. Podemos cambiar de forma automática cualquier contenido mostrado en la web desde nuestro navegador modificando el contenido de los ficheros, **pero modificar parte del contenido es más sencillo que otro**. **Este proyecto está pensado para que personas sin un gran conocimiento sobre desarrollo web puedan cambiar el contenido de las actividades que organiza el equipo fácilmente**. Para ello solo tendrán que cambiar la información que aparece en los archivos ``.md`` dentro del directorio ``_posts``. A continuación detallaremos cómo añadir, editar y borrar contenido de la web junto con algo de información sobre como embeber vídeos de YouTube o imágenes que subiremos nosotros mismos.

**Disclaimer: Decidimos usar un sitio estático generado con Jekyll y que se pueda modificar desde GitHub para evitar los costes de mantenimiento asociados a servidores y derivados. Desde la organización de Educación Siglo XXI creemos que estra infraestructura es suficiente por ahora para las necesidades del proyecto.**

**Ten en cuenta que tras cada modificación, un servidor externo publicará los cambios que realices en la web. Este proceso puede tardar un poco, pero será automático y transparente para los usuarios.**

**Si por cualquier motivo crees que no puedes realizar la modificación o la adición de contenido que tienes en mente no dudes en ponerte en contacto con cualquier otro miembro de la organización. Son muy simpáticos y te ayudarán en todo momento con todo lo que necesites ** :smiley:

# Añadir contenido a la web

El proyecto está pensando para que añadamos actividades de forma sencilla y repetitiva. Para añadir otro tipo de páginas, por favor ponte en contacto con el resto de la organización. Este tipo de modificaciones no son sencillas.

**Consejo: Cuando tengas que crear una actividad nueva no escribas el archivo ``.md`` de la actividad desde cero. Copia uno ya existente y modifica su contenido. Esto te ayudará a cometer menos errores.**

Lo primero que debemos hacer cuando queramos añadir una actividad es subir las imágenes que vamos a utilizar. Para ello lo que haremos será subir contenido a la carpeta ``img/posts`` con un nombre de fichero que no se haya usado previamente.

Puedes acceder a la carpeta de imágenes pusando desde la página principal del repositorio en la carpeta llamada ``img`` o haciendo click en este enlace: [https://github.com/EducacionSiglo21/jekyll/tree/master/img](https://github.com/EducacionSiglo21/jekyll/tree/master/img)

***ES MUY IMPORTANTE QUE NOS NOMBRES DE LAS FOTOS NO CONTENGAN ESPACIOS EN BLANCO***

Una vez dentro de la carpeta llamada ``img`` solo tendrás que pulsar el boton ``Subir archivos``:

![uploadFiles1](./art/uploadFiles1.png)

Al hacer click en el enlace o en la carpeta de llamada ``img`` llegarás a esta pantalla:

![uploadFiles2](./art/uploadFiles2.png)

Luego solo tendrás que seleccionar el archivo que quieres subir y pulsar el botón ``commit``:

![uploadFiles2](./art/uploadFiles2.png)

**Recuerda que por cada actividad podrás subir las imágenes que necesites**.

Una vez subidas las imágenes podrás hacer referencia a ellas desde los archivos de las actividades de la siguiente forma

```
![foto](/img/posts/NOMBRE_DEL_FICHERO.EXTENSION_DEL_FICHERO)
```

Si subimos una foto llamada ``pedroGomez.png`` la podremos referenciar en los ficheros de las actividades de la siguiente forma:

```
![foto](/img/posts/pedroGomez.png)
```

**Una vez hemos subido las fotos estamos listos para crear nuestro fichero de actividad**

Cada actividad tiene un fichero asociado en la carpeta ``_posts``. Cuando creamos un fichero nuevo la pantalla principal de la web se actualiza para mostrar información de este fichero sin que tengamos que hacer nada. La pantalla de actividades también se actualiza mostrando una nueva actividad en la lista.

Podemos crear los ficheros de las atividades haciendo click en la carptea ``_posts`` o en el siguiente enlace: [https://github.com/EducacionSiglo21/jekyll/tree/master/_posts](https://github.com/EducacionSiglo21/jekyll/tree/master/_posts). Esto nos llevará a la siguiente pantalla:

![activities1](./art/activities1.png)

Este directorio contendrá un fichero por cada actividad listada [en la página del programa central de nuestra web](https://educacionsiglo21.github.io/programaCentral) o el [programa por localidades](https://educacionsiglo21.github.io/localidades).

Para añadir una actividad pulsaremos en el botón ``Crear nuevo archivo``.

![activities2](./art/activities2.png)

Que nos mostrará la siguiente pantalla:

![activities3](./art/activities3.png)

**El nombre que le pongamos al fichero en esta pantalla es muy importante. Tiene que tener el siguiente formato y no puede contener espacios**:

```
2018-01-01-el-reto-de-los-hombres-ante-la-igualdad.md

2018-01-31 // Fecha en la que publicamos la actividad, normalmente la fecha de hoy o un día pasado en formato AÑO-MES-DIA 

-el-reto-de-los-hombres-ante-la-igualdad // Nombre de la actividad separado por guiones y sin símbolos de puntuación.

.md // Extensión del fichero. Tiene que acabar en .md obligatoriamente
```

**Una vez tengamos el nombre del fichero es hora de ir a por el contenido**.

A continuación encontrarás un ejemplo de un fichero de actividad.

```markdown
---
layout: post
title: "Heike Freire en Alhama de Murcia"
subtitle: "Conferencia"
background: "/img/posts/bg-alhama.jpg"
eventdate: 2019-02-09 19:00:00 +0100
placeName: "Casa de la Cultura, Alhama de Murcia."
placeMapsUrl: https://www.google.es/maps/place/Casa+De+La+Cultura/@37.8508669,-1.4291304,17z/data=!3m1!4b1!4m5!3m4!1s0xd648e8dac18a665:0x8a353c478ef0cca2!8m2!3d37.8508627!4d-1.4269417
category: "local"
tags: "Alhama"
speakers:
    - name: "Raimundo de los Reyes"
      bio: "Director de IES"
    - name: "Mariola Sanz"
      bio: "Director de CEIP"
    - name: "Carlos Nicolás"
      bio: "Orientador"
presenters:
    - name: "Raimundo Benzal"
---

### Las nuevas masculinidades - Jueves, 18 Enero, 20:00h

Empezamos el año con un encuentro con la [Asociación de Hombre por la Igualdad de Género (AHIGE)](https://www.facebook.com/asociacion.ahige) con los que **charlaremos sobre la necesidad de que los hombres asumamos nuestra responsabilidad social y personal ante la injusticia que significa la discriminación en razón de sexo**, obtenemos la ventaja de poder situarnos ante el *machismo como algo dañino también para nosotros*.

![ahigelogo](/img/posts/ahigeLogo.png)

Por cada mujer cansada de tener que aparentar debilidad,
hay un hombre que disfruta de protegerla esperando sumisión.

```

Dentro de estos ficheros encontrarás una cabecera que contiene metadatos sobre el evento y que se usa en la página principal o la página de actividades para mostrar información sobre el mismo. Todos los metadatos se encuentran dentro de los caracteres ```---```. Aquí tienes una lista de lo que significa cada elemento:

```
layout: post # SIEMPRE TENEMOS QUE PONER ESTO
title: "Heike Freire en Alhama de Murcia" # TÍTULO DE LA ACTIVIDAD
subtitle: "Conferencia" # TIPO DE ACTIVIDAD O SUBTÍTULO
background: "/img/posts/bg-alhama.jpg" # FONDO QUE USAREMOS EN LA ACTIVIDAD
eventdate: 2019-02-09 19:00:00 +0100 # FECHA DEL EVENTO CON FORMATO, AÑO-MES-DIA HORA:MINUTOS:SEGUNDOS +0100 
placeName: "Casa de la Cultura, Alhama de Murcia." # NOMBRE DEL LUGAR DEL EVENTO
placeMapsUrl: https://www.google.es/maps/place/Casa+De+La+Cultura/@37.8508669,-1.4291304,17z/data=!3m1!4b1!4m5!3m4!1s0xd648e8dac18a665:0x8a353c478ef0cca2!8m2!3d37.8508627!4d-1.4269417 # URL A GOOGLE MAPS DEL LUGAR DEL EVENTO
category: "local" # CATEGORÍA, "local" o "central" dependiendo de si la actividad está asignada a una localidad o es central
tags: "alhama" # Nombre de la localidad o vacío si es del programa central
speakers: # Información de los speakers
    - name: "Raimundo de los Reyes" # Nombre del primer speaker
      bio: "Director de IES" # Cargo o información extra del primer spekaer
    - name: "Mariola Sanz" # Nombre del segundo speaker
      bio: "Director de CEIP" # Cargo o información extra del segundo spekaer
    - name: "Carlos Nicolás"
      bio: "Orientador"
presenters:
    - name: "Raimundo Benzal" # Nombre del presentador
```

Si por algún motivo no hay speakers o presentadores puedes borrar estas partes del fichero.

# Contenido con formato especial

El resto del fichero contiene la información que se mostrará en la página de detalle de la actividad. **Esta parte del fichero está escrita utilizando un lenguaje llamado markdown que nos permite añadir imágenes negritas y enlaces tal y como te indico a continuación**:

```markdown
//Añadir un enlace:

[nombreDelEnalce](https://cualquierenlace.com)

//Marcar texto en cursiva

Esto es un texto *en cursiva*.

//Marcar texto en negrita

Esto es un texto **importante**.

//Añadir una foto:

![nombreDeLaFoto](/img/posts/mifoto.png)

//Escribir un título:

# Título

//Escribir un subtítulo:

## Subtítulo

//Hacer una lista de elementos:

* Elemento 1
* Elemento 2
* Elemento 3
  * Elemento 3.1

//Escribir una cita:

> Mi cita célebre.

//Añadir un separador:

***

```

**Podrás encontrar más información sobre cómo usar elementos de markdown a parte de esta en el [siguiente enlace](https://markdown.es/sintaxis-markdown/)**.

Una vez tengas el contenido listo y escrito puedes añadirlo al campo de texto donde va el contenido del fichero y pulsar el botón ``commit``. **Tras unos minutos la web será actualizada y podrás ver tu contenido en el enlace que configuraste**

![activities4](./art/activities4.png)

**Tras unos minutos la web se actualizará cambiando la portada si la actividad que has añadido es la más reciente en el tiempo, añadiendo una nueva actividad a la pantalla de actividades y teniendo su contenido disponible en el enlace que configuraste**

# Modificar el contenido de la web

Para modificar el contenido de la web lo único que tienes que hacer es hacer log in con tu usuario de GitHub, seleccionar el archivo que quieres cambiar, pulsar el botón de editar, y tras realizar tus cambios pulsar el botón de que dice ``commit``. Encontrarás los ficheros que contienen la información sobre las actividades en el directorio llamado ``_post``.

![edit1](./art/edit1.png)

Una vez modificado el contenido del archivo, podrás guardar los cambios pulsando el botón ``commit`` al final de la página.

![edit2](./art/edit2.png)

La página se actualizará en unos minutos.

# Eliminar contenido de la web

Para borrar una actividad de la web solo tenemos que borrar el archivo asociado a la actividad en la carpeta ``_posts`` o ``img`` 

![delete1](./art/delete1.png)

# Problemas comunes

Cuando añadimos o editamos contenido es posible que por algún error no se visualce correctamente. A continuación vamos a listar los errores más comunes y cómo solucionarlos.

1. **He creado una actividad pero no se visualiza ni en la página de actividad ni en la principal**

Esto se debe a que el nombre del archivo no es correcto. Por ejemplo este:

```
2015-06-26-primer-concierto-tomas
```

El archivo de la actividad tiene que estar siempre dentro de la carpeta ``_posts`` y tener la extensión adecuada ``.md``. En este caso el archivo no contiene ``.md`` al final del nombre y esto hace que no se visualice. El nombre correcto del fichero sería:

```
2015-06-26-primer-concierto-tomas // INCORRECTO, LE FALTA LA EXTENSIÓN
2015-06-26-primer-concierto-tomas.md // CORRECTO
```

2. **He subido una foto pero no se ve cuando la enlazo en el banner, la actividad o el texto de la actividad.**

Cuando subimos una foto a ``/img/posts`` con el nombre ``nombredemifoto.png`` haremos siempre referencia a ella como: ``/img/posts/nombredemifoto.png``. En caso de que la extensión de la foto sea ``jpg`` usaremos ``/img/posts/nombredemifoto.jpg``. 

3. **He creado una actividad pero no se ve correctamente o no se pinta**

Revisa que no añadiste información en el fichero de la actividad que contenga el carácter ``:``. El carácter ``:`` solo puede usarse en la cabecera de la actividad (la información que va entre las tres rallitas ``---`` de principio del fichero) si se pone esa información entre comillas. 

El siguiente título no funcionará porque hay una carácter ``:`` después de la palabra ``Islam``.

```markdown
---
layout: post
title: Islam: ¿Paz o violencia?
---
```

Lo correcto sería ponerlo entre comillas. Si quieres lo puedes poner siempre entre comillas y así evitarás estos errores comunes:

```markdown
---
layout: post
title: "Islam: ¿Paz o violencia?"
---
```

**Recuerda, si estás subiendo contenido y no se visualiza quizás sea por estos motivos. Si aun revisando estos problemas comunes no consigues que se visualize solo tienes que avisar a alguien de la organización Ateneo de Molina de Segura y estaremos encantados de ayudarte.**

# Ejecutar este proyecto

Si necesitas modificar parte del código fuente que no está relacionado con las publicaciones y tienes que probar las modificaciones de las plantillas o cualquier otro elemento recuerda que puedes hacerlo fácilmente clonando este repositorio, instalando Ruby 2.X y Jekyll. Recuerdas que el contenido se puede añadir y modificar sin ningún tipo de software necesario más que un navegador como Google Chrome o Safari.

```
// Clonar el proyecto
git clone https://github.com/EducacionSiglo21/jekyll
cd jekyll

// Actualizar Ruby, bundler y jekyll
curl -L https://get.rvm.io | bash -s stable
rvm install ruby-2.4.1
rvm use ruby-2.4.1
rvm --default use 2.4.1
gem install bundler jekyll

// Lanzar el servidor de desarrollo en el puerto 4000
// Tras ejecutar el comando podrás acceder a la web en [localhost:4000](localhost:4000)
bundle exec jekyll serve --livereload

// Construir el proyecto. Tras la ejecución de este comando la carpeta _site contendrá los archivos
// que compondrán nuestro sitio web
bundle exec jekyll build 
```

En esta web encontrarás algo de información sobre cómo utilizar las plantillas o algunos comandos útiles [aquí](https://devhints.io/jekyll).