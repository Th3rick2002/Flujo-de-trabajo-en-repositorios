# 🚀 Guía de flujo de trabajo con Git y GitHub

Este repositorio sigue un flujo de trabajo colaborativo basado en **Git Flow simplificado**.  
La idea es mantener el código limpio, revisado y organizado sin complicaciones innecesarias.

---

## 🧭 Estructura de ramas

| Rama | Propósito |
|------|------------|
| **main** | Contiene la versión estable y actualizada del proyecto. |
| **dev** | Rama de integración. Aquí se fusionan las ramas `feature/*` antes de pasar a `main`. |
| **feature/nombre-dev** | Cada desarrollador trabaja sus funciones específicas aquí. |
| **prod** | Rama usada exclusivamente para despliegue (viene de `main`). |

### 💡 Ejemplos de nombres de ramas

Usa nombres descriptivos y añade tu nombre o alias:

```bash
feature/login-erick
fix/product-price-calc-jose
refactor/inventory-module-ana
docs/api-reference-luis
```

## 🧱 Reglas del flujo de trabajo

🚫 Prohibido hacer push directo a main, dev o prod.
Solo se aceptan Pull Requests (PR).

👀 Cada PR debe ser revisado por al menos 2 desarrolladores antes de aprobarse.

🗂️ No eliminar ramas del repositorio remoto.
Se pueden limpiar ramas inactivas cada cierto tiempo (mensualmente o segun proyecto).

✅ main y prod deben estar siempre estables, funcionales y listas para deploy.

## 🧩 Formato de commits

Usamos el estándar de Conventional Commits:

Tipo	Descripción
- feat:	Nueva característica o funcionalidad.
- fix:	Corrección de errores.
- refactor:	Mejora de código sin cambiar funcionalidad.
- chore:	Tareas menores (configuración, dependencias, etc).
- docs:	Cambios en documentación.
- test:	Creación o actualización de pruebas.
- style:	Cambios de formato, indentación o lint.
- merge-branch:	Unificación de ramas.

### Ejemplo de formato

```bash
git commit -m "feat: agregar componente de login"
git commit -m "fix: corregir cálculo de total en ventas"
git commit -m "refactor: mejorar estructura del módulo de productos"
git commit -m "docs: actualizar guía de instalación"
```

## 🧰 Formato de PR (pull request)

### Descripción
(Explica brevemente qué hace este PR)

## Tipo de cambio
- [ ] Nueva característica
- [ ] Corrección de error
- [ ] Refactor
- [ ] Documentación
- [ ] Otro (especificar)

## Checklist
- [ ] Probado localmente
- [ ] Revisado por al menos 2 devs
- [ ] Sin conflictos con `dev`
