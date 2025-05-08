### Resumen

Como crear venv de python para instalar paquetes de manera prolija y saber donde estan por si quiero desinstalar etc. Además como poner todo lo instalado en requeriments.txt, para que después en un repo nuevo, me creo el venv y le instalo todo junto. Asi se siempre qué intérprete de Python estoy usando y qué paquetes tengo qué versiones etc.

## Cómo crear un entorno virtual Python con paquetes específicos

Previamente tener instalado pip y Python3

### 1. Crear la estructura del proyecto (si no existe)

```bash
mkdir -p ~/proyectos/mi-proyecto
cd ~/proyectos/mi-proyecto
```

### 2. Crear el entorno virtual dentro del proyecto

```bash
python3 -m venv .venv
```

> Esto crea un entorno aislado dentro de la carpeta `.venv/`.

### 3. Activar el entorno virtual

```bash
source .venv/bin/activate
```

> El prompt cambiará para mostrar que estás dentro del entorno.

### 4. Instalar los paquetes necesarios

```bash
pip install numpy matplotlib
```

> Reemplazá o agregá los paquetes que necesites.

### 5. Guardar las dependencias instaladas (opcional)

```bash
pip freeze > requirements.txt
```

> Esto genera un archivo con las versiones exactas de los paquetes para reproducir el entorno.

---

### 📁 Ignorar el entorno virtual en Git

Agregá esta línea a tu archivo `.gitignore` para evitar subir `.venv/` al repositorio:

```gitignore
.venv/
```
