# Lumen
**Lumen** es un plugin de Minecraft enfocado en mejorar la QoL al optimizar la iluminación en los mundos. Permite iluminar áreas de manera eficiente con comandos y ofrece ítems fabricables únicos: la **Lumen Torch**, que ilumina el entorno, y la **Lumen Guard**, que bloquea el spawn de mobs hostiles.

![Discord](https://img.shields.io/discord/1079917552588816484?label=Discord&logo=discord&logoColor=white&color=31FFA3&style=for-the-badge) ![](https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F%20by%20stargaze-31FFA3?style=for-the-badge)

![Banner Logo](https://cdn.modrinth.com/data/5WB5vvtt/images/35551de205d79fe92272a95c2af1123590fce1fa.png)
---

## Características principales

---

### **Paper**
<details><summary>Resumen</summary>

- **Compatibilidad con servidores Paper**: Totalmente integrado con las API de Paper.
- **Sistema de Iluminación Personalizada**:
    - Coloca bloques de luz dinámicamente con `/lumen light <range> <light_level> <include_skylight>` para configurar tamaño, intensidad y luz natural.
- **Antorchas Anti-Mobs**:
    - Protege áreas contra mobs hostiles con la `Lumen Torch Guard`.
- **Antorcha auto-iluminadora**:
    - La `Lumen Torch` ilumina automáticamente áreas al ser colocada.
- **Soporte Multilingüe**:
    - Añade nuevas traducciones creando archivos en la carpeta `Translations` y activándolos en `config.yml` o mediante comandos.
    - Soporte para `es_es.yml`, `en_en.yml`, `fr_fr.yml`, `de_de.yml`, `it_it.yml` y `pt_br.yml`.
  
</details>

### **Integraciones (Recomendadas)**

<details><summary>CoreProtect</summary>
- Permite registrar las acciones de colocación y eliminación de luces. 
</details>

<details><summary>FastAsyncWorlEdit</summary>
- Aprovecha la API de FAWE para colocar bloques de luz de forma más rápida y eficiente. Se recomienda su uso para mejorar el rendimiento general del plugin.
</details>

---

### **Comandos y Permisos**

<details><summary>Comandos</summary>

- `/lumen light <range> <light_level> <include_skylight>`: Coloca luces dinámicamente.
- `/lumen undo <operation_id>`: Deshace colocaciones previas de luz.
- `/lumen redo <operation_id>`: Rehace luces eliminadas.
- `/lumen remove area <range>`: Elimina luces en un rango específico.
- `/lumen clear confirm`: Elimina todas las luces registradas.
- `/lumen give <all/player> <torch_type> <quantity>`: Proporciona antorchas a jugadores.
- `/lumen reload`: Recarga la configuración y traducciones del plugin.
- `/lumen lang <language>`: Cambia el idioma del plugin.

</details>

<details><summary>Permisos</summary>

- **`lumen.light`**: Requerido para usar `/lumen light`.
- **`lumen.cancel`**: Requerido para cancelar tareas activas de colocación de luz.
- **`lumen.undo`**: Requerido para deshacer colocaciones de luz.
- **`lumen.redo`**: Requerido para rehacer luces eliminadas.
- **`lumen.remove`**: Requerido para eliminar luces.
- **`lumen.clear`**: Requerido para eliminar todas las luces.
- **`lumen.give`**: Requerido para dar antorchas `Lumen Torch` y `Lumen Guard`.
- **`lumen.reload`**: Requerido para recargar la configuración y traducciones del plugin.
- **`lumen.lang`**: Requerido para cambiar el idioma del plugin.
- **`lumen.craft.torch`**: Requerido para craftear la `Lumen Torch`.
- **`lumen.craft.guard`**: Requerido para craftear la `Lumen Guard`.

</details>

---

## Instalación

### **Requisitos Previos**
- Minecraft 1.21+
- Un servidor basado en Paper.

### Pasos
1. Coloca `Lumen.jar` en tu carpeta `plugins`.
2. Inicia el servidor para generar los archivos de configuración.
3. Ajusta `config.yml` según tus preferencias.
4. Usa `/lumen reload` para recargar la configuración y traducciones.

---

## Uso

### **Jugadores**
- Se puede utilizar la `Lumen Torch` para iluminar un área de forma automática y la `Lumen Guard` para bloquear el spawn de mobs hostiles.
- Se necesita otorgar los permisos `lumen.craft.torch y lumen.craft.guard` para poder fabricar las antorchas.
- Si se quitan las antorchas, las luces y protecciones se eliminarán automáticamente de las zonas (No se pierde la antorcha por quitarla).
- **Recetas de crafteo**:
  <details><summary>Lumen Torch</summary>
  
  ![Lumen Torch Recipe](https://cdn.modrinth.com/data/5WB5vvtt/images/3cf389c35844ac90b2f07e8f7194913937712305.png)
  
  </details>
  <details><summary>Lumen Guard</summary>
    
  ![Lumen Guard Recipe](https://cdn.modrinth.com/data/5WB5vvtt/images/64419e0fbf155c4c1aad408f77c3083b2764da6a.png)
    
  </details>

### **Administradores**
- Maneja iluminación de forma eficiente con comandos:
    - `/lumen light <range> <light_level> <include_skylight>`: Coloca luces de una intensidad específica en un área.
    - `/lumen undo`: Deshace colocaciones previas de luz.
    - `/lumen redo`: Rehace luces eliminadas.
    - `/lumen remove area <range>`: Elimina luces en un rango específico.
    - `/lumen clear confirm`: Elimina todas las luces registradas en la base de datos y del mundo. (No se pueden recuperar).
    - `/lumen give <player> <torch_type> <quantity>`: Proporciona antorchas a jugadores.
- Añade nuevas traducciones colocando archivos en la carpeta `Translations` y especificándolos en `config.yml`.

---

## Soporte

Si encuentras algún problema o tienes preguntas, no dudes en contactarnos. 😊

---
