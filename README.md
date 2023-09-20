### Actualización de la BIOS

Este repositorio está diseñado para brindar una guía detallada sobre cómo actualizar la BIOS de tu placa base de manera segura y efectiva. La actualización de la BIOS puede ser crucial para mejorar el rendimiento, solucionar problemas de compatibilidad y mantener tu sistema al día. Sigue estos pasos para realizar una actualización exitosa:

**Paso 1: Obtener el Modelo de la Placa Base**
- Utiliza [CPU-Z](https://www.cpuid.com/softwares/cpu-z.html) u otras herramientas para obtener el modelo de tu placa base.

**Paso 2: Buscar y Descargar la Última Versión de la BIOS**
- Ingresa el nombre del modelo de la placa base en el buscador y dirígete al sitio web del fabricante.
- Ve a la sección de soporte de controladores/bios y descarga la última versión de la BIOS.

**Paso 3: Preparar el Pendrive**
- Formatea un pendrive en buen estado a formato FAT32.
- Descomprime el archivo de la BIOS descargado en el pendrive.

**Paso 4: Actualizar la BIOS**
- Reinicia tu PC y entra en la BIOS.
- Busca la opción de "flash" o similar en la configuración de la BIOS.
- Selecciona la opción para cargar o actualizar la BIOS.
- Selecciona el archivo de la BIOS desde el pendrive.
- Espera durante el proceso de actualización (la PC se reiniciará varias veces; NO LA TOQUES).

**Nota Importante:**
- Comprueba las características de tu placa base para ver si tiene dual BIOS. Si es así, sigue este procedimiento; de lo contrario, ten precaución.
- Si tu placa base tiene dual BIOS y la actualización falla por algún motivo, puedes volver a cargar la BIOS anterior, ya que el dual BIOS realiza un respaldo.


### Flasheo de BIOS de Tarjetas Gráficas

**Comandos para NVIDIA (nvflash):**

1. `nvflash(64/32) --protectoff`: Utiliza este comando antes de flashear una nueva BIOS. Deshabilita la protección de escritura en la BIOS de la tarjeta gráfica para permitir el proceso de flasheo.

2. `nvflash(64/32) -6 Nombre de la BIOS.rom`: Ejecuta este comando para flashear la nueva BIOS en la tarjeta gráfica. Asegúrate de reemplazar "Nombre de la BIOS.rom" con el nombre del archivo de la BIOS que deseas instalar.

3. `nvflash(64/32) --protecton`: Después de completar el flasheo, utiliza este comando para volver a habilitar la protección de escritura en la BIOS.

**Comandos para AMD (AMDVBFlash):**

1. `AMDVBFlash.exe -f -p 0 Nombre de la BIOS.rom`: Este comando se utiliza para flashear la BIOS en tarjetas gráficas AMD. Reemplaza "Nombre de la BIOS.rom" con el nombre del archivo de la BIOS que deseas instalar. El "-p 0" se refiere al número de dispositivo, que puede variar según tu configuración.

**Herramientas de Descarga:**

- [VGA Bios Collection](https://www.techpowerup.com/vgabios/): Una colección de BIOS de tarjetas gráficas NVIDIA y AMD que puedes utilizar como referencia o descargar para flashear.

- [NVIDIA NVFlash - TechPowerUp](https://www.techpowerup.com/download/nvidia-nvflash/): Descarga la última versión de NVFlash para flashear tarjetas gráficas NVIDIA.

- [AMDVBFlash - ATI ATIFlash  - TechPowerUp](https://www.techpowerup.com/download/ati-atiflash/): Descarga AMDVBFlash (ATI ATIFlash) para flashear tarjetas gráficas AMD.

### Cuándo Utilizar Estos Comandos:**
Utiliza estos comandos y herramientas cuando desees actualizar la BIOS de tu tarjeta gráfica para solucionar problemas de compatibilidad, mejorar el rendimiento o personalizar la configuración. El flasheo de la BIOS conlleva riesgos, así que asegúrate de respaldar tu BIOS actual y sigue cuidadosamente las instrucciones proporcionadas por el fabricante de tu tarjeta gráfica. Ten en cuenta que el flasheo incorrecto puede dejar tu tarjeta inoperable y afectar la garantía, así que úsalo bajo tu propio riesgo y responsabilidad.

Mantén tu sistema actualizado y optimizado siguiendo estos pasos cuidadosamente para actualizar la BIOS de manera segura.

## Licencia
Este proyecto está bajo la licencia [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/). Puedes compartir, adaptar y utilizar estos archivos siempre que des el crédito correspondiente al autor original.
