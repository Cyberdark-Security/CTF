# Informe de Auditoría y Desarrollo del Repositorio - CTF Writeups

## 1. Inventario del Repositorio
Este repositorio contiene una colección de 14 guías (writeups) en formato PDF sobre la resolución de máquinas de Captura la Bandera (CTF) de diversas plataformas.

### Máquinas por Plataforma:
- **MiraSoyRoot:**
  - Anonymous
  - Arcode
  - Fuzzer
  - Mirasoyroot
  - Sabores Ocultos
  - Time Traversal
- **Dockerlabs:**
  - Domain
  - Trust
  - Upload
  - Injection
- **CyberConquer:**
  - Ecorp
  - Enigma Codificado
  - Relampago
  - Vias Ocultas

---

## 2. Análisis de Seguridad
Se han identificado los siguientes puntos de atención respecto a la seguridad y gestión de archivos:

### A. Metadatos en Archivos PDF
**Riesgo:** Los archivos PDF suelen contener metadatos (autor, software de creación, rutas locales del sistema) que pueden filtrar información personal o del entorno de desarrollo del autor.
**Recomendación:** Utilizar herramientas como `exiftool` para limpiar los metadatos antes de subir los archivos.

### B. Integridad de los Archivos
**Riesgo:** No existe un mecanismo para que los usuarios verifiquen que los archivos no han sido alterados.
**Recomendación:** Incluir un archivo `hashes.txt` con las sumas de verificación (SHA-256) de cada PDF.

### C. Enlaces Externos
**Riesgo:** Los writeups suelen contener enlaces a herramientas o recursos. Estos enlaces deben ser auditados periódicamente para evitar el "link rotting" o redirecciones a sitios maliciosos.

---

## 3. Sugerencias de Desarrollo y Optimización

### A. Estructura de Directorios
Actualmente, todos los archivos están en la raíz. Se recomienda organizar por plataforma para mejorar la escalabilidad:
```text
/
├── Dockerlabs/
├── MiraSoyRoot/
└── CyberConquer/
```

### B. Adopción de Markdown (.md)
**Mejora:** Cambiar de PDF a Markdown ofrece múltiples ventajas:
- **Control de Versiones:** Permite ver cambios exactos en el contenido mediante `git diff`.
- **Accesibilidad:** Mejor indexación por motores de búsqueda y facilidad de lectura en dispositivos móviles.
- **Peso:** Reduce drásticamente el tamaño del repositorio.

### C. Automatización (CI/CD)
Implementar GitHub Actions para:
- Validar que no se suban archivos pesados innecesarios.
- Generar automáticamente una tabla de contenidos en el README.
- Comprobar la validez de los enlaces internos y externos.

### D. Convención de Nombres
Se recomienda evitar espacios y caracteres especiales en los nombres de archivos para asegurar la compatibilidad en todos los sistemas operativos (ej: `Machine_Trust_Dockerlabs.pdf`).
