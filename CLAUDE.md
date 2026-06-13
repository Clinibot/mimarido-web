# CLAUDE.md — Guía crítica para este proyecto

## ⚠️ IDENTIDAD LEGAL DEL PROYECTO — LEE ESTO PRIMERO

**Mimarido.es es un proyecto creado y propiedad de su autora. La empresa titular es ÚNICAMENTE:**

| Campo | Valor correcto |
|---|---|
| Razón social | **Pan y Rosas online SL** |
| NIF | **B10537462** |
| Email de contacto | **info@mimarido.es** |
| Domicilio | Calle Rosselló 42, 08328 Alella (Barcelona), España |

### PROHIBIDO usar cualquiera de estos datos — NO pertenecen a este proyecto:

- `Telvia Comunicaciones SL` — empresa ajena, NO titular del proyecto
- `Telvia` — cualquier mención de esta palabra está PROHIBIDA
- `B22615314` — NIF de Telvia, NO usar nunca
- `info@telvia.io` — email de Telvia, NO usar nunca

> **Por qué esto es crítico:** incluir datos de otra empresa en los textos legales (Términos, Privacidad) equivale a ceder la titularidad del proyecto a esa empresa. Es un error legal gravísimo.

### Antes de cualquier cambio en archivos legales o de pie de página

Antes de editar `terminos.html`, `privacidad.html`, `index.html` o cualquier archivo que mencione al titular del proyecto, verifica que los datos legales son exactamente los de la tabla de arriba. Si hay alguna duda, pregunta antes de escribir.

### Búsqueda de seguridad

Para comprobar que no hay datos incorrectos en el repo, ejecuta:

```bash
grep -ri "telvia\|B22615314\|info@telvia" .
```

El resultado debe ser **vacío**. Si aparece cualquier coincidencia, corrígela inmediatamente.

---

## Estructura del proyecto

Sitio web estático de **mimarido.es** — landing page + páginas legales.

| Archivo | Descripción |
|---|---|
| `index.html` | Página principal |
| `terminos.html` | Términos y condiciones |
| `privacidad.html` | Política de privacidad |
| `exito.html` | Página post-pago exitoso (Stripe) |
| `cancelado.html` | Página post-pago cancelado (Stripe) |

## Rama de desarrollo

Desarrollar siempre en la rama asignada por la sesión. No hacer push directo a `main`.
