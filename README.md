# Lumen
**Lumen** es un plugin de Minecraft enfocado en mejorar la QoL al optimizar la iluminación en los mundos. Permite iluminar áreas de manera eficiente con comandos y ofrece ítems fabricables únicos: la **Lumen Torch**, que ilumina el entorno, y la **Lumen Guard**, que bloquea el spawn de mobs hostiles.

![Discord](https://img.shields.io/discord/1079917552588816484?label=Discord&logo=discord&logoColor=white&color=31FFA3&style=for-the-badge) ![](https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F%20by%20stargaze-31FFA3?style=for-the-badge)

![Banner Logo](https://cdn.modrinth.com/data/5WB5vvtt/images/35551de205d79fe92272a95c2af1123590fce1fa.png)
---

## Características principales

---

### **Paper**
<details><summary>Plugin</summary>

- **Compatibilidad con servidores Paper**: Totalmente integrado con las API de Paper.
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
