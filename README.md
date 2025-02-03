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

## Installation

### Requirements
- **Minecraft 1.21+**
- **Paper-based server**

### Steps
1. Download `Lumen.jar` and place it in the `plugins` folder.
2. Start the server to generate the configuration files.
3. Adjust `config.yml` to your preferences.
4. Use `/lumen reload` to apply the changes.

(**Only newly placed** `Lumen Torch` and `Lumen Guard` **will have effects. Previously placed torches will not be affected unless removed and placed again.**)

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

## Instalación

### Requisitos
- **Minecraft 1.21+**
- **Servidor basado en Paper**

### Pasos
1. Descarga `Lumen.jar` y colócalo en la carpeta `plugins`.
2. Inicia el servidor para generar los archivos de configuración.
3. Ajusta `config.yml` según tus necesidades.
4. Usa `/lumen reload` para aplicar los cambios.

(Las antorchas `Lumen Torch` y `Lumen Guard` colocadas antes de aplicar la configuración no se verán afectadas. Para que adopten los nuevos ajustes, deben retirarse y volver a colocarse.)

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
