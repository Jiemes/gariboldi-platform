# Estrategia de Desarrollo: Plataforma Odontológica Integral (Gariboldi & Co)

## 1. Visión del Proyecto
Crear una plataforma SaaS "Todo-en-Uno" diseñada específicamente para la realidad del mercado odontológico en Mercedes y Bragado, automatizando la gestión clínica, administrativa y la relación con obras sociales.

## 2. Investigación y Diferenciadores (Benchmarking)
Basado en el análisis de plataformas globales (Open Dental, Curve) y locales (Benty, Bilog):
- **Automatización de Liquidaciones**: Módulo específico para generar planillas de Obras Sociales (OSDE, Galeno, Swiss Medical, etc.) con los códigos de prestaciones actualizados.
- **Omnicanalidad**: Recordatorios automáticos vía WhatsApp (más efectivo en Argentina) y Email.
- **Privacidad Granular**: Esquema de permisos donde los odontólogos solo ven su producción y pacientes, y las secretarias gestionan la agenda de su consultorio asignado.
- **Tele-odontología y Portal del Paciente**: Para subir estudios y ver planes de tratamiento desde el celular.

## 3. Arquitectura Propuesta
- **Modelo**: Multi-tenant SaaS (Aislamiento total de datos por grupo/consultorio).
- **Frontend**: React.js / Next.js con Tailwind CSS para una interfaz moderna, rápida y "Glassmorphic".
- **Backend**: Node.js / Python (FastAPI) con base de datos PostgreSQL (con particionamiento por Tenant).
- **Infraestructura**: AWS o Google Cloud con cumplimiento redundante y backups automáticos.
- **Seguridad**: Autenticación 2FA, cifrado de datos sensibles y logs de auditoría.

## 4. Plan Estratégico (Fases)

### Fase 1: Descubrimiento y Diseño (Semanas 1-4)
- User Personas (Odontólogo, Secretaria, Dueño de Red).
- User Journey Maps.
- Prototipado de alta fidelidad (UI/UX).
- Definición de diccionario de prestaciones (Nomenclador Nacional Odontológico).

### Fase 2: MVP - Core Clínico (Semanas 5-12)
- Gestión de Pacientes e Historia Clínica.
- Odontograma Digital Interactivo.
- Agenda Dinámica con Drag & Drop.
- Módulo de Roles y Permisos.

### Fase 3: Administrativa y Obras Sociales (Semanas 13-20)
- Liquidaciones automáticas por prestador.
- Control de caja y pagos.
- Facturación electrónica (Integración con AFIP).

### Fase 4: Fidelización y Escalamiento (Semanas 21+)
- Recordatorios vía WhatsApp API.
- IA para análisis de imágenes radiológicas (Partnership).
- Dashboard de Business Intelligence para dueños de clínicas.

## 5. Estrategia de Despliegue en Mercedes y Bragado
1. **Piloto**: Lanzamiento en 2 consultorios seleccionados de la red.
2. **Feedback Loop**: Ajustes semanales basados en el uso real de las secretarias y doctores.
3. **Migración**: Herramientas para importar datos desde Excel u otros sistemas antiguos.
