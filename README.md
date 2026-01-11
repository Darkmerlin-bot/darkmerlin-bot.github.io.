# 🌿 GlutenFree Kitchen

Aplicación web progresiva (PWA) para planificar comidas sin gluten y bajas en carbohidratos, con **búsqueda inteligente de recetas online** y lista de compras compartida.

![Preview](https://img.shields.io/badge/Gluten-Free-green) ![Carbs](https://img.shields.io/badge/Low-Carb-orange) ![PWA](https://img.shields.io/badge/PWA-Ready-blue)

## ✨ Características

- 🔍 **Búsqueda inteligente de recetas** - Busca en la web y analiza automáticamente si son sin gluten y bajas en carbs
- 📖 **20+ recetas base** sin gluten y bajas en carbohidratos
- 🧪 **Análisis automático** de ingredientes para verificar gluten y carbohidratos
- 📅 **Planificador semanal** de menús (desayuno, almuerzo, cena)
- 🛒 **Lista de compras** generada automáticamente desde el menú
- ✅ Items tachables para ir marcando lo que comprás
- ➕ Agregar items manualmente a la lista
- 📱 **Instalable** como app en el celular
- 🔄 **Datos compartidos** entre usuarios via GitHub Pages

## 🔍 Búsqueda Inteligente

La app puede buscar recetas en internet y analizarlas automáticamente:

1. Escribe lo que querés cocinar (ej: "pollo", "ensalada", "pescado")
2. La IA busca recetas en la web
3. Analiza cada ingrediente para detectar gluten
4. Calcula los carbohidratos estimados
5. Muestra solo las recetas que son APTAS (sin gluten + bajo en carbs)

**Ingredientes que detecta como GLUTEN:**
- Harina de trigo, pan, pasta, fideos
- Cebada, centeno, avena regular
- Empanizados, rebozados, salsa de soja

**Ingredientes que detecta como ALTO EN CARBS:**
- Papa, arroz, maíz, azúcar
- Banana, mango, piña
- Legumbres, quinoa

## 🚀 Cómo usar con GitHub (Para compartir entre 2 usuarios)

### Paso 1: Crear el repositorio

1. Andá a [github.com](https://github.com) y logueate
2. Hacé clic en el botón verde **"New"** para crear un repositorio
3. Nombre del repositorio: `gluten-free-kitchen` (o el que quieras)
4. Marcá como **Public**
5. Click en **"Create repository"**

### Paso 2: Subir los archivos

1. En el repositorio vacío, hacé clic en **"uploading an existing file"**
2. Arrastrá todos los archivos de la carpeta:
   - `index.html`
   - `manifest.json`
3. Hacé clic en **"Commit changes"**

### Paso 3: Activar GitHub Pages

1. Andá a **Settings** (configuración del repositorio)
2. En el menú lateral, buscá **Pages**
3. En "Source", seleccioná **Deploy from a branch**
4. En "Branch", seleccioná **main** y carpeta **/ (root)**
5. Click en **Save**
6. Esperá 2-3 minutos y tu app estará en:
   ```
   https://TU-USUARIO.github.io/gluten-free-kitchen/
   ```

### Paso 4: Agregar al segundo usuario

1. Andá a **Settings** → **Collaborators**
2. Click en **"Add people"**
3. Ingresá el nombre de usuario o email del otro usuario
4. El otro usuario acepta la invitación desde su email

### Paso 5: Instalar como app en el celular

**En Android (Chrome):**
1. Abrí la URL de GitHub Pages en Chrome
2. Tocá el menú (3 puntos) → **"Agregar a pantalla de inicio"**
3. Confirmá y listo, tenés la app instalada

**En iPhone (Safari):**
1. Abrí la URL en Safari
2. Tocá el botón de compartir (cuadrado con flecha)
3. Seleccioná **"Agregar a pantalla de inicio"**

## 🔄 Cómo sincronizar datos entre usuarios

Para que ambos usuarios vean los mismos menús y lista de compras, pueden usar una de estas opciones:

### Opción A: Sincronización manual (Simple)
Exportá/importá los datos usando el LocalStorage del navegador.

### Opción B: Usando un backend gratuito (Avanzado)
Podés agregar Firebase Realtime Database o Supabase para sincronización en tiempo real. Contactame si querés ayuda con esto.

### Opción C: Archivo JSON compartido
Editá el archivo `data.json` en GitHub y ambos usuarios tendrán los mismos datos base.

## 📂 Estructura de archivos

```
gluten-free-kitchen/
├── index.html      # App principal (todo incluido)
├── manifest.json   # Configuración PWA
└── README.md       # Este archivo
```

## 🥗 Recetas incluidas

| Categoría | Recetas |
|-----------|---------|
| 🌅 Desayuno | Huevos con aguacate, Omelette de espinacas, Pancakes de almendra |
| ☀️ Almuerzo | Ensalada César, Tacos de lechuga, Zoodles con pesto, Ensalada griega |
| 🌙 Cena | Salmón con espárragos, Pollo al curry, Costillas de cerdo |
| 🍿 Snacks | Rollitos de jamón, Chips de kale |

## 🛠️ Tecnologías

- HTML5, CSS3, JavaScript vanilla
- Progressive Web App (PWA)
- LocalStorage para persistencia
- Sin dependencias externas

## 📱 Capturas

La app tiene un diseño elegante con:
- Paleta de colores naturales (verde bosque, terracotta, crema)
- Tipografía Playfair Display + DM Sans
- Animaciones suaves
- Optimizado para móviles

## ❓ FAQ

**¿Puedo agregar más recetas?**
Sí, editá el array `recipes` en el archivo `index.html`.

**¿Funciona offline?**
Los datos se guardan localmente, pero para una experiencia offline completa necesitarías agregar un Service Worker.

**¿Es seguro para celíacos?**
Las recetas fueron diseñadas sin gluten, pero siempre verificá los ingredientes que comprás.

---

Hecho con 💚 para una vida más saludable
