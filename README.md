# Planeador Didáctico · Cultura Digital I (Prepa 50 UAGro)

Aplicación de planeación para la Unidad de Aprendizaje Curricular **Cultura Digital I** (Plan 2023 NEM / MCCEMS). Genera planes de clase sesión por sesión, lleva el avance del semestre y trae un **banco de actividades ampliable por internet**.

## Qué contiene el repositorio

```
.
├── index.html              ← la aplicación (un solo archivo, abre en cualquier navegador)
└── data/
    └── activities.json     ← banco de actividades (edítalo para agregar más)
```

## Cómo publicarlo gratis con GitHub Pages

1. Crea una cuenta en https://github.com y un repositorio nuevo, por ejemplo `cultura-digital-1`.
2. Sube estos archivos respetando la carpeta `data/`.
3. En el repositorio entra a **Settings → Pages**.
4. En *Build and deployment* elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`, y guarda.
5. En 1–2 minutos GitHub te dará una dirección como:
   `https://TU-USUARIO.github.io/cultura-digital-1/`
   Esa es tu app en línea, lista para usar desde cualquier dispositivo.

## Cómo conectar la app al banco de actividades

1. Abre la app y entra a la pestaña **Banco**.
2. En el campo de URL pega la dirección **raw** de tu archivo `activities.json`:
   `https://raw.githubusercontent.com/TU-USUARIO/cultura-digital-1/main/data/activities.json`
3. Pulsa **Actualizar actividades**. Se descargan y quedan guardadas para usarlas sin conexión.

> Si abres la app dentro de un visor que bloquea internet, publícala en GitHub Pages (paso anterior) y la descarga funcionará sin problema.

## Cómo agregar tus propias actividades

Edita `data/activities.json` y añade objetos al arreglo `actividades`. Cada actividad necesita un **id único**:

```json
{
  "id": "u2-b7",
  "unidad": 2,
  "tema": "II.4 Presentaciones",
  "titulo": "Storytelling con datos",
  "tipo": "Proyecto",
  "duracion": 50,
  "herramienta": "Google Slides",
  "objetivo": "Contar una historia apoyada en una gráfica.",
  "pasos": ["Paso 1", "Paso 2", "Paso 3"],
  "evidencia": "Presentación con narrativa"
}
```

- `unidad`: 1, 2 o 3.
- `tipo`: Gamificación · Reto · Proyecto · Aula invertida · Colaborativo · Práctica guiada (puedes crear otros).
- La app combina por `id`: ids nuevos se **agregan**, ids repetidos se **actualizan**.

Guarda el archivo en GitHub y vuelve a pulsar **Actualizar actividades** en la app: las nuevas aparecerán al instante.

## Privacidad

La app no envía datos a ningún servidor: tus planes y tu avance se guardan en el propio dispositivo. La única conexión a internet es la descarga (de solo lectura) del archivo de actividades que tú indiques.

---
Elaboración: Lic. Jonatan Cervantes Juárez · Preparatoria No. 50 · UAGro · Ciclo 2025–2026.
