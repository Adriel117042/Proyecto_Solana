# Gestión Banda 🎵

Aplicación web descentralizada (dApp) construida sobre la red de **Solana** para administrar bandas musicales, gestionando sus puestos, integrantes, puntuaciones de experiencia y materiales en cadena.

## 🚀 Características Principales

* **Consulta en modo lectura:** Localiza cualquier banda por su nombre y dirección de autoridad sin necesidad de firmar transacciones.
* **Creación de bandas y puestos:** Registra la estructura de tu agrupación directamente en Solana.
* **Gestión de integrantes:** Alta, modificación de experiencia y baja de miembros con firma de wallet.

---

## 📸 Capturas de Pantalla

### 🔍 Localización y consulta de bandas
 Permite consultar la información pública de una banda ingresando su nombre y la wallet de la autoridad.

![Localizar Banda](docs/imagenes/localizar-banda.png)

### ⚙️ Operaciones On-Chain
 Módulo interactivo con firma de transacciones para crear bandas, puestos, registrar integrantes, modificar puntuaciones o dar de baja miembros.

![Operaciones On-Chain](docs/imagenes/operaciones.png)

---

## 🛠️ Tecnologías Utilizadas

* **Frontend:** React + TypeScript + Vite + Tailwind CSS
* **Blockchain:** Solana (Web3.js, Codama IDL client generation)
* **Smart Contracts / Program:** `gestionBanda`

---

## ⚡ Instalación y Ejecución Local

1. **Clonar el repositorio e instalar dependencias:**
   ```bash
   npm install
