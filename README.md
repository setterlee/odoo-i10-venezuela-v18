# Localización de Odoo 18 para Venezuela

Bienvenido al repositorio oficial de la localización de **Odoo 18** para **Venezuela**. Este proyecto tiene como objetivo adaptar Odoo a los requisitos legales, fiscales y comerciales específicos del país, ofreciendo una solución completa para empresas venezolanas que deseen implementar este poderoso ERP.

## Objetivos

Este proyecto busca desarrollar:

- Configuración de impuestos según la normativa venezolana (IVA, ISLR, entre otros).
- Gestor de retenciones fiscales.
- Adaptación de formatos legales (facturas, libros de compra y venta, etc.).
- Módulos para el manejo de moneda dual (Bolívares y dólares).
- Herramientas para ajuste por inflación.
- Cumplimiento con las normativas del SENIAT.
- Configuración de períodos fiscales y ajustes contables.
- Localización bancaria (bancos y códigos SWIFT específicos de Venezuela).

## Requisitos

Antes de instalar este módulo (una vez desarrollado), asegúrate de contar con:

- **Odoo 18** instalado.
- Python 3.8 o superior.
- Dependencias adicionales necesarias para los módulos de localización (ver documentación futura).

## Progreso del Desarrollo

El proyecto está en sus primeras etapas. Las siguientes tareas están en curso:

1. Investigación de requisitos legales y fiscales en Venezuela.
2. Diseño del esquema de datos para impuestos y retenciones.
3. Creación de los primeros módulos de configuración.
4. Desarrollo de formatos legales iniciales.

## Contribuciones

Este es un proyecto de código abierto y agradecemos tus contribuciones. Para colaborar:

1. Haz un fork del repositorio.
2. Crea una rama con tu funcionalidad o corrección:

   ```bash
   git checkout -b mi-nueva-funcionalidad
   ```

3. Realiza tus cambios y súbelos:

   ```bash
   git commit -m "Descripción de los cambios"
   git push origin mi-nueva-funcionalidad
   ```

4. Abre un Pull Request en este repositorio.

### Gitflow Localización Odoo 18 VE

#### Ramas principales
1. **`main`**:
   - Contiene el código en producción.
   - Siempre estable y funcional.

2. **`develop`**:
   - Rama principal para integrar desarrollos.
   - Contiene el código listo para pruebas y lanzamientos.

#### Ramas de desarrollo
1. **`feature/*`**:
   - Cada nueva funcionalidad o ajuste debe desarrollarse en una rama `feature/`.
   - Ejemplo: `feature/add-tax-module`, `feature/fix-rif-validation`.

2. **`hotfix/*`**:
   - Ramas para arreglar errores críticos encontrados en producción.
   - Se crean desde `main` y se fusionan tanto en `main` como en `develop`.

#### Flujo de Trabajo

1. **Nueva funcionalidad**
   - Crea una rama `feature/` basada en `develop`:
     ```bash
     git checkout develop
     git pull
     git checkout -b feature/add-tax-module
     ```

   - Realiza cambios, comités frecuentes, y sube la rama:
     ```bash
     git add .
     git commit -m "feat: add tax calculation module"
     git push origin feature/add-tax-module
     ```

   - Abre un *pull request* (PR) desde la rama `feature/` hacia `develop`.

2. **Preparar para producción**
   - Cuando todo esté listo para producción, fusiona `develop` en `main`:
     ```bash
     git checkout main
     git pull
     git merge develop
     git push origin main
     ```

3. **Arreglo de errores críticos**
   - Si hay un error en producción, crea una rama `hotfix/` desde `main`:
     ```bash
     git checkout main
     git pull
     git checkout -b hotfix/fix-rif-validation
     ```

   - Corrige el error, realiza un PR hacia `main` y `develop`.

#### Reglas básicas
1. **Nombres claros para ramas**:
   - Usa nombres descriptivos en las ramas `feature/` y `hotfix/`.

2. **Estandarización de commits**:
   - Sigue un formato consistente como:
     - `feat: add tax calculation`
     - `fix: correct RIF validation bug`

3. **Integración continua**:
   - Fusiona ramas frecuentemente para evitar conflictos.

---

## Licencia

Este proyecto estará licenciado bajo la [MIT License](LICENSE).


## Desarrolladores Principales:

- [Marco Nuñez](https://github.com/setterlee)
- [Nerdo Pulido](https://github.com/nerdop44)



---

¡Gracias por unirte a este esfuerzo para mejorar la adopción de Odoo en Venezuela! 🎉
