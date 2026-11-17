# Jasboot - descargas

Aqui se publican los instaladores de **Jasboot**, un lenguaje de programacion en espanol con memoria
neuronal asociativa integrada, compilador propio, maquina virtual y compilador nativo (AOT).

Este repositorio no contiene codigo: solo las versiones (`Releases`).

## Instalar (Windows 10/11, 64 bits)

1. Abre la ultima version en [Releases](../../releases) y descarga `Jasboot-Setup-X.Y.Z.exe`.
2. (Opcional) Comprueba la descarga: el hash SHA-256 del archivo debe coincidir con `SHA256SUMS.txt`
   (`Get-FileHash Jasboot-Setup-X.Y.Z.exe`).
3. Ejecuta el instalador. Por defecto instala solo para tu usuario y no pide administrador.
   Windows puede mostrar un aviso de SmartScreen porque el instalador aun no esta firmado:
   elige "Mas informacion" y "Ejecutar de todas formas".
4. Abre una consola nueva y prueba:

```
jb ejecutar hola.jasb        compila y ejecuta en la maquina virtual
jb nativo hola.jasb          genera hola.exe (necesita gcc/MinGW en el PATH)
```

El compilador nativo (AOT) necesita gcc; si no lo tienes, instala MinGW-w64 (por ejemplo WinLibs).
La maquina virtual y el compilador funcionan sin gcc.

## Extension de Visual Studio Code

El instalador la instala si encuentra `code`. Tambien puedes descargar `Jasboot-Extension-X.Y.Z.vsix` y usar
"Extensiones: Instalar desde VSIX".

## Versiones

`X.Y.Z` con cada numero de 0 a 99 (0.0.1 ... 0.0.99, 0.1.0 ...). Las versiones 0.x se marcan como preliminares.
