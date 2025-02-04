<details><summary>English</summary>

# Lumen – Advanced Lighting for Minecraft

**Lumen** is a **Minecraft** plugin designed to enhance server quality of life by optimizing lighting. It allows efficient area illumination using commands and offers unique items:

- **Lumen Torch** – Automatically lights up the surroundings.
- **Lumen Guard** – Prevents hostile mobs from spawning.

![Discord](https://img.shields.io/discord/1079917552588816484?label=Discord&logo=discord&logoColor=white&color=31FFA3&style=for-the-badge) ![](https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F%20by%20stargaze-31FFA3?style=for-the-badge)

![Banner Logo](https://cdn.modrinth.com/data/5WB5vvtt/images/ed1c78a69e6aba737ccc687acc242140fcce6299.png)

---

## Features

- **Paper Compatibility** – Full integration with the Paper API.
- **Multiple command aliases** – Use `/lumen`, `/lu`, and `/l` for convenience.
- **Customizable Lighting** – Use `/lumen light <range> <light_level> <include_skylight>` to adjust size, intensity, and natural light inclusion.
- **Mob Protection** – Prevents hostile mob spawning with the `Lumen Guard`.
- **Auto-Lighting Torch** – The `Lumen Torch` automatically lights up when placed.
- **Multilingual Support** – Available translations: `es_es.yml`, `en_en.yml`, `fr_fr.yml`, `de_de.yml`, `it_it.yml`, `pt_br.yml`. Custom languages can be added.

---

## Compatible Integrations

Lumen can leverage other tools to enhance performance and functionality:

- **CoreProtect** – Logs light placements and removals, allowing rollbacks and audits.
- **FastAsyncWorldEdit (FAWE)** – Optimizes light block placement through commands and the Lumen Torch, improving server performance.

These integrations are optional but recommended for better control and efficiency.

---

## Installation Guide

<details><summary>Installation></summary$
    
## **Prerequisites**  
Before installing Lumen, make sure your server meets the following requirements:

- **Minecraft Server:** PaperMC **1.21 or higher** (recommended **1.21.4**, the latest stable version).  
- **Java:** Version **21 or higher**.  
- **Write permissions:** The server must have permission to write in its plugins directory.  
- **Internet connection:** Required to verify the license via the Polymart API.  
- **Optional Dependencies:**  
  - **CoreProtect (Optional):** Enables tracking and rollback of placed or removed lights. Integration can be verified in the console upon server startup.  
  - **FastAsyncWorldEdit (Optional):** Optimizes performance for placing and removing large amounts of lights.  

---

## **Step 1: Download the Plugin**  
Download the latest version of Lumen from [Polymart](https://polymart.org) and ensure you obtain a valid `.jar` file.  

---

## **Step 2: Installation**  
1. **Upload the file** `Lumen.jar` to the `plugins/` folder of your PaperMC server.  
2. **Restart the server** to automatically generate the configuration files.  
3. **Verify installation** by checking the console. If the installation was successful, you will see a message indicating that the plugin has been loaded correctly.  

---

## **Step 3: Initial Configuration**  
1. **Navigate to the configuration folder:** `plugins/Lumen/`  
2. **Edit `config.yml`** to adjust performance settings, such as:  
   - `command_lights_per_tick`: Number of lights added per tick when using commands.  
   - `torch_lights_per_tick`: Number of lights added per tick when using torches.  
   - `torch_tick_interval`: Interval between torch ticks.  
   - `mob_torch_radius`: Protection radius of the anti-mob torch.  
3. **If using CoreProtect,** check the server console on startup. If integration is successful, you will see a message indicating that CoreProtect has been detected and is active in Lumen.  
4. **If using FastAsyncWorldEdit,** ensure it is installed and properly configured to optimize the placement and removal of lights.  

---

## **Step 4: License Verification**  
Lumen requires an internet connection to verify the purchase via the Polymart API. **If your server does not have internet access, the plugin will not work.**  
To avoid issues:  
- Ensure the server can make outgoing HTTP requests.  
- Do not block connections to `api.polymart.org` in your firewall.  

---

## **Step 5: Troubleshooting**  
- **The plugin does not load:** It is recommended to use **PaperMC 1.21.4**, the latest stable version. Also, ensure you are using Java 21 or higher.  
- **License verification failed:** Confirm that the server has internet access and check the console for error messages.  
- **CoreProtect errors:** Check the console when starting the server. If integration does not activate, ensure CoreProtect is correctly installed.  
- **Low performance when placing lights:** Adjust values in `config.yml` and/or install **FastAsyncWorldEdit** to optimize large-scale block processing.  
- Only newly placed `Lumen Torch` and `Lumen Guard` will have effects of changes in config.yml. Previously placed torches will not be affected unless removed and placed again.

---

## **Support & Contact**  
If you encounter issues or have questions, contact support on **[Discord](https://erosmari.com/discord)** or refer to the official plugin documentation.

</details>

---

## Commands & Permissions

<details>
<summary>Commands</summary>

Lumen also provides a variety of aliases for each command `/lumen`, `/lu`, and `/l`.

- `/lumen light <range> <light_level> <include_skylight>` – Places lights dynamically.
- `/lumen undo` – Undoes previous light placements.
- `/lumen redo` – Redoes removed lights.
- `/lumen remove area <range>` – Removes lights in a specified area.
- `/lumen clear confirm` – Clears all registered lights.
- `/lumen give <player/all> <torch_type> <quantity>` – Gives torches to players.
- `/lumen reload` – Reloads configuration and translations.
- `/lumen lang <language>` – Changes the plugin language.

</details>

<details>
<summary>Permissions</summary>

- `lumen.light` – Permission to use `/lumen light`.
- `lumen.cancel` – Permission to cancel active tasks.
- `lumen.undo` – Permission to undo placements.
- `lumen.redo` – Permission to redo removed lights.
- `lumen.remove` – Permission to remove lights.
- `lumen.clear` – Permission to clear all lights.
- `lumen.give` – Permission to give `Lumen Torch` and `Lumen Guard`.
- `lumen.reload` – Permission to reload configuration and translations.
- `lumen.lang` – Permission to change the language.
- `lumen.craft.torch` – Permission to craft the `Lumen Torch`.
- `lumen.craft.guard` – Permission to craft the `Lumen Guard`.

</details>

---

## Usage

### For Players
- The `Lumen Torch` automatically lights up nearby areas.
- The `Lumen Guard` prevents mob spawning within its range.
- Torches can be removed without being lost, and their effects disappear when removed.
- To craft them, you need `lumen.craft.torch` and `lumen.craft.guard` permissions.

**Crafting Recipes**
<details>
<summary>Lumen Torch</summary>

![Lumen Torch Recipe](https://cdn.modrinth.com/data/5WB5vvtt/images/3cf389c35844ac90b2f07e8f7194913937712305.png)

</details>
<details>
<summary>Lumen Guard</summary>

![Lumen Guard Recipe](https://cdn.modrinth.com/data/5WB5vvtt/images/64419e0fbf155c4c1aad408f77c3083b2764da6a.png)

</details>

---

### For Administrators
- Advanced light management using commands.
- Safe light removal with `/lumen remove` and `/lumen clear confirm`.
- Item distribution using `/lumen give`.
- Full customization through `config.yml` and translation files in `Translations/`.

---

## Support

If you have any questions or encounter issues, feel free to contact us on [Discord](https://erosmari.com/discord)

</details>

# Lumen – Iluminación Avanzada para Minecraft

**Lumen** es un plugin para **Minecraft** diseñado para mejorar la calidad de vida en los servidores al optimizar la iluminación. Permite iluminar áreas de manera eficiente mediante comandos y ofrece ítems únicos:

- **Lumen Torch** – Ilumina el entorno automáticamente.
- **Lumen Guard** – Previene el spawn de mobs hostiles.

![Discord](https://img.shields.io/discord/1079917552588816484?label=Discord&logo=discord&logoColor=white&color=31FFA3&style=for-the-badge) ![](https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F%20by%20stargaze-31FFA3?style=for-the-badge)

![Banner Logo](https://cdn.modrinth.com/data/5WB5vvtt/images/ed1c78a69e6aba737ccc687acc242140fcce6299.png)

---

## Características

- **Compatibilidad con Paper** – Integración completa con la API de Paper.
- **Múltiples Alias de Comandos** – Usa `/lumen`, `/lu`, y `/l` para mayor comodidad.
- **Iluminación Personalizada** – Usa `/lumen light <range> <light_level> <include_skylight>` para personalizar el tamaño, intensidad y luz natural.
- **Protección contra Mobs** – Evita el spawn de mobs hostiles con la `Lumen Guard`.
- **Antorcha Auto-Iluminadora** – La `Lumen Torch` ilumina automáticamente al colocarse.
- **Soporte Multilingüe** – Traducciones disponibles en `es_es.yml`, `en_en.yml`, `fr_fr.yml`, `de_de.yml`, `it_it.yml`, `pt_br.yml`. Se pueden añadir idiomas personalizados.

---

## Integraciones Compatibles

Lumen puede aprovechar otras herramientas para mejorar su rendimiento y funcionalidad:

- **CoreProtect** – Registra la colocación y eliminación de luces, permitiendo realizar rollbacks y auditorías.
- **FastAsyncWorldEdit (FAWE)** – Optimiza la colocación de bloques de luz generados por comandos y por la Lumen Torch, mejorando el rendimiento del servidor.

Estas integraciones son opcionales, pero recomendadas para un mejor control y eficiencia.

---

## Guía de Instalación

<details><summary>Instalación</summary>

## **Requisitos Previos**  
Antes de instalar Lumen, asegúrate de que tu servidor cumple con los siguientes requisitos:

- **Servidor Minecraft:** PaperMC **1.21 o superior** (recomendado **1.21.4**, la última versión estable).  
- **Java:** Versión **21 o superior**.  
- **Permisos de escritura:** El servidor debe tener permisos para escribir en su directorio de plugins.  
- **Conexión a Internet:** Obligatoria para verificar la licencia a través de la API de Polymart.  
- **Dependencias Opcionales:**  
  - **CoreProtect (Opcional):** Permite rastrear y restaurar luces colocadas o eliminadas. La integración puede verificarse en la consola al iniciar el servidor.  
  - **FastAsyncWorldEdit (Opcional):** Optimiza el rendimiento en la colocación y eliminación de grandes cantidades de luces.  

---

## **Paso 1: Descargar el Plugin**  
Descarga la última versión de Lumen desde [Polymart](https://polymart.org) y asegúrate de obtener un archivo `.jar` válido.  

---

## **Paso 2: Instalación**  
1. **Sube el archivo** `Lumen.jar` a la carpeta `plugins/` de tu servidor PaperMC.  
2. **Reinicia el servidor** para generar automáticamente los archivos de configuración.  
3. **Verifica la instalación** revisando la consola. Si la instalación fue exitosa, verás un mensaje indicando que el plugin se ha cargado correctamente.  

---

## **Paso 3: Configuración Inicial**  
1. **Accede a la carpeta de configuración:** `plugins/Lumen/`  
2. **Edita `config.yml`** para ajustar los parámetros de rendimiento, como:  
   - `command_lights_per_tick`: Cantidad de luces añadidas por tick al usar comandos.  
   - `torch_lights_per_tick`: Cantidad de luces añadidas por tick al usar antorchas.  
   - `torch_tick_interval`: Intervalo entre ticks de las antorchas.  
   - `mob_torch_radius`: Radio de protección de la antorcha anti-mobs.  
3. **Si usas CoreProtect,** revisa la consola del servidor al iniciar. Si la integración es exitosa, verás un mensaje indicando que CoreProtect ha sido detectado y está activo en Lumen.  
4. **Si usas FastAsyncWorldEdit,** asegúrate de que está instalado y configurado correctamente para optimizar la colocación y eliminación de luces.  

---

## **Paso 4: Verificación de Licencia**  
Lumen requiere una conexión a Internet para verificar la compra a través de la API de Polymart. **Si tu servidor no tiene acceso a Internet, el plugin no funcionará.**  
Para evitar problemas:  
- Asegúrate de que el servidor puede realizar peticiones HTTP salientes.  
- No bloquees conexiones a `api.polymart.org` en tu firewall.  

---

## **Paso 5: Solución de Problemas**  
- **El plugin no se carga:** Se recomienda usar **PaperMC 1.21.4**, la última versión estable. Asegúrate también de estar utilizando Java 21 o superior.  
- **No se puede verificar la licencia:** Confirma que el servidor tiene acceso a Internet y revisa la consola para mensajes de error.  
- **Errores con CoreProtect:** Revisa la consola al iniciar el servidor. Si la integración no se activa, asegúrate de que CoreProtect está correctamente instalado.  
- **Bajo rendimiento al colocar luces:** Ajusta los valores en `config.yml` y/o instala **FastAsyncWorldEdit** para optimizar el procesamiento de grandes cantidades de bloques.  
- Solo las **nuevas** `Lumen Torch` y `Lumen Guard` colocadas tendrán efecto con los cambios realizados en `config.yml`. Las antorchas previamente colocadas no se verán afectadas a menos que se eliminen y se vuelvan a colocar.  

---

## **Soporte y Contacto**  
Si tienes problemas o dudas, contacta con el soporte en **[Discord](https://erosmari.com/discord)** o consulta la documentación oficial del plugin.

</details>

---

## Comandos y Permisos

<details>
<summary>Comandos</summary>

Luemen también ofrece una variedad de alias para cada comando `/lumen`, `/lu`, y `/l`.

- `/lumen light <range> <light_level> <include_skylight>` – Coloca luces dinámicamente.
- `/lumen undo` – Deshace colocaciones previas de luz.
- `/lumen redo` – Rehace luces eliminadas.
- `/lumen remove area <range>` – Elimina luces en un área específica.
- `/lumen clear confirm` – Elimina todas las luces registradas.
- `/lumen give <player/all> <torch_type> <quantity>` – Da antorchas a jugadores.
- `/lumen reload` – Recarga la configuración y traducciones.
- `/lumen lang <language>` – Cambia el idioma del plugin.

</details>

<details>
<summary>Permisos</summary>

- `lumen.light` – Permiso para usar `/lumen light`.
- `lumen.cancel` – Permiso para cancelar tareas activas.
- `lumen.undo` – Permiso para deshacer colocaciones.
- `lumen.redo` – Permiso para rehacer luces eliminadas.
- `lumen.remove` – Permiso para eliminar luces.
- `lumen.clear` – Permiso para eliminar todas las luces.
- `lumen.give` – Permiso para dar antorchas `Lumen Torch` y `Lumen Guard`.
- `lumen.reload` – Permiso para recargar configuración y traducciones.
- `lumen.lang` – Permiso para cambiar el idioma.
- `lumen.craft.torch` – Permiso para fabricar la `Lumen Torch`.
- `lumen.craft.guard` – Permiso para fabricar la `Lumen Guard`.

</details>

---

## Uso

### Para Jugadores
- La `Lumen Torch` ilumina automáticamente áreas cercanas.
- La `Lumen Guard` bloquea el spawn de mobs hostiles en su radio de acción.
- Las antorchas pueden retirarse sin perderlas, y sus efectos desaparecen al hacerlo.
- Para fabricarlas, es necesario tener los permisos `lumen.craft.torch` y `lumen.craft.guard`.

**Recetas de Crafteo**
<details>
<summary>Lumen Torch</summary>

![Lumen Torch Recipe](https://cdn.modrinth.com/data/5WB5vvtt/images/3cf389c35844ac90b2f07e8f7194913937712305.png)

</details>
<details>
<summary>Lumen Guard</summary>

![Lumen Guard Recipe](https://cdn.modrinth.com/data/5WB5vvtt/images/64419e0fbf155c4c1aad408f77c3083b2764da6a.png)

</details>

---

### Para Administradores
- Gestión de iluminación con comandos avanzados.
- Eliminación segura de luces con `/lumen remove` y `/lumen clear confirm`.
- Distribución de ítems con `/lumen give`.
- Personalización total con `config.yml` y archivos de traducción en `Translations/`.

---

## Soporte

Si tienes dudas o encuentras algún problema, contáctanos por [Discord](https://erosmari.com/discord)
