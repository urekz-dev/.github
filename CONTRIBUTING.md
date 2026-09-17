# Contribuir a los repositorios de Urekz

Cómo trabajamos está en el handbook público: https://handbook.urekz.com. Esta página resume lo que aplica a cualquier repositorio de `urekz-dev`.

## Origen del trabajo
El trabajo se planifica en **Plane**. GitHub Issues está desactivado. Todo PR enlaza un work item (`EMR-12`, `UCODE-4`, `UREKZ-7`) o declara `N/A - maintenance exception`.

## Ramas
Cortas, desde `main`: `<type>/<PLANE-ID>-<descripcion-corta>` (`feat/EMR-12-busqueda-por-categoria`, `docs/UREKZ-3-onboarding`, `rfd/0017-titulo` en el handbook). Una rama por story; mergeada antes del cierre del ciclo de seis semanas.

## Commits
Conventional Commits (`feat`, `fix`, `docs`, `chore`, `refactor`, `test`, `rfd`). Firmados con SSH (ver onboarding en el handbook).

## Pull requests
Plantilla de la organización. Revisión de una persona distinta del autor. CI verde. Conversaciones resueltas. **Squash merge** únicamente: el título del PR es el commit en `main`.

En repos públicos lo impone un ruleset. En repos privados (plan Free) lo vigila el workflow `main-guard`: si alguien hace push directo a `main`, el workflow falla y avisa; corrige con un PR.

## Decisiones
Técnicas de un producto: ADR en `docs/adr/` del repo. Organizativas o transversales: RFD en el handbook.

## Agentes
Un agente puede abrir un PR si el work item lleva `flow:agent-ready`. El PR incluye un recibo: qué leyó, qué cambió, qué verificó. Lo aprueba una persona.

## Seguridad
Sin secretos en el repo: `infisical scan install --pre-commit-hook` en cada clon. Vulnerabilidades: security@urekz.com (ver SECURITY.md).
