# 🚀 Mi Primer Workflow con GitHub Actions

![CI Pipeline](https://github.com/aniapalominoq/mi-primer-workflow/actions/workflows/ci.yml/badge.svg)

Proyecto de práctica para aprender **CI/CD con GitHub Actions**, construyendo diferentes workflows utilizados en proyectos reales de DevOps.

---

# 📌 Objetivo

Aprender los fundamentos de **Integración Continua (CI)** y **Despliegue Continuo (CD)** utilizando GitHub Actions, creando workflows independientes para diferentes escenarios.

---

# 🛠 Tecnologías

- Git
- GitHub
- GitHub Actions
- Bash
- YAML
- Node.js
- npm

---

# 📂 Estructura del proyecto

```text
mi-primer-workflow/
│
├── .github/
│   └── workflows/
│       ├── ci.yml
│       ├── matrix.yml
│       ├── pipeline.yml
│       ├── pages.yml
│       ├── manual-inputs.yml
│       ├── secrets-demo.yml
│       └── cache.yml
│
├── test.sh
├── docs/
│   └── index.html
├── package.json
└── README.md
```

---

# 📚 Workflows implementados

## ✅ CI Pipeline

- Ejecuta automáticamente con `push` y `pull_request`
- Checkout del repositorio
- Ejecución de pruebas
- Variables de entorno
- Validación del pipeline

---

## ✅ Matrix Strategy

Prueba el mismo proyecto en diferentes versiones de Node.js.

```text
Node 18

Node 20

Node 22
```

También se puede ejecutar en diferentes sistemas operativos:

```text
Ubuntu

Windows
```

Utilizando:

```yaml
strategy:
  matrix:
```

---

## ✅ Pipeline con needs

Se creó un pipeline secuencial utilizando dependencias entre jobs.

```text
Lint
 │
 ▼
Test
 │
 ▼
Deploy
```

Aprendiendo el uso de:

```yaml
needs:
```

---

## ✅ Workflow Manual

Se implementó un workflow ejecutable manualmente mediante:

```yaml
workflow_dispatch
```

Incluyendo parámetros personalizados (inputs):

- Nombre
- Ambiente
- Ejecutar pruebas

---

## ✅ Variables y Secrets

Se aprendió a utilizar:

- Repository Variables (`vars`)
- Repository Secrets (`secrets`)

Para almacenar información pública y credenciales de forma segura.

---

## ✅ Caché de Dependencias

Se agregó caché para acelerar la instalación de dependencias usando:

```yaml
cache: npm
```

reduciendo el tiempo de ejecución de futuros workflows.

---

## ✅ GitHub Pages

Se creó un workflow para desplegar automáticamente un sitio estático en GitHub Pages después de cada `push` a la rama `main`.

---

# ⚙ Ejemplo de flujo CI/CD

```text
git push
     │
     ▼
GitHub Actions
     │
     ▼
Lint
     │
     ▼
Tests
     │
     ▼
Build
     │
     ▼
Deploy
```

---

# 📚 Conceptos aprendidos

- Workflows
- Jobs
- Steps
- Runners
- Triggers (`push`, `pull_request`, `workflow_dispatch`)
- Variables de entorno (`env`)
- Repository Variables (`vars`)
- Repository Secrets (`secrets`)
- Matrix Strategy
- Jobs en paralelo
- Jobs secuenciales con `needs`
- Caché de dependencias
- GitHub Pages
- CI (Continuous Integration)
- CD (Continuous Deployment)

---

# 🚀 Próximos pasos

Este repositorio continuará creciendo con nuevos laboratorios relacionados con DevOps:

- Docker
- Docker Hub
- Kubernetes
- Terraform
- Jenkins
- Automatización de despliegues

---

## 👩‍💻 Autora

**Melania Palomino**

Proyecto desarrollado como laboratorio de aprendizaje de **GitHub Actions** y **DevOps**.