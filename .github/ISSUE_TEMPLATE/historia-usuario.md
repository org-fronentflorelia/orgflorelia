# HU-01 - Registrar hoja de vida

## Historia de usuario

**Como** usuario que busca oportunidades laborales,
**quiero** registrar mi hoja de vida en la plataforma EMPLEATE,
**para** proporcionar mi información personal, académica y laboral y poder participar en oportunidades de empleo.

## Descripción

El sistema debe permitir al usuario diligenciar y registrar su hoja de vida mediante un formulario. La información registrada debe quedar almacenada en la base de datos para su posterior consulta y revisión.

## Criterios de aceptación

* [ ] El usuario debe poder ingresar su dirección.
* [ ] El usuario debe poder registrar su información de educación.
* [ ] El usuario debe poder adjuntar un soporte de educación en formato PDF.
* [ ] El usuario debe poder registrar su experiencia laboral.
* [ ] El usuario debe poder adjuntar un soporte de experiencia laboral en formato PDF.
* [ ] El usuario debe poder registrar los idiomas que domina.
* [ ] El usuario debe poder registrar información sobre sus antecedentes penales.
* [ ] El usuario debe poder registrar sus habilidades.
* [ ] Todos los campos requeridos deben ser diligenciados antes de enviar el formulario.
* [ ] Los soportes de educación y experiencia deben ser archivos PDF.
* [ ] La información debe almacenarse correctamente en la base de datos.
* [ ] La hoja de vida debe quedar inicialmente en estado **Pendiente**.
* [ ] El sistema debe mostrar un mensaje confirmando que la hoja de vida fue registrada correctamente.

## Datos de la hoja de vida

| Campo                  | Tipo  | Obligatorio |
| ---------------------- | ----- | ----------- |
| Dirección              | Texto | Sí          |
| Educación              | Texto | Sí          |
| Soporte de educación   | PDF   | Sí          |
| Experiencia laboral    | Texto | Sí          |
| Soporte de experiencia | PDF   | Sí          |
| Idiomas                | Texto | Sí          |
| Antecedentes penales   | Texto | Sí          |
| Habilidades            | Texto | Sí          |
| Estado                 | Texto | Automático  |

## Estado inicial

Al registrarse una nueva hoja de vida, el sistema debe establecer automáticamente el estado:

`Pendiente`

Los estados disponibles son:

* `Pendiente`
* `Aprobada`
* `Rechazada`

## Resultado esperado

Una vez enviada correctamente la información, el sistema debe guardar la hoja de vida en la base de datos y mostrar al usuario un mensaje indicando que el registro fue exitoso y que la hoja de vida quedó pendiente de revisión.

## Prioridad

**Alta**

## Requerimiento relacionado

**Registrar hoja de vida**
