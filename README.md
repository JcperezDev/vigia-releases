# Vigía · instaladores

Aquí solo están los instaladores de Vigía. El código es privado.

## Instalar

1. Baja **Puente.exe** de la [última versión](https://github.com/JcperezDev/vigia-releases/releases/latest).
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
