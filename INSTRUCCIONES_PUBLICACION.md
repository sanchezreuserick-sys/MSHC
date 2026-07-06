# Cómo publicar este sitio en GitHub Pages

## Opción A — Ya tienes el repo `sanchezreuserick-sys/MSHC`
1. Descarga y descomprime este paquete.
2. Reemplaza todos los archivos dentro de tu repo local (o súbelos directo desde la web de GitHub: **Add file → Upload files**, arrastra todo el contenido de esta carpeta y confirma el commit en `main`).
3. Ve a `https://github.com/sanchezreuserick-sys/MSHC/settings/pages`
4. En **Build and deployment → Source**, elige **Deploy from a branch**.
5. En **Branch**, selecciona `main` y carpeta `/ (root)` → **Save**.
6. En **Custom domain**, escribe `makersteamhorizontecero.space` → **Save** (esto regenera el `CNAME`).
7. Espera 1–3 minutos y confirma el check verde "DNS check successful".

## Opción B — Repo nuevo desde cero
```bash
cd MSHC   # esta carpeta descomprimida
git init
git add .
git commit -m "Publicación inicial del sitio"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/TU-REPO.git
git push -u origin main
```
Luego repite los pasos 3–7 de la Opción A.

## Contenido del paquete
- `index.html` — sitio completo (glassmorphism, asistente IA, animaciones)
- `logo.png` — logo oficial actualizado
- `uniforme_oxford.png`, `uniforme_playera_negra.png`, `uniforme_polo.png`, `uniforme_varsity.png` — piezas del uniforme oficial
- `CNAME` — dominio personalizado configurado
- `README.md` — archivo original del repo

## Nota de seguridad
Ningún archivo aquí contiene credenciales ni tokens. Si en algún momento compartiste un Personal Access Token en el chat, revócalo desde GitHub → Settings → Developer settings → Tokens.
