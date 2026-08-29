# TargApps — GitHub Copilot instructions (solo este workspace)

> **Alcance:** Estas reglas aplican **SOLO** al workspace TargApps (`/media/vmcode/Cluster Mint/Atlas/TargApps`).
> **NO** son reglas globales de Cursor, Claude, Gemini ni del usuario.
> Solo aplican cuando se trabaja en este monorepo/proyecto.

Convención local de commits con etapas griegas. Ver [`../AGENTS.md`](../AGENTS.md) para el detalle completo.

## Formato

```
[<etapa>] <tipo>: <descripción>
```

Etapas: `o` (omega, experimental), `a` (alfa), `b` (beta), `g` (gama), `d` (delta), `e` (épsilon / producción v1 RC).

## Reglas

- Progresión solo hacia adelante: `a → b → g → d → e`
- No retroceder la etapa de un proyecto
- `[o]` / `[ω]` es la única excepción (experimentos)
- Proyectos y features nuevos empiezan en `[a]`

Etapa actual por proyecto: [`../STAGE.md`](../STAGE.md)

Validación: `./scripts/commit-stage.sh validate "[g] feat: descripción" <proyecto>`
