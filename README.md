# OVERTHEWIRE (NATAS)

## LEVEL 0 -> 1
### Solucion
```bash
ll  # Para ver carpetas ocultas
cd .backup  # Para direccionarse a esa carpeta
grep leviathan1 bookmarks.html  # Para buscar la contraseña
```

**Contrasenia:**
```bash
3QJ3TgzHDq
```

---
## LEVEL 1 -> 2
### Solucion

Para este nivel ingresamos a `check` y nos pide una contraseña. Como no la tenemos, usamos:
```bash
ltrace ./check
```
Aqui encontramos la contrasenia para ingresar a `./check`. Una vez dentro, obtenemos la contrasenia del siguiente nivel con:
```bash
cat /etc/leviathan_pass/leviathan2
```

**Contrasenia:**
```bash
NsN1HwFoyN
```

---
## LEVEL 2 -> 3
### Solucion

Este nivel se resolvio con ayuda... :v

**Contrasenia:**
```bash
f0n8h2iWLP
```

---
## LEVEL 3 -> 4
### Solucion

Similar al nivel 2, utilizamos:
```bash
ltrace ./level3
cat /etc/leviathan_pass/leviathan4
```
Para obtener la contrasenia.

**Contrasenia:**
```bash
WG1egElCvO
```

---
## LEVEL 4 -> 5
### Solucion

Nos dirigimos al directorio `.trash`, luego a `.bin`, donde se nos entrega una cadena binaria. Con ayuda de CyberChef la decodificamos para obtener la contrasenia del proximo nivel.

**Contrasenia:**
```bash
0dyxT7F4QD
```

---
## LEVEL 5 -> 6
### Solución

Ejecutamos:
```bash
./leviathan5  # Parece ser un ejecutable
ltrace ./leviathan5  # Analizamos su ejecución
```
Luego, creamos un enlace simbolico a `/etc/leviathan_pass/leviathan6` y lo enlazamos a `/tmp/file.log` para obtener la contrasenia.

**Contrasenia:**
```bash
szo7HDB88w
```

---
## LEVEL 6 -> 7
### Solución
Este nivel se resolvio con ayuda :v
