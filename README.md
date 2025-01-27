<details><summary>English</summary>

# Lumen
**Lumen** is a Minecraft plugin designed to add customizable lighting systems, anti-mob protection, and efficient command handling using Paper's APIs.

![Discord](https://img.shields.io/discord/1079917552588816484?label=Discord&logo=discord&logoColor=white&color=31FFA3&style=for-the-badge) ![](https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F%20by%20stargaze-31FFA3?style=for-the-badge)

![Banner Logo](https://cdn.modrinth.com/data/5WB5vvtt/images/35551de205d79fe92272a95c2af1123590fce1fa.png)
---

## Main Features

---

### **Paper**
<details><summary>Plugin</summary>

- **Compatibility with Paper servers**: Fully integrated with Paper APIs for optimal performance.
- **Custom Lighting System**:
    - Place light blocks dynamically with `/lumen light <range> <light_level> <include_skylight>` to configure size, intensity, and natural light inclusion.
- **Anti-Mob Torches**:
    - Protect areas from hostile mobs with the `Lumen Torch Anti-mob`.
- **Command Management**:
    - `/lumen undo <operation_id>`: Undo light placement based on operation ID or `last`.
    - `/lumen redo <operation_id>`: Redo previously removed lights using an operation ID.
    - `/lumen remove area <range>`: Remove lights within a specified range.
    - `/lumen remove operation <operation_id>`: Remove lights tied to a specific operation ID.
    - `/lumen clear confirm`: Remove all registered lights with a confirmation step.
    - `/lumen give <player> <torch_type> <quantity>`: Provide players with `Lumen Torch` or `Lumen Torch Anti-mob`.
    - `/lumen reload`: Reload plugin configuration and translations.
- **Multilingual Support**:
    - Add new translations by placing files in the `Translations` folder and specifying them in `config.yml`.
    - Supports both `es_es.yml` (Spanish) and `en_en.yml` (English).
</details>

---

<details><summary>Permissions</summary>

- **`lumen.light`**: Required to use `/lumen light`.
- **`lumen.cancel`**: Required to cancel ongoing light placement tasks.
- **`lumen.undo`**: Required to undo light placements.
- **`lumen.redo`**: Required to redo removed lights.
- **`lumen.remove`**: Required to remove lights.
- **`lumen.clear`**: Required to clear all lights.
- **`lumen.give`**: Required to give `Lumen Torch` and `Lumen Torch Anti-mob`.
- **`lumen.reload`**: Required to reload the plugin configuration and translations.

</details>

---

## Installation

### **Requirements**
- Minecraft 1.21+
- A Paper server for the plugin.

### Steps
1. Place the `Lumen.jar` in your `plugins` folder.
2. Start the server to generate config files.
3. Adjust `config.yml` to your preferences.
4. Use `/lumen reload` to apply changes without restarting.

---

## Usage

### **Players**
- Use torches to illuminate areas or protect from mobs.
- **Crafting Recipes**: Both `Lumen Torch` and `Lumen Torch Anti-mob` have unique crafting recipes accessible to all players.

### **Administrators**
- Manage lighting dynamically with commands:
    - `/lumen light <range> <light_level> <include_skylight>`: Place lights dynamically.
    - `/lumen undo <operation_id>`: Undo previous light placements.
    - `/lumen redo <operation_id>`: Redo removed light placements.
    - `/lumen remove area <range>`: Remove lights in a specific range.
    - `/lumen clear confirm`: Clear all registered lights.
    - `/lumen give <player> <torch_type> <quantity>`: Provide torches to players.
- Add new translations by placing files in the `Translations` folder and specifying them in `config.yml`.

---

## Key Classes

### **Core**
- `Lumen`: Main plugin class.
- `LumenCommandManager`: Manages command registrations.
- `TranslationHandler`: Handles multilingual support.

### **Lighting**
- `LightHandler`: Optimized light placement with batching.
- `ItemLightsHandler`: Manages lights associated with operations.

### **Items**
- `LumenItems`: Handles custom item creation and distribution.

### **Events**
- `TorchListener`: Manages `Lumen Torch` interactions.
- `MobListener`: Handles `Lumen Torch Anti-mob` effects.

---

## Support

If you encounter any issues or have questions, feel free to reach out. 😊

</details>

# Lumen
**Lumen** es un plugin de Minecraft diseñado para añadir sistemas de iluminación personalizados mediante comandos y mediante ítems, protección anti-mobs de la forma más eficiente posible.

![Discord](https://img.shields.io/discord/1079917552588816484?label=Discord&logo=discord&logoColor=white&color=31FFA3&style=for-the-badge) ![](https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F%20by%20stargaze-31FFA3?style=for-the-badge)

![Banner Logo](https://cdn.modrinth.com/data/5WB5vvtt/images/35551de205d79fe92272a95c2af1123590fce1fa.png)
---

## Características principales

---

### **Paper**
<details><summary>Plugin</summary>

- **Compatibilidad con servidores Paper**: Totalmente integrado con las APIs de Paper.
- **Sistema de Iluminación Personalizada**:
    - Coloca bloques de luz dinámicamente con `/lumen light <range> <light_level> <include_skylight>` para configurar tamaño, intensidad y luz natural.
- **Antorchas Anti-Mobs**:
    - Protege áreas contra mobs hostiles con la `Lumen Torch Anti-mob`.
- **Gestión de Comandos**:
    - `/lumen undo <operation_id>`: Deshaz colocaciones de luz por ID o usando `last`.
    - `/lumen redo <operation_id>`: Rehaz luces eliminadas previamente usando un ID de operación.
    - `/lumen remove area <range>`: Elimina luces en un rango especificado.
    - `/lumen remove operation <operation_id>`: Elimina luces asociadas a un ID de operación.
    - `/lumen clear confirm`: Elimina todas las luces registradas con confirmación.
    - `/lumen give <player> <torch_type> <quantity>`: Da antorchas `Lumen Torch` o `Lumen Torch Anti-mob` a jugadores.
    - `/lumen reload`: Recarga la configuración y las traducciones del plugin.
- **Soporte Multilingüe**:
    - Añade nuevas traducciones colocando archivos en la carpeta `Translations` y especificándolos en `config.yml`.
    - Soporte para `es_es.yml` (Español) y `en_en.yml` (Inglés).
</details>

---

<details><summary>Permisos</summary>

- **`lumen.light`**: Requerido para usar `/lumen light`.
- **`lumen.cancel`**: Requerido para cancelar tareas activas de colocación de luz.
- **`lumen.undo`**: Requerido para deshacer colocaciones de luz.
- **`lumen.redo`**: Requerido para rehacer luces eliminadas.
- **`lumen.remove`**: Requerido para eliminar luces.
- **`lumen.clear`**: Requerido para eliminar todas las luces.
- **`lumen.give`**: Requerido para dar antorchas `Lumen Torch` y `Lumen Torch Anti-mob`.
- **`lumen.reload`**: Requerido para recargar la configuración y traducciones del plugin.

</details>

---

## Instalación

### **Requisitos Previos**
- Minecraft 1.21+
- Un servidor Paper para el plugin.

### Pasos
1. Coloca `Lumen.jar` en tu carpeta `plugins`.
2. Inicia el servidor para generar los archivos de configuración.
3. Ajusta `config.yml` según tus preferencias.
4. Usa `/lumen reload` para aplicar cambios sin reiniciar.

---

## Uso

### **Jugadores**
- Usa antorchas para iluminar áreas o proteger de mobs.
- **Recetas de crafteo**: Tanto la `Lumen Torch` como la `Lumen Torch Anti-mob` tienen recetas únicas accesibles para los jugadores.

### **Administradores**
- Maneja iluminación dinámicamente con comandos:
    - `/lumen light <range> <light_level> <include_skylight>`: Coloca luces dinámicamente.
    - `/lumen undo <operation_id>`: Deshaz colocaciones previas de luz.
    - `/lumen redo <operation_id>`: Rehaz luces eliminadas.
    - `/lumen remove area <range>`: Elimina luces en un rango específico.
    - `/lumen clear confirm`: Elimina todas las luces registradas.
    - `/lumen give <player> <torch_type> <quantity>`: Proporciona antorchas a jugadores.
- Añade nuevas traducciones colocando archivos en la carpeta `Translations` y especificándolos en `config.yml`.

---

## Clases Clave

### **Core**
- `Lumen`: Clase principal del plugin.
- `LumenCommandManager`: Gestiona el registro de comandos.
- `TranslationHandler`: Maneja el soporte multilingüe.

### **Iluminación**
- `LightHandler`: Colocación optimizada de luces con procesamiento en lotes.
- `ItemLightsHandler`: Gestiona luces asociadas a operaciones.

### **Ítems**
- `LumenItems`: Maneja la creación y distribución de ítems personalizados.

### **Eventos**
- `TorchListener`: Gestiona interacciones con la `Lumen Torch`.
- `MobListener`: Maneja los efectos de la `Lumen Torch Anti-mob`.

---

## Soporte

Si encuentras algún problema o tienes preguntas, no dudes en contactarnos. 😊

---
