# Guía de Contribución

## Convención de Commits

Usamos [Conventional Commits](https://www.conventionalcommits.org/) para nuestros mensajes de commit. Cada mensaje de commit debe tener la siguiente estructura:

```
<tipo>[alcance opcional]: <descripción>

[cuerpo opcional]

[nota de pie opcional]
```

### Tipos de Commits

- `feat`: Nueva característica
- `fix`: Corrección de errores
- `docs`: Cambios en documentación
- `style`: Cambios que no afectan el significado del código
- `refactor`: Cambio de código que no corrige errores ni añade características
- `test`: Añadir o corregir tests
- `chore`: Cambios en el proceso de build o herramientas auxiliares

### Ejemplos

```
feat: add login component
fix(auth): correct token validation
docs: update README with new API endpoints
style: format code with prettier
refactor: restructure user service
test: add unit tests for auth middleware
chore: update dependencies
```

## Flujo de Trabajo con Git

1. Crear una nueva rama para cada feature/fix:
```bash
git checkout -b feature/nombre-feature
git checkout -b fix/nombre-fix
```

2. Hacer commits frecuentes siguiendo la convención

3. Antes de hacer push:
```bash
git pull origin main
# Resolver conflictos si existen
```

4. Push a GitHub:
```bash
git push origin nombre-rama
```

5. Crear Pull Request en GitHub

## Estructura de Ramas

- `main`: Código en producción
- `develop`: Código en desarrollo
- `feature/*`: Nuevas características
- `fix/*`: Correcciones
- `docs/*`: Documentación

## Reglas Adicionales

1. No hacer commit directamente a `main`
2. Mantener los commits pequeños y enfocados
3. Escribir mensajes de commit descriptivos
4. Actualizar la documentación cuando sea necesario
