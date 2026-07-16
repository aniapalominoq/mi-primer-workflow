# 🚀 Mi Primer Workflow con GitHub Actions

Mi primer proyecto de CI/CD utilizando GitHub Actions.

## 📌 Objetivo

Aprender a crear un pipeline automático que se ejecute cada vez que se realiza un `git push`.

---

## 🛠 Tecnologías

- Git
- GitHub
- GitHub Actions
- Bash
- YAML

---

## 📂 Estructura del proyecto

```text
mi-primer-workflow/
│
├── .github/
│   └── workflows/
│       └── ci.yml
│
├── test.sh
│
└── README.md
```

---

## ⚙ Flujo del Pipeline

```text
git push
     │
     ▼
GitHub Actions
     │
     ▼
Checkout del código
     │
     ▼
Dar permisos al script
     │
     ▼
Ejecutar test.sh
     │
     ▼
Pipeline exitoso
```

---

## 📷 Resultado esperado

El workflow aparece en la pestaña **Actions** del repositorio y ejecuta automáticamente:

- Checkout del código
- Información del runner
- Permisos al script
- Ejecución de pruebas
- Pipeline completado

---

## 📚 Lo aprendido

- Crear un Workflow
- Crear un archivo YAML
- Crear un Pipeline
- Ejecutar un script Bash
- Comprender CI/CD con GitHub Actions

---

Proyecto realizado como práctica de DevOps.