# marlene-ch1-2026

Material de un curso, publicado como sitio estático y **cifrado del lado del cliente**.

Lo que hay en este repo son bloques cifrados con AES-GCM 256. La clave se deriva de una contraseña
con PBKDF2-SHA256 (310.000 vueltas) y nunca está acá: sin ella no hay nada que leer.

El sitio no se indexa (`robots.txt` y `<meta name="robots" content="noindex">`).

Se regenera desde el proyecto `marlene`:

```
python3 scripts/armar_sitio.py --salida ../marlene-sitio --password "la de siempre"
```
