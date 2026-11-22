# Proyecto Gestión de Banda — Solana (Devnet)

Programa en Anchor (`gestion_banda`) y archivos de configuración inicial para integrar en el frontend (`Registro-Ventas-Solana-App`).

- **Program ID (Devnet):** `BHwvjDbEvoFhdoA7iSsYCBn56WcDDWiQYn8btbuE7SAo`

## Cómo trabajar con Git y tu repositorio

1. Clona el repositorio template del frontend:
   ```bash
   git clone https://github.com/WayLearnLatam/Registro-Ventas-Solana-App.git
   cd Registro-Ventas-Solana-App
   npm install
   ```
2. Copia `frontend/idl.json`, `frontend/scripts/contrato-idl.mjs` y `frontend/scripts/verificar-contrato.mjs` desde este paquete hacia tu repositorio clonado.
3. Ejecuta la importación del IDL y generación del cliente Codama:
   ```bash
   npm run configurar:idl -- ./idl.json --program-id BHwvjDbEvoFhdoA7iSsYCBn56WcDDWiQYn8btbuE7SAo
   ```
4. Revisa los cambios con Git (`git status`, `git diff`) y sube tu avance a tu propio repositorio remoto en GitHub (`git remote set-url origin <TU_REPO_URL>` o crea un repositorio nuevo).

## Árbol de PDAs
- `Material` (raíz): `[b"material", nombre_banda.as_bytes(), owner.key().as_ref()]`
- `Puesto`: `[b"puesto", material.key().as_ref(), nombre_puesto.as_bytes()]`
- `Integrante`: `[b"integrante", puesto.key().as_ref(), id_integrante.to_le_bytes().as_ref()]`
