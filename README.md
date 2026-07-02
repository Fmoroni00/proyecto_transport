# 🚖 TransPort (Flask + Leaflet)

**TransPort** es una aplicación web desarrollada en **Python (Flask)** con interfaz basada en **Leaflet.js** que permite la conexión entre **pasajeros** y **conductores** dentro de un entorno de rutas simuladas en Lima Metropolitana.  
El sistema permite registrar usuarios, buscar viajes, visualizar rutas en el mapa y almacenar la información localmente en archivos JSON.

---

## 🌐 Demo en línea

👉 **Versión pública:** [https://proyecto-transport.onrender.com](https://proyecto-transport.onrender.com)

> ⚠️ *La versión online puede tardar unos segundos en cargar por la instancia gratuita de Render.*

---

## 🧩 Características principales

- 👥 Registro y login de **pasajeros** y **conductores**
- 🚗 Creación de rutas y búsqueda de viajes
- 🗺️ Visualización interactiva con **Leaflet**
- ⚙️ Algoritmo para calcular la mejor ruta entre puntos
- 💾 Almacenamiento de datos en archivos `.json`
- 🧠 Sistema de solicitudes (match entre pasajero y conductor)
- 📱 **Interfaz responsive** (nueva versión adaptada para conductores)
- 🔒 Hash de contraseñas con `werkzeug.security`
- 🧰 Módulos estructurados (servicios, controladores, templates, etc.)

---

## 🧱 Estructura del proyecto

```

proyecto_transport/
│
├── app.py                        # Archivo principal (Flask)
│
├── data/                         # Archivos JSON con datos persistentes
│   ├── pasajeros.json
│   ├── conductores.json
│   └── viajes.json
│
├── servicios/                    # Lógica de negocio y manejo de datos
│   ├── usuarios_repo.py
│   ├── gestor_rutas.py
│   └── solicitudes.py
│
├── static/                       # Archivos estáticos (CSS, JS, imágenes)
│
├── templates/                    # Páginas HTML con Jinja2
│   ├── index.html
│   ├── login.html
│   ├── registro.html
│   ├── dashboard.html
│   ├── buscar_viaje.html
│   ├── crear_ruta.html
│   └── mis_viajes.html
│
├── requirements.txt              # Dependencias del proyecto
├── README.md                     # Este archivo 😄
└── .gitignore

````

---

## ⚙️ Instalación local

1️⃣ Clona el repositorio:
```bash
git clone https://github.com/milagros-hr/proyecto_transport.git
````

2️⃣ Entra al proyecto:

```bash
cd proyecto_transport
```

3️⃣ Crea un entorno virtual:

```bash
python -m venv .venv
```

4️⃣ Activa el entorno virtual:

* En Windows:

  ```bash
  .venv\Scripts\activate
  ```
* En macOS/Linux:

  ```bash
  source .venv/bin/activate
  ```

5️⃣ Instala las dependencias:

```bash
pip install -r requirements.txt
```

6️⃣ Ejecuta el servidor local:

```bash
python app.py
```

7️⃣ Abre en tu navegador:

```
http://127.0.0.1:5000/
```

---

## 🧠 Tecnologías utilizadas

| Tecnología         | Descripción                      |
| ------------------ | -------------------------------- |
| 🐍 Flask           | Framework backend en Python      |
| 🌍 Leaflet.js      | Librería para mapas interactivos |
| 🧾 JSON            | Almacenamiento de datos local    |
| 💡 HTML / CSS / JS | Interfaz web y diseño            |
| 🔐 Werkzeug        | Seguridad de contraseñas         |

---


