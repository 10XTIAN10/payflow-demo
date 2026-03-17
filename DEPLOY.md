# 🚀 Publicar PayFlow Demo en GitHub Pages

Seguí estos pasos para tener tu demo en una URL pública en menos de 5 minutos.

---

## Paso 1 — Crear un repositorio en GitHub

1. Andá a [github.com/new](https://github.com/new)
2. Completá los campos:
   - **Repository name**: `payflow-demo` (o el nombre que prefieras)
   - **Visibility**: Public ✅ (requerido para GitHub Pages gratis)
   - **No** tildes "Add a README file"
3. Hacé clic en **Create repository**

---

## Paso 2 — Subir los archivos desde tu computadora

Abrí una terminal en la carpeta `Demo Fintech` y ejecutá estos comandos uno por uno:

```bash
# Inicializar git en la carpeta
git init

# Agregar todos los archivos
git add index.html

# Primer commit
git commit -m "Initial commit: PayFlow demo con Amplitude"

# Conectar con tu repositorio de GitHub
# (reemplazá TU_USUARIO por tu nombre de usuario de GitHub)
git remote add origin https://github.com/TU_USUARIO/payflow-demo.git

# Subir al branch principal
git branch -M main
git push -u origin main
```

> 💡 Si es la primera vez que usás git, puede pedirte autenticarte. Usá tu usuario y un **Personal Access Token** (no tu contraseña). Lo podés generar en: GitHub → Settings → Developer settings → Personal access tokens → Generate new token.

---

## Paso 3 — Activar GitHub Pages

1. En tu repositorio de GitHub, andá a **Settings** (pestaña superior)
2. En el menú izquierdo, buscá **Pages**
3. En la sección **Build and deployment**:
   - **Source**: Deploy from a branch
   - **Branch**: `main` / `/ (root)`
4. Hacé clic en **Save**

GitHub tardará entre 1 y 3 minutos en publicar el sitio.

---

## Paso 4 — Acceder a tu URL pública

Una vez desplegado, tu demo va a estar disponible en:

```
https://TU_USUARIO.github.io/payflow-demo/
```

La URL aparece también en la sección **Pages** de Settings una vez que el deploy terminó.

---

## Actualizar la demo en el futuro

Cada vez que modifiques el `index.html` y quieras publicar los cambios:

```bash
git add index.html
git commit -m "Update: descripción del cambio"
git push
```

GitHub Pages se actualiza automáticamente en 1-2 minutos.

---

## ✅ Checklist rápido

- [ ] Repositorio creado en GitHub (público)
- [ ] `git init` + `git push` ejecutados
- [ ] GitHub Pages activado desde Settings → Pages
- [ ] URL pública funcionando
- [ ] Badge "Amplitude activo ✓" visible en la demo

---

> **Tip para demos con clientes**: compartí la URL directamente en la reunión. No requiere que el cliente instale nada — se abre en cualquier browser y los eventos de Amplitude se trackean en tiempo real.
