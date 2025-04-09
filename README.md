
# VigilantIA ⚖️

![Logo de VigilantIA](https://raw.githubusercontent.com/bladealex9848/VigilantIA/main/logo.png)

[![Version](https://img.shields.io/badge/versión-1.0.0-darkgreen.svg)](https://github.com/bladealex9848/VigilantIA)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.30.0-ff4b4b.svg)](https://streamlit.io/)
[![OpenAI](https://img.shields.io/badge/OpenAI_API-v2-00C244.svg)](https://platform.openai.com/)
[![Licencia](https://img.shields.io/badge/Licencia-MIT-yellow.svg)](LICENSE)
[![Visitantes](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fvigilantia.streamlit.app&label=Visitantes&labelColor=%235d5d5d&countColor=%231e7ebf&style=flat)](https://vigilantia.streamlit.app)

## ⚖️ Descripción

VigilantIA es un asistente virtual especializado en Vigilancia Judicial Administrativa en Colombia, desarrollado con Streamlit y la API de OpenAI. Su base de conocimiento incluye el artículo 101 de la Ley 270 de 1996, el Acuerdo No. PSAA11-8716 de 2011 y la Circular PCSJC17-43 de 2017.

Este asistente está diseñado para proporcionar información clara y accesible sobre los procedimientos, requisitos y efectos de la Vigilancia Judicial Administrativa a magistrados, jueces, abogados, estudiantes de derecho y cualquier persona interesada en este ámbito específico del sistema judicial colombiano.

## 🔍 Funcionalidades Principales

### 1. Marco Legal y Fundamentación
- **Base Normativa**: Información sobre la Ley 270 de 1996, Acuerdo No. PSAA11-8716 de 2011 y Circular PCSJC17-43 de 2017
- **Naturaleza y Alcance**: Explicación sobre el control administrativo y sus diferencias con la acción disciplinaria
- **Fundamentación Jurídica**: Análisis de la base constitucional y legal de la vigilancia judicial

### 2. Procedimiento Detallado
- **Fase de Iniciación**: Información sobre modalidades de inicio y requisitos
- **Fase de Reparto**: Explicación del procedimiento de asignación
- **Recopilación de Información**: Detalle sobre plazos y métodos de verificación
- **Apertura y Traslado**: Elementos del auto de apertura y términos procesales
- **Fase de Decisión**: Procedimiento para la toma de decisiones administrativas

### 3. Aspectos Procedimentales
- **Notificaciones**: Información sobre las distintas modalidades de notificación
- **Recursos**: Detalle sobre el recurso de reposición y sus plazos
- **Efectos**: Implicaciones en calificación de servicios, traslados y estímulos
- **Garantías Procesales**: Explicación sobre el derecho de defensa y motivación de decisiones

### 4. Análisis de Documentos
- **Procesamiento OCR**: Análisis de documentos administrativos mediante tecnología avanzada
- **Evaluación Jurídica**: Análisis preliminar de documentos desde la perspectiva administrativa
- **Identificación de Elementos Clave**: Detección de aspectos relevantes en documentos oficiales
- **Sugerencias Normativas**: Referencias a normativa y jurisprudencia aplicables

## 🚀 Instalación

### Requisitos Previos
- Python 3.8 o superior
- Pip (administrador de paquetes de Python)
- Cuenta en OpenAI con acceso a la API
- Asistente VigilantIA configurado en OpenAI

### Pasos de Instalación

1. **Clonar el repositorio**
   ```bash
   git clone https://github.com/bladealex9848/VigilantIA.git
   cd VigilantIA
   ```

2. **Crear un entorno virtual (recomendado)**
   ```bash
   python -m venv venv
   
   # En Windows
   venv\Scripts\activate
   
   # En macOS/Linux
   source venv/bin/activate
   ```

3. **Instalar las dependencias**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configurar credenciales**

   **Opción A: Usando variables de entorno**
   ```bash
   # En Windows
   set OPENAI_API_KEY=tu-api-key-aqui
   set ASSISTANT_ID=tu-assistant-id-aqui
   
   # En macOS/Linux
   export OPENAI_API_KEY=tu-api-key-aqui
   export ASSISTANT_ID=tu-assistant-id-aqui
   ```

   **Opción B: Usando archivo secrets.toml**
   
   Crea un archivo `.streamlit/secrets.toml` con el siguiente contenido:
   ```toml
   OPENAI_API_KEY = "tu-api-key-aqui"
   ASSISTANT_ID = "tu-assistant-id-aqui"
   ```

## ⚙️ Uso

### Iniciar la Aplicación

```bash
streamlit run app.py
```

Esto lanzará la aplicación y abrirá automáticamente una ventana del navegador en `http://localhost:8501`.

### Funcionalidades del Asistente

1. **Consultas sobre Vigilancia Judicial Administrativa**
   - Pregunta sobre conceptos, procedimientos o normativa aplicable
   - Ejemplo: "¿Cuáles son las fases del procedimiento de vigilancia judicial administrativa?"

2. **Información sobre Aspectos Procesales**
   - Consulta sobre recursos, notificaciones y efectos
   - Ejemplo: "¿Qué recursos proceden contra las decisiones de vigilancia judicial?"

3. **Consultas sobre Competencia**
   - Obtén información sobre las autoridades competentes y sus facultades
   - Ejemplo: "¿Quién es competente para iniciar un proceso de vigilancia judicial administrativa?"

4. **Análisis de Documentos**
   - Sube documentos para recibir un análisis desde la perspectiva administrativa
   - El asistente puede procesar autos, informes o decisiones administrativas

5. **Referencia Normativa**
   - Solicita información sobre normativa específica o jurisprudencia relevante
   - Ejemplo: "¿Qué establece el Acuerdo No. PSAA11-8716 de 2011 sobre el procedimiento?"

## ⚠️ Limitaciones

- VigilantIA proporciona información general y no constituye asesoramiento legal personalizado
- La información se basa en el conocimiento disponible hasta octubre de 2023
- Para casos específicos, siempre es recomendable consultar con un abogado especializado
- El análisis de documentos es preliminar y no reemplaza la revisión profesional

## 📊 Escenarios de Uso

### 1. Magistrados y Jueces
- Consulta de normativa y procedimientos aplicables
- Comprensión de sus derechos y garantías procesales
- Información sobre efectos de las medidas de vigilancia

### 2. Profesionales del Derecho
- Referencia rápida sobre normativa y jurisprudencia
- Análisis preliminar de documentos administrativos
- Preparación de recursos y respuestas procesales

### 3. Estudiantes de Derecho
- Orientación académica sobre derecho administrativo judicial
- Comprensión de los mecanismos de control en la Rama Judicial
- Información sobre procedimientos especiales

## 👥 Contribuciones

Las contribuciones son bienvenidas. Para contribuir al desarrollo de VigilantIA:

1. Realiza un fork del repositorio
2. Crea una nueva rama (`git checkout -b feature/nueva-funcionalidad`)
3. Implementa tus cambios
4. Envía un pull request

## 📝 Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.

## 🙏 Agradecimientos

- **OpenAI** por proporcionar la tecnología que impulsa el asistente
- **Streamlit** por facilitar el desarrollo de interfaces intuitivas
- **Rama Judicial de Colombia** por su contribución al derecho administrativo judicial

## 👤 Autor

Creado con ❤️ por [Alexander Oviedo Fadul](https://github.com/bladealex9848)

[GitHub](https://github.com/bladealex9848) | [Website](https://alexanderoviedofadul.dev) | [LinkedIn](https://www.linkedin.com/in/alexander-oviedo-fadul/) | [Instagram](https://www.instagram.com/alexander.oviedo.fadul) | [Twitter](https://twitter.com/alexanderofadul) | [Facebook](https://www.facebook.com/alexanderof/) | [WhatsApp](https://api.whatsapp.com/send?phone=573015930519&text=Hola%20!Quiero%20conversar%20contigo!%20)

---

## 💼 Mensaje Final

VigilantIA busca democratizar el acceso a la información sobre Vigilancia Judicial Administrativa en Colombia, facilitando la comprensión de conceptos jurídicos complejos. Aunque este asistente proporciona información valiosa, recuerda que cada caso administrativo es único y puede requerir orientación profesional personalizada.

*"El conocimiento de los procedimientos administrativos judiciales es fundamental para garantizar una adecuada administración de justicia y proteger los derechos de todos los actores del sistema judicial."*