# Librerías Open Source para el sistema Impulso

Este documento lista bibliotecas de código abierto útiles para los distintos módulos del sistema **Impulso**. Los comandos de ejemplo están pensados para Termux o Pydroid 3 en Android. Revise siempre la licencia de cada proyecto para confirmar su compatibilidad con la filosofía de software libre y ético de Impulso.

Las carpetas clonadas o archivos descargados se recomienda almacenarlos en:

```
/storage/emulated/0/OneDrive/Impulso/Libs_OpenSource
```

así podrá conservar una copia local de todo el código.

## Automatización en Android con Python y Bash

```bash
# Acceso a funciones del dispositivo desde Termux
pkg install termux-api
pip install termux-api

# Bibliotecas Python para automatizar scripts
pip install pexpect sh colorama

# Guardar copia del código fuente
git clone https://github.com/termux/termux-api.git \
  /storage/emulated/0/OneDrive/Impulso/Libs_OpenSource/termux-api
```

## Simulación de lógica de PLC industrial

```bash
# OpenPLC es un entorno de PLC libre
git clone https://github.com/thiagoralves/OpenPLC_v3.git \
  /storage/emulated/0/OneDrive/Impulso/Libs_OpenSource/OpenPLC_v3

# Bibliotecas para comunicarse con PLC Siemens o Allen Bradley
pip install python-snap7 pylogix
```

## Inteligencia Artificial distribuida

```bash
# Framework para ejecutar modelos en paralelo
pip install ray

# Biblioteca de modelos abiertos (incluye modelos como Mistral)
pip install transformers accelerate

# Opciones para correr modelos locales
git clone https://github.com/ggerganov/llama.cpp.git \
  /storage/emulated/0/OneDrive/Impulso/Libs_OpenSource/llama.cpp

git clone https://github.com/nomic-ai/gpt4all.git \
  /storage/emulated/0/OneDrive/Impulso/Libs_OpenSource/gpt4all
```

_Nota: ChatGPT, Gemini y Copilot no son proyectos de código abierto; para usarlos se necesitan sus servicios oficiales._

## Visualización de datos y dashboards

```bash
pip install pandas matplotlib seaborn plotly dash openpyxl xlsxwriter
```

## Procesamiento de lenguaje natural y análisis semántico

```bash
pip install nltk spacy gensim scikit-learn sympy
```

## Trazabilidad de eventos y estructuras hash para Excel

```bash
pip install pandas openpyxl loguru
# hashlib viene incluido en la biblioteca estándar de Python
```

## Sincronización y gestión de archivos en OneDrive y Google Drive

```bash
# Herramienta CLI de sincronización (OneDrive, Google Drive, etc.)
pkg install rclone

# Bibliotecas específicas en Python
pip install PyDrive2 onedrivesdk

git clone https://github.com/rclone/rclone.git \
  /storage/emulated/0/OneDrive/Impulso/Libs_OpenSource/rclone
```

Estas bibliotecas y herramientas son de código abierto y pueden combinarse para desarrollar los diferentes módulos de Impulso en Android. Conserve las copias descargadas en la carpeta indicada para tener una referencia local siempre disponible.
