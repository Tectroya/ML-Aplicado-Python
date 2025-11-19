# Machine Learning Aplicado con Python

## Instrucciones de configuración para Mac

### Parte 1: Clonar el Repo

Aquí vas a obtener una copia local del código en tu ordenador.

1. **Instala Git** en casi todos los Mac viene instaldo por defecto

- Abre el Terminal (Aplicaciones > Utilidades > Terminal)
- Escribe `git --version` Si no está instalado, se te pedirá que lo instales pulsado intro.
- O puedes descarga Git desde https://git-scm.com/download/

2. **Navega hasta la carpeta de tus proyectos:**.

Si tienes una carpeta específica para proyectos, navega hasta ella usando el comando cd. Por ejemplo
`cd C:\Dev\Machine Learning Aplicado con Python`

Si no tienes una carpeta de proyectos, puedes crear una:
```
mkdir C:\Dev\Machine Learning Aplicado con Python
cd C:\Dev\Machine Learning Aplicado con Python
```

3. **Clonar el repositorio**

- Ve a la página GitHub del curso
- Haz clic en el botón verde 'Código' y copia la URL
- En Terminal ubicate en la carpeta raiz, escribe esto, `git clone https://github.com/Tectroya/ML-Aplicado-Python.git .` 


### Parte 2: Instalar el entorno de Anaconda

Existe una alternativa a la Parte 2 si esto te causa problemas.

1. **Instala Anaconda:**

- Descarga Anaconda desde https://docs.anaconda.com/anaconda/install/mac-os/ (Es posible que debas registrarte)
- Haz doble clic en el archivo descargado y sigue las instrucciones de instalación. Ten en cuenta que ocupa varios GB y que la instalación demora un poco.

2. **Configurar el entorno:**

- Abre una nueva Terminal (Aplicaciones > Utilidades > Terminal)
- Navega hasta el "directorio raíz del proyecto" usando `cd C:\Dev\Machine Learning Aplicado con Python` (reemplaza esta ruta según sea necesario con la ruta real a tu directorio). 
- Crea el entorno mediante: `conda env create -f environment.yml`
- Espera unos minutos a que se instalen todos los paquetes. En algunos casos, esto puede llevar literalmente entre 20 y 30 minutos si no has utilizado Anaconda antes, e incluso más tiempo según tu conexión a Internet.
- Ahora debes **activarlo** con este comando: 
```
conda activate ml
```

Deberías ver `(ml)` en tu prompt, lo que indica que has activado tu nuevo entorno.

3. **Inicia Jupyter Lab:**

- Navegue hasta el "directorio raíz del proyecto" ingresando algo como `cd C:\Dev\Machine Learning Aplicado con Python`, y escribe: 
```
jupyter lab
```


...y Jupyter Lab debería abrirse en tu navegador. Ahora cierra la pestaña del navegador de Jupyter Lab, cierra la Terminal.