# /productizar · Agenda + pre-call

Sitio estático, sin build. Dominio: **agendar.productizar.co** (CNAME `agendar` → `tu-sitio.netlify.app`).

Dos páginas:

| Ruta | Archivo | Qué es |
|---|---|---|
| `/` | `index.html` | Página de agenda con el calendario de Cal.com |
| `/confirmada/` | `confirmada/index.html` | Página pre-call (video, confirmar en calendario, preparación) |

Al reservar en `/`, la página manda sola a `/confirmada/`.

## Qué editar

- **Video de la pre-call:** en `confirmada/index.html`, busca `const VIDEO_EMBED = "";` y pega el link de embed de Loom (`https://www.loom.com/embed/...`).
- **Casos:** en el mismo archivo, `const CASOS = [];`.
- **Link de Cal.com:** en `index.html`, `calLink: "checo-perezcuadra-buyzro/30min"`.

## Cal.com

Deja apagado **Redirect on booking** en el evento. La redirección la hace `index.html`.
