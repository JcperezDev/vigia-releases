# Vigía · instaladores

![Descargas](https://img.shields.io/github/downloads/JcperezDev/vigia-releases/total?label=descargas&color=6d5bd0)
![Última versión](https://img.shields.io/github/v/release/JcperezDev/vigia-releases?label=versi%C3%B3n)

Aquí solo están los instaladores de Vigía. El código es privado. Web: https://jcperezdev.github.io/vigia-releases/

Vigía es gratis: no tiene cuenta, anuncios ni versión de pago. No envía datos tuyos; el número de descargas sale de los contadores públicos de GitHub.

## Instalar

1. Baja **[Vigia-Setup.exe](https://github.com/JcperezDev/vigia-releases/releases/latest/download/Vigia-Setup.exe)** (es Puente, el instalador).
2. Ábrelo. Te pide permiso de administrador porque Vigía lo necesita para leer sensores y aplicar ajustes.
3. Puente descarga Vigía, comprueba la firma y crea los accesos en el Escritorio y en Inicio.

## Actualizar

Vigía avisa abajo a la izquierda cuando hay una versión nueva. Con **Actualizar** se cierra, Puente instala la nueva y la vuelve a abrir.
También puedes abrir «Puente (actualizar Vigia)» desde el menú Inicio.

## Volver a la versión anterior

```
"%LOCALAPPDATA%\Programs\Vigia-Puente\Puente.exe" --rollback
```

## Quitar

```
"%LOCALAPPDATA%\Programs\Vigia-Puente\Puente.exe" --uninstall
```

Tus ajustes y las copias de lo que cambió Vigía se quedan en `%LOCALAPPDATA%\Vigia`.

## Firma

Cada versión trae un `.sig` por archivo (ECDSA P-256 / SHA-256). Puente lleva dentro la clave pública y no instala nada cuya firma no cuadre.
