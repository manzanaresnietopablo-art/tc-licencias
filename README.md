# Licencias de TimeController

Un fichero por empresa con el estado de su servicio. Los programas instalados
lo consultan al arrancar para saber si siguen dados de alta.

- El nombre de cada fichero es un **resumen** del nombre de la empresa, no el
  nombre: esta carpeta no revela la cartera de clientes.
- El contenido va **firmado** (Ed25519). Nadie puede fabricar un «cortado» ni
  un «al día», ni reutilizar el de una empresa en otra, porque hace falta una
  clave privada que no está aquí.

Por eso este repositorio puede ser público sin ningún problema: es información
firmada y anónima, no un secreto.

Los ficheros los escribe `emitir_licencia.py --publicar`, que además hace el
commit y los sube.
