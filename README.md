# Portal Académico — Cuerpo Académico CUCEI

Portal web institucional para la difusión de producción científica del Cuerpo Académico de Instrumentación, Óptica, Electrónica y Fotónica de la Universidad de Guadalajara (CUCEI).

## Demo en vivo

[portal-academico-nu.vercel.app](https://portal-academico-nu.vercel.app)

## Descripción

Proyecto desarrollado como parte del Servicio Social universitario. Permite consultar y gestionar la producción científica del cuerpo académico: artículos de investigación, patentes, proyectos, tesistas e integrantes del grupo.

El sistema cuenta con un panel de administración protegido para que los responsables del cuerpo académico mantengan la información actualizada sin necesidad de conocimientos técnicos.

## Funcionalidades

- Consulta pública de artículos, patentes, proyectos y tesistas
- Búsqueda y filtrado en tiempo real
- Visor de documentos PDF integrado
- Panel de administración con autenticación
- Sección de novedades dinámica con los últimos registros
- Diseño responsivo para móvil y escritorio

## Tecnologías

| Capa | Tecnología |
|---|---|
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| Backend | Vercel Serverless Functions (Node.js) |
| Almacenamiento | JSONbin.io |
| Despliegue | Vercel |
| Control de versiones | Git + GitHub |

## Arquitectura

```
Frontend (HTML/CSS/JS)
        ↓
Vercel Serverless API (/api/get-*, /api/save-*)
        ↓
JSONbin.io (almacenamiento JSON en la nube)
```

Los endpoints de escritura están protegidos mediante token de autenticación en el header de cada petición. Las variables de entorno (API keys, tokens, IDs) se gestionan desde Vercel sin exponerse en el código fuente.

## Autor

Edson Ruiz — Estudiante de Ingeniería, CUCEI — Universidad de Guadalajara

[LinkedIn](https://linkedin.com/in/edson-ruiz-4b4b17204) · [GitHub](https://github.com/edsonruiz09112)
