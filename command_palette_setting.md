# Configuración para Centrar la Paleta de Comandos

Para centrar la paleta de comandos en Visual Studio Code (como en Cursor o Kiro), necesitas modificar tu archivo de configuración `settings.json`.

## Instrucciones

1.  Abre la Paleta de Comandos en VS Code (puedes usar `Cmd+Shift+P` en macOS o `Ctrl+Shift+P` en Windows/Linux).
2.  Busca el comando **"Preferences: Open User Settings (JSON)"** y selecciónalo.
3.  Esto abrirá tu archivo `settings.json`. Añade la siguiente línea dentro del objeto JSON principal:

```json
{
  // ... otras configuraciones que ya tengas
  "workbench.commandPalette.experimental.layout": "horizontal"
}
```

Guarda el archivo y la paleta de comandos aparecerá ahora en el centro de la pantalla cada vez que la invoques.
