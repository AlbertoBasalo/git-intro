1. Resolver conflictos, `merge` con `rebase`, `stash`

2. Modo de trabajo: _gitflow_ puro

3. Ramas que utilizamos y formatos de las mismas

Ramas **master**, **release** y **develop**
• Ramas protegidas, solo se modifican a través de Merge request.

Ramas **feature**
• Formato: feature/[id-tarea]-[título-de-tarea]
• El título de la tarea debería estar en un máximo de 40 caracteres, no se forzará ese límite ya que se espera que se siga esa recomendación (sin los corchetes).
• Las ramas de features se podarán después de realizar el merge, en caso de que haya que volver a la misma tarea se abrirá la rama con la nomenclatura anterior igualmente.

Ramas **hotfix**
• Formato: fix/[id-tarea]

Ramas **release**
• Formato: release/sprint-[id-sprint]
• Al mezclar en esta rama, se desplegaría de forma automática en nuestros servidores de test.

> La convención para hacer commits: https://www.conventionalcommits.org/en/v1.0.0/

# 1. Fundamentos de git

Gestión de cambios en el repositorio local
Integración en el repositorio remoto

# 2. Control de cambios

Creación y mezclado de ramas
Etiquetas y puntos de control

# 3. Gestión de conflictos

Conflictos locales
Conflictos globales

# 4. Flujos de trabajo

Conceptos y ramas involucradas
Un Happy Path con Git Flow
