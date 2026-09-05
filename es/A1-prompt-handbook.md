# Apéndice · Prompt para crear el handbook de tu empresa

Este prompt genera el **handbook interno de tu empresa remota** —las reglas concretas con las que trabajáis— siguiendo la filosofía de esta biblia. La biblia es el *porqué*; el handbook es el *cómo lo hacéis vosotros*.

Pégalo en Claude o ChatGPT, rellena lo que está entre `[corchetes]` y te devuelve el manual en Markdown, listo para subir a GitHub como el resto de la biblia.

## Cómo usarlo

- Rellena todo lo que puedas entre `[corchetes]`. Lo que no sepas, déjalo: el modelo lo marcará `[POR DEFINIR]` en vez de inventárselo.
- Pídelo **sección a sección** si quieres revisar sobre la marcha.
- El prompt no copia la biblia: escribe las reglas específicas de tu empresa. La filosofía la da esta biblia; los datos, tú.

---

## Prompt (copia desde aquí)

```text
Eres un redactor experto en handbooks de empresas remotas, en la línea de
«La Biblia del Remoto» de ActiveXRemote: asíncrono primero, todo por escrito,
se juzga por resultados y no por presencia. Tu tarea NO es repetir esa filosofía,
sino escribir el handbook interno de MI empresa: las reglas concretas con las que
trabajamos. Habla de tú (nunca «usted» ni impersonal), frases de menos de 20
palabras, sin relleno y sin emoji. Todo el dinero, en dólares (USD).

DATOS DE MI EMPRESA (si falta alguno, márcalo como [POR DEFINIR] y sigue; no lo inventes):
- Nombre: [ ]
- Qué hacemos, en una línea: [ ]
- Tamaño del equipo: [ ]
- Dónde está la gente (países y franjas horarias): [ ]
- Cómo contratamos (contratista / EOR / mixto): [ ]
- Solapamiento horario obligatorio: [p. ej. 3 h entre 14:00 y 17:00 CET, o «ninguno»]
- Herramientas (stack): [comunicación · documentación · gestión · pago]
- Filosofía de sueldo (ajustado por geografía / igual para todos): [ ]
- Política de reuniones: [ ]
- Vacaciones y bajas: [días y cómo se piden]
- Seguridad mínima obligatoria: [gestor de contraseñas, 2FA, cifrado de disco…]
- Cómo nos tratamos (valores, en 3-5 frases): [ ]
- KPI o métrica del norte de la empresa: [ ]
- País de la entidad legal y notas legales: [ ]
- Idioma del handbook: [español / inglés / ambos]

INSTRUCCIONES:
1. Antes de escribir, si falta algún dato crítico (contratación, solapamiento,
   seguridad, KPI), pídemelo. Si te digo que sigas, marca esos huecos como [POR DEFINIR].
2. Escribe el handbook en Markdown, listo para GitHub: un archivo por sección con
   encabezado H1, y un README.md que enlace todas las secciones. Nombra los archivos
   00-, 01-, 02-…
3. Estructura de referencia (adáptala a mi empresa, no la copies a ciegas):
   00 · Bienvenida y cómo usar este handbook
   01 · Cómo trabajamos (asíncrono primero, todo por escrito)
   02 · Comunicación (qué canal para qué, tiempos de respuesta)
   03 · Reuniones (cuándo sí, cómo se preparan)
   04 · Jornada y disponibilidad (horas, solapamiento, zonas)
   05 · Vacaciones, bajas y ausencias
   06 · Cómo te contratamos y cómo cobras (contratista / EOR)
   07 · Beneficios y extras
   08 · Rendimiento: KPI, reports y evaluaciones
   09 · Herramientas y accesos
   10 · Seguridad y dispositivos
   11 · Onboarding: tus primeros 90 días
   12 · Cómo nos tratamos (código de conducta)
4. Reglas de estilo: cada norma dice qué se hace, quién y cuándo; una idea por
   sección; sin ambigüedad. Cada afirmación con un dato debe poder atarse a una
   política real de la empresa; si no me la has pedido, va como [POR DEFINIR].
5. No inventes cifras, leyes ni políticas. Al pie de cualquier sección legal o
   fiscal añade: «Esto no es asesoramiento legal; consulta con un profesional del país».
6. Marca el handbook como documento vivo: en el README, una nota de versión y la fecha.
7. Empieza pidiéndome los datos que falten. Luego genera el README y ve sección a
   sección, parándote tras cada una para que la revise antes de seguir.
```

---

## Después de generarlo

Guarda cada sección como su propio `.md`. Puedes subirlo a un repositorio nuevo, o meterlo en este mismo dentro de una carpeta `handbook/`, con los mismos pasos que usaste para la biblia (privado hasta la revisión, colaboradores invitados). El handbook son las reglas de tu empresa; la biblia es la referencia que las inspira. Que vivan juntos ayuda a que no se contradigan.
