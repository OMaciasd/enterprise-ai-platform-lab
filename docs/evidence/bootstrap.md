# Bootstrap Evidence

## Fecha

- UTC de ejecución: 2026-11-09T04:12:05Z
- UTC de creación de esta evidencia: 2026-11-09T04:15:00Z

## Repositorio

- URL: https://github.com/OMaciasd/enterprise-ai-platform-lab
- Visibilidad: pública
- Descripción: Enterprise AI Platform Lab
- Rama predeterminada: main
- allow_auto_merge: false
- Repositorio de referencia intacto: `/home/oscar/projects/vscode-wsl-action-buttons`

## Ramas y SHAs antes de la evidencia

| Rama | SHA | Contenido |
| --- | --- | --- |
| main | 328e13d4d48f6946ddae1e49168020e1209499c5 | Commit raíz vacío |
| feat/enterprise-ai-platform-foundation | 873610bb6d8c26af45246b5eee9da20ce3109f27 | Scaffold de bootstrap |

## T0: estado del repositorio de referencia

Capturado fuera de ambos repositorios en
`/tmp/opencode/enterprise-ai-platform-lab-bootstrap/t0`.

- Fecha UTC: 2026-11-09T04:12:24Z
- Ruta: `/home/oscar/projects/vscode-wsl-action-buttons`
- Rama: `feat/ollama-terminal-button`
- HEAD: `ebe128c6ca800c648bbf675c05be11798390c583`
- Último commit: `chore: ignore .opencode plan files` (2026-11-04T01:38:08-05:00)
- Worktree: único, en la misma ruta y HEAD
- Stash: `stash@{0}: On feat/parity-original-buttons: backup-before-icon-only-english-ui`
- Índice: SHA-256 `03986061317eb2a868c9f3d9c50d236f462b23d4a0675683d4d590f76d328c96`
- Estado de trabajo: rama adelantada 1 commit; cambios no preparados en
  `README.md` y `package.json`; varios archivos no rastreados y respaldos.
- Configuración: `origin` apuntaba únicamente a
  `https://github.com/OMaciasd/vscode-wsl-action-buttons.git`.
- No se modificó el repositorio de referencia durante la captura.

El detalle completo (status, stash, configuración, índice, worktrees y remotos)
se conserva en el directorio T0 indicado.

## Controles aplicados

- Repositorio remoto creado público sin `--source`, `--push`, README ni
  licencia automática.
- `main` contiene exactamente un commit raíz vacío.
- El scaffold y la evidencia viven únicamente en la rama feature.
- `origin` se configuró únicamente en el repositorio nuevo.
- No se crearon pull requests, merges ni despliegues.
- No se activó auto-merge; `allow_auto_merge=false`.
- No se modificó ningún otro repositorio.
- No se borraron archivos ni recursos.
- No se modificó `.wslconfig`.
- No se instalaron herramientas ni se descargaron modelos.
- No se incluyeron secretos, tokens, credenciales ni datos personales.
- Se documentó la naturaleza de laboratorio y la diferencia entre PoC y
  experiencia profesional real.

## Herramientas

| Herramienta | Versión | Uso |
| --- | --- | --- |
| git | 2.43.0 | Inicialización, commits y push |
| gh | 2.78.0 | Creación y configuración del repositorio |
| gitleaks | 8.18.2 | Escaneo de árbol e historial con redacción |

## Resultados de seguridad

- Gitleaks sobre el árbol (`--no-git`): 0 hallazgos.
- Gitleaks sobre el historial: 0 hallazgos. El informe indicó 1 commit
  escaneado; el commit raíz de `main` es vacío y no contiene archivos.
- Gitleaks con `--log-opts="--all"`: 0 hallazgos.
- Reportes generados fuera del repositorio, con redacción, en
  `/tmp/opencode/enterprise-ai-platform-lab-bootstrap/security/`.
- Revisión manual: sin `.env`, claves privadas, credenciales ni archivos
  sensibles rastreados.
- `detect-secrets` no está operativo en el entorno
  (`ModuleNotFoundError: No module named 'detect_secrets'`). No se intentó
  instalar. Esta limitación se documenta y el control se cubrió con Gitleaks y
  revisión manual.

## Archivos del scaffold

- `README.md`
- `.gitignore`
- `LICENSE` (Apache-2.0 completo)
- `NOTICE`
- `docs/ARCHITECTURE.md`
- `docs/ROADMAP.md`
- `infra/README.md`
- `src/README.md`

## Estado de Fase 0

La Fase 0 no se ha iniciado. El bootstrap termina con este documento.
