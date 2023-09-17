# Simple-AR-demostration 👩🏼‍💻

### ☞ Notion Page ➡️ https://carolina-riddick.notion.site/Principios-de-una-AR-app-48bb3300422c450f94d41d5aeb552bf3?pvs=4
### ☞ Linkedin ➡️ https://www.linkedin.com/in/carolina-riddick/?locale=en_US
-----
## What do you need?
We need 4 objects:

1. **`Wikitude Camera`**
2. **`Trackable Object`** which has the marker.
    1. The **`Marker`** or **`marker`** (**Image**, jpg extension and can be printed or not, so that the object can be placed there)
3. `**Image Tracker` / `Image Tracker`** (who will have a Trackable child)
    1. Search for the image or mark
    2. This mark must be placed in **`.wtc`** format within the options given by the Image Tracker.
4. **`Virtual object`** to **render** as child of **`Trackable`**.
---
## Image Tracker / Image Tracker
- The **`Image Tracker`** has **`Trackable`** who will be **in charge of **tracking** the image trained on the camera.
- When it finds the image trained on the camera, it will carry out other processes where it will finally render the object.
---
### How do we configure the **`Trackable`** ?
- Click on Image Tracker and inside it, in the inspector panel we have all its settings and properties.    
---
### What is a bear.wtc file?
- It is the trained version of an image.
---
## Steps
1. Place in the project folder (**`Assets`**), the unity package **`wikitude.unitypackage`**.
    1. **`Import`**

2. You should add the .wtc file inside the **`Wikitude`** folder.
       
    1. The **`Wikitude`** camera will be looking for these images all the time in the video stream and then *plaster a virtual object on that marker* 2.
3. Place in the project folder (**`Assets`**), the unity package **`TeddyBear.unitypackage`** 1.
    1. **`Import`**
    2. We brought the model
                
4. We add a **`wikitude Camera`**
5. We eliminate the **`main camera`** brought by default of unity
      
6. We add an `**Image Tracker`** / `Image Tracker`**.
- What this image tracker does is find our marker in the video feed / What this image tracker does is finding our marker in the video feed
    
7. This image Tracker has a child called Trackable *(Trákabl)* 8.
        
8. What we have to do with this **`Rastreador de imagenes / Image Tracker`** is to link it with our **`imagen entrenada / Trained image`(bear.wtc file).**
- In this way the *Image tracker* is going to search (*by means of the camera ****************Wikitude*****************) to our *trained image*.

9. Anything that we place in the **`Wikitude`** folder in **`StreamingAssets` *will be available in Wikitude for viewing in the panel that opens***.
10. Click on **`Trackable` where the image we selected will appear, this will be the image that will be tracked and searched by our image tracker**.   

----
## Summary: 1. The **`Wikitude Camera`** will take the camera from our Web Cam and the **`Image Tracker`** will search for a **`trackable objects`** where in this case it is our trained image ( bear.wtc)**.
2. What image is to be rendered?*We need to place a virtual object that will be rendered in our trained image.
    1. We look in **`Assets`** for our prefab to be rendered.
    2. <img width="162" alt="Screenshot 2023-09-17 at 1 45 25 p m" src="https://github.com/Carolina-Riddick/Simple-AR-demostration/assets/107819898/a3a78d6e-0459-4f3d-9a76-f932ec8954fc">
    3. We place in the hierarchy
    4. This virtual object ****************************************es child of Trackable****************************************        

1. The virtual object must be rendered in a certain position...
    1. This means that our Teddy bear will be placed in the position **`0 of X, 0 of Y, and 0 of Z`**, therefore it will be in the **********center of our trained image**********         
2. En la Scene, veremos el objeto virtual       
3. Play!
   1. Se reproducira la camara de nuestra PC y con nuestra imagen impresa podremos observar nuestro modelo, en este caso a Teddy !

<img width="1120" alt="Captura de pantalla 2023-09-17 a las 1 22 18 p  m" src="https://github.com/Carolina-Riddick/Simple-AR-demostration/assets/107819898/ee453f42-4960-40c1-80b6-e05bcb32be64">

<img width="858" alt="Captura de pantalla 2023-09-17 a las 1 45 36 p  m" src="https://github.com/Carolina-Riddick/Simple-AR-demostration/assets/107819898/c880d799-1080-4b9e-9427-6298fd425802">

<img width="858" alt="Captura de pantalla 2023-09-17 a las 1 46 00 p  m" src="https://github.com/Carolina-Riddick/Simple-AR-demostration/assets/107819898/03937602-c90a-4edc-a6c1-2cc09ea16527">


## ------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## ***Spanish Version***
-------
➡️ Una simple demostracion de una app de Realidad Aumentada con los pasos a seguir para realizarla

## Que necesitamos?

Necesitamos 4 objetos:

1. **`Wikitude Camera`**
2. **`Trackable Object / Objeto Rastreable`** que tiene la marca / marker
    1. La **`Marker`** o **`marca`**  (**Imagen**, con extension jpg y puede estar impresa como no,  para poder colocar el objeto ahi)
3. **`Image Tracker` / `Rastreador de imagen`** (quien tendra un hijo Trackable)
    1. Buscara la imagen o marca
    2. Esta marca debe ser colocara en formato **`.wtc`** dentro de las opciones que da el Rastreador de imagen
4. **`Virtual object`** to **render** as child of **`Trackable`**
---
## Image Tracker / Rastreador de imagen
- El **`imagen Tracker  o Rastreador de imagenes`** tiene **`Trackable`** quien sera el **encargado de rastrear** la imagen entrenada en la camara
- Cuando este encuentre la imagen entrenada en la camara, llevara a cabo otros procesos donde finalmente renderizara el objeto.
---
### Como configuramos el **`Trackable`** ?
- Clickeamos en Imagen Tracker y dentro de el, en el panel de inspector tenemos todas sus configuracions y propiedades    
---
### Que es un archivo bear.wtc
- *Es una version entrenada de una imagen*
---
## Pasos
1. Colocar en la carpeta de proyectos (**`Assets`**), el unity package **`wikitude.unitypackage`**
    1. **`Import`**
    2. Nos trajimos la marca
2. Colocar **SI O SI** dentro de la carpeta **`Wikitude`** dentro de `**StreamingAssets**` el unity el archivo .wtc es decir la **`imagen entrenada`** / the **`trained marker`**
       
    1. La camara **`Wikitude`** estara buscando a estas imagenes todo el tiempo en la transmision de video para luego *plasmar un objeto virtual en esa marca*
3. Colocar en la carpeta de proyectos (**`Assets`**), el unity package **`TeddyBear.unitypackage`**
    1. **`Import`**
    2. Nos trajimos el modelo
                
4. Agregamos un **`wikitude Camera`**
5. Eliminamos la **`main camara`** traida por default de unity
      
6. Agregamos un **`rastreador de imagen` / `Image Tracker`**
    1. Lo que hace es encontrar nuestro marcador en el vídeo / What this image trackar does is finding our marker in te video feed
    
7. This image Tracker has a child called Trackable *(Trákabl)*
        
8. Lo que debemos hacer con ese **`Rastreador de imagenes / Image Tracker`** es vincularlo con nuestra **`imagen entrenada / Trained image`(bear.wtc file).** 
        
    1. De esta forma el *Image tracker* va a buscar (*por medio de la camara ****************Wikitude*****************) a nuestra  *imagen entrenada*
                
9. Cualquier cosa que nosotros coloquemos en la carpeta **`Wikitude`** dentro de **`StreamingAssets` *estara disponible dentro de Wikitude para poder verse en ese panel que se abre***
10. Click on **`Trackable` donde aparecera la imagen entrenada que seleccionamos, ésta sera la imagen que rastreara y buscara nuestro rastreador de imagenes**   
----
## Resumen:
1. El **`Wikitude Camera`** tomara la camara de nuestra Web Cam y el **`Image Tracker`** buscara por un **`trackable objects / objetos rastreables` donde en este caso es nuestra imagen entrenada ( bear.wtc)**
2. Que imagen se va a renderizar? *Necesitamos colocar un objeto virtual que sea renderizado en nuestra imagen entrenada.*
    1. Buscamos en **`Assets`** nuestro prefab a renderizar
    2. <img width="162" alt="Captura de pantalla 2023-09-17 a las 1 45 25 p  m" src="https://github.com/Carolina-Riddick/Simple-AR-demostration/assets/107819898/a3a78d6e-0459-4f3d-9a76-f932ec8954fc">
    3. Colocamos en la jerarquia
    4. Esta objeto virtual ****************************************es hijo de Trackable****************************************        

1. El objeto virtual debera ser renderizado en una posicion determinada…
    1. Esto significa que nuestro Teddy bear sera colocaro en la posicion **`0 de X, 0 de Y y 0 de Z`**, por ende estara en el **********centro de nuestra imagen entrenada**********
            
    1. En la Scene, veremos el objeto virtual       
3. Play!
   1. Se reproducira la camara de nuestra PC y con nuestra imagen impresa podremos observar nuestro modelo, en este caso a Teddy !
