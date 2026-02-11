# TallerControl (Web + Escritorio + iPhone)

Aplicación basada en tu diseño de **TallerControl** para gestionar OTs, repuestos y costos.

## Stack
- Vite + JavaScript vanilla.
- PWA (instalable en navegador/escritorio).
- Capacitor para empaquetado iPhone (iOS).

## Uso rápido
```bash
npm install
npm run dev
```

## Build web
```bash
npm run build
npm run preview
```

## Instalar como app de escritorio
1. Levanta la app en producción (`npm run build && npm run preview`) o en `npm run dev`.
2. En Chrome/Edge abre la URL de la app.
3. Usa **Instalar aplicación** desde la barra de direcciones.

## iPhone (app instalable)

### Opción 1: PWA (sin App Store)
- Abre la URL desde Safari.
- Compartir → **Agregar a pantalla de inicio**.

### Opción 2: App nativa iOS con Capacitor
```bash
npm run build
npx cap add ios
npx cap sync ios
npx cap open ios
```
Luego compilas y firmas desde Xcode.

## Persistencia
- Se guarda localmente en `localStorage` del dispositivo/navegador.
