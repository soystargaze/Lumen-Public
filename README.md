# Lumen – Iluminación Avanzada para Minecraft

**Lumen** es un plugin para **Minecraft** diseñado para mejorar la calidad de vida en los servidores al optimizar la iluminación. Permite iluminar áreas de manera eficiente mediante comandos y ofrece ítems únicos:

- **Lumen Torch** – Ilumina el entorno automáticamente.
- **Lumen Guard** – Previene el spawn de mobs hostiles.

![Discord](https://img.shields.io/discord/1079917552588816484?label=Discord&logo=discord&logoColor=white&color=31FFA3&style=for-the-badge) ![](https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F%20by%20stargaze-31FFA3?style=for-the-badge)

![Banner Logo](https://cdn.modrinth.com/data/5WB5vvtt/images/35551de205d79fe92272a95c2af1123590fce1fa.png)

---

## Características

- **Compatibilidad con Paper** – Integración completa con la API de Paper.
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

- `/lumen light <range> <light_level> <include_skylight>` – Coloca luces dinámicamente.
- `/lumen undo <operation_id>` – Deshace colocaciones previas de luz.
- `/lumen redo <operation_id>` – Rehace luces eliminadas.
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

Si tienes dudas o encuentras algún problema, contáctanos.  