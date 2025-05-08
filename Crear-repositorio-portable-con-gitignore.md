## 📁 Crear repositorio de trabajo portable

```
mi-proyecto/
│
├── .venv/               # Carpeta del entorno virtual (ignorada por Git)
├── requirements.txt      # Archivo con las dependencias del proyecto
├── script.py             # Tu código fuente
├── README.md             # Documentación del proyecto
└── .gitignore            # Archivos que se ignoran en el control de versiones
```

### Contenido total del archivo `.gitignore`

```
.venv/
*.pyc
__pycache__/
*.pyo
*.log
```



## 📁 Ignorar archivos de trabajo en Git

### QE

Agregar las siguientes líneas al archivo `.gitignore` para evitar subir archivos de salida o temporales al repositorio:

```gitignore
*.out
*.in
*.save/
tmp/
```

### venv de Python y otras lineas generadas por Python

Agregar esta línea al archivo `.gitignore` para evitar subir `.venv/` y las demás al repositorio:

### 📁 Ignorar el entorno virtual de Python en Git y otras carpetas generadas por Python

Agregá esta línea a tu archivo `.gitignore` para evitar subir `.venv/` al repositorio:

```gitignore
.venv/
__pycache__/
```
> __pycache__/ es una carpeta que Python crea para almacenar los archivos .pyc y .pyo de cada módulo o script que se ejecute. Dentro de esta carpeta, Python guarda las versiones compiladas de tus archivos .py para que no tengan que ser recompiladas en futuras ejecuciones. Es nomás para hacerlo más eficiente.

### Archivos *.log 

```gitignore
*.log
```

> El *.log en el archivo .gitignore sirve para ignorar todos los archivos de registro (logs) generados durante la ejecución del programa. Los archivos .log son comúnmente utilizados para registrar información, errores o advertencias sobre el comportamiento de una aplicación o script, especialmente durante el desarrollo o la depuración.
