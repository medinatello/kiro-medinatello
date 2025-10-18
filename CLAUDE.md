# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Proyecto

Extensión de tema de color para VS Code. **Orquídea Morada** - tema venezolano inspirado en orquídeas moradas (flor nacional). Dos variantes: dark y light.

## Comandos

```bash
# Probar extensión
F5  # Abre ventana de desarrollo con el tema cargado

# Empaquetar
vsce package

# Publicar
vsce publish
```

## Estructura

```
themes/
├── orquidea-morada-dark-theme.json   # Tema oscuro
└── orquidea-morada-light-theme.json  # Tema claro
```

Archivos JSON con:
- `colors`: Colores de UI (editor, sidebar, statusbar, etc.)
- `tokenColors`: Colores de sintaxis (scopes TextMate)
- `semanticTokenColors`: Coloreado semántico

## Paleta Base

**Dark**: `#2D1B3D` (fondo) · `#E9E7F1` (texto) · `#B366FF` (acento)
**Light**: `#FDFCFF` (fondo) · `#2D1B3D` (texto) · `#8E5BFF` (acento)

## Identidad

Mantener coherencia morada/violeta en modificaciones. La paleta representa elegancia y fortaleza de las orquídeas venezolanas.

## Requisitos

- VS Code ^1.103.0 o superior
- Para publicar: Personal Access Token de Azure DevOps con permisos de Marketplace
