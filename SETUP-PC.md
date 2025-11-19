# Machine Learning Aplicado con Python

## Instrucciones de configuración para Windows

### Parte 1: Clonar el Repo

Aquí vas a obtener una copia local del código en tu ordenador.

1. **Instala Git** si no está ya instalado


- Descarga Git desde https://git-scm.com/download/win

2. **Abrir el símbolo del sistema:**

- Presiona Win + R, y escribe `cmd`, para luego pulsar Enter

3. **Navega hasta tu carpeta de proyecto:**

Si tienes una carpeta específica para proyectos, navega hasta ella utilizando el comando cd. Por ejemplo  
`cd C:\Dev\Machine Learning Aplicado con Python`

Si no tienes una carpeta de proyectos, puedes crear una:
```
mkdir C:\Dev\Machine Learning Aplicado con Python
cd C:\Dev\Machine Learning Aplicado con Python
```
4. **Clonar el repositorio:**

Ingresa la siguiente instrucción en el símbolo del sistema en la carpeta Proyectos:

`git clone https://github.com/Tectroya/ML-Aplicado-Python.git .`


### Parte 2: Instalar el Entorno de Anaconda

1. **Instala Anaconda:**

- Descarga Anaconda desde https://docs.anaconda.com/anaconda/install/windows/ te pedira que te registres previamente.
- Ejecuta el instalador y sigue las instrucciones. Ten en cuenta que ocupa varios GB y que la instalación demora un tiempo.

2. **Configurar el entorno:**

- Abre **Anaconda Prompt** (búscala desde el menú de inicio)
- Navegue hasta el "directorio raíz del proyecto" ingresando algo como `cd C:\Dev\Machine Learning Aplicado con Python`
- Crea el entorno: `conda env create -f environment.yml`
- Si te da este error:
```
Error while loading conda entry point: conda-libmamba-solver (module 'libmambapy' has no attribute 'QueryFormat')

CondaValueError: You have chosen a non-default solver backend (libmamba) but it was not recognized. Choose one of: classic
```
Prueba forzando el comando de actualización, a usar también el solucionador "classic":
`conda update -n base conda conda-libmamba-solver --solver=classic`
Y luego repite:
`conda env create -f environment.yml`

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