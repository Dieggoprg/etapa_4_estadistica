
# Etapa 4: Contrastación de Datos - Trabajo Integrador

Este documento detalla el desarrollo de la **Cuarta Etapa** del trabajo integrador, enfocado en el análisis estadístico descriptivo del consumo diario de redes sociales en estudiantes.

## 📋 Descripción del Problema
Se analizan los datos recolectados en una encuesta sobre la cantidad de horas diarias de uso de redes sociales durante el último mes en un grupo numeroso de estudiantes. 

El objetivo principal es procesar la variable **"Cantidad de horas de consumo de redes sociales por día"** mediante Python para construir una tabla de frecuencias completa y calcular medidas de resumen que permitan contrastar estos resultados con las etapas previas del proyecto.

## 🚀 Requisitos y Configuración del Entorno
Este análisis está desarrollado en un **Jupyter Notebook** (`.ipynb`). Para ejecutarlo localmente, necesitas tener instalado Python en tu sistema. A continuación, se detallan las instrucciones según tu sistema operativo:

### 🪟 Para usuarios de Windows
1. Asegúrate de tener Python instalado (puedes descargarlo desde python.org). Al instalarlo, asegúrate de marcar la casilla **"Add Python to PATH"**.
2. Abre la consola de comandos (**CMD** o **PowerShell**).
3. Instala las librerías necesarias ejecutando:
   ```cmd
   pip install jupyter pandas numpy openpyxl

   Para abrir el entorno, navega hasta la carpeta donde guardaste este archivo y ejecuta:
```cmd
  jupyter notebook

🐧 Para usuarios de Linux (Debian/Ubuntu)

    Abre tu terminal.

    Actualiza los repositorios e instala Python, pip y la herramienta para entornos virtuales (recomendado en Linux para evitar conflictos de sistema):
    ```Bash
      sudo apt update
      sudo apt install python3 python3-pip python3-venv
```Bash
    Crea y activa un entorno virtual en la carpeta de tu proyecto:
    ```Bash
      python3 -m venv mi_entorno
      source mi_entorno/bin/activate

    Instala las dependencias dentro del entorno virtual:
    ```Bash
      pip install jupyter pandas numpy openpyxl
```Bash
    Inicia Jupyter Notebook ejecutando:
    ```Bash
      jupyter notebook
```Bash
### Nota general:
  También puedes subir este notebook junto con el archivo Excel a plataformas en la nube como Google Colab y ejecutarlo directamente en el navegador sin necesidad de instalar ni configurar     nada en tu computadora.

##🛠️ Estructura del Notebook

El código está dividido en celdas lógicas para facilitar su lectura y ejecución paso a paso:

    Importación y Carga de datos: Lectura del archivo Excel proporcionado.

    Construcción de la Tabla de Frecuencias:

        Frecuencia Absoluta: Conteo de estudiantes por cantidad de horas.

        Frecuencia Relativa: Proporción de estudiantes respecto al total.

        Frecuencias Acumuladas: Suma progresiva de las frecuencias absolutas y relativas.

    Cálculo de Medidas de Resumen:

        Media Aritmética: Promedio de horas de consumo en el grupo estudiado.

        Desviación Estándar: Grado de dispersión de las horas de consumo respecto a la media.

###💻 Instrucciones de Uso

    Asegúrate de que el archivo de datos de Excel (ej. datos.xlsx) esté guardado en la misma carpeta que este Notebook (o súbelo al entorno si usas Google Colab).

    Verifica que el nombre del archivo y la columna coincidan en la celda de carga de datos:
    ```cmd
      df = pd.read_excel("nombre_del_archivo.xlsx")
      horas = df["Cantidad de horas de redes sociales por día"]
```cmd
    Ejecuta las celdas en orden secuencial.

📊 Resultados Esperados

Al ejecutar las celdas de resultados, se imprimirá la tabla de frecuencias estructurada en un formato tabular limpio, seguida de los valores de la Media y la Desviación Estándar. Estos datos servirán como base para la interpretación y contrastación final en el informe del trabajo integrador.
