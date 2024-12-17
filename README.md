# Módulos Odoo - Activitats d'ERP-CRM

Este repositorio contiene las soluciones a diversas activitats sobre la creación y ampliación de módulos en **Odoo**. Cada actividad aborda un caso práctico diferente, implementando modelos, relaciones, vistas y configuraciones de seguridad.

## Tabla de Contenidos

1. [Activitat 01 - Llista de Tasques amb Kanban i Calendar](#activitat-01---llista-de-tasques-amb-kanban-i-calendar)
2. [Activitat 02 - Biblioteca de Còmics](#activitat-02---biblioteca-de-còmics)
3. [Activitat 03 - Gestió d'Hospital](#activitat-03---gestió-dhospital)
4. [Activitat 04 - Gestió de Cicles Formatius](#activitat-04---gestió-de-cicles-formatius)

---

## Activitat 01 - Llista de Tasques amb Kanban i Calendar

### Descripció
Aquest mòdul amplia un exemple senzill de llista de tasques per incloure les següents funcionalitats:

- **Vista Kanban**: Una nova vista per visualitzar les tasques en format "Kanban".
- **Vista Calendar**: Les tasques ara tenen assignada una data i es poden visualitzar en una vista "Calendar".

### Característiques
- **Nova propietat**: `data_assignada` per a les tasques.
- **Seguretat**: Configuració de grups i permisos bàsics.

  
Activitat 02 - Biblioteca de Còmics
Descripció
Aquest mòdul amplia l'exemple d'una biblioteca de còmics per permetre la gestió de socis i exemplars de còmics per a préstecs.

Models Implementats
Soci: Emmagatzema nom, cognom i identificador.
Còmic: Serveix com a referència per a la informació dels còmics.
Exemplar: Registra a qui està prestat un còmic, amb dates de préstec i devolució.
Validacions
La data de préstec no pot ser posterior a la data actual.
La data de tornada no pot ser anterior a la data actual.
Activitat 03 - Gestió d'Hospital
Descripció
Aquest mòdul implementa una solució per gestionar pacients, metges i diagnòstics en un hospital.

Models Implementats
Pacient

Nom i cognoms
Símptomes
Metge

Nom i cognoms
Número de col·legiat
Atenció

Relació entre metges i pacients
Diagnòstic
Relacions
Un pacient pot ser atès per diversos metges.
Un metge pot atendre diversos pacients.
Activitat 04 - Gestió de Cicles Formatius
Descripció
Aquest mòdul gestiona els cicles formatius d'un institut, incloent-hi alumnes, professors i mòduls.

Models Implementats
Cicle Formatiu

Representa un cicle formatiu en un institut.
Mòdul

Relacionat amb el cicle formatiu, alumnes matriculats i el professor que l'imparteix.
Alumne

Relacionat amb els mòduls matriculats.
Professor

Relacionat amb els mòduls que imparteix.
Seguretat
Els usuaris amb el rol "Director" poden modificar tots els registres.
Els usuaris amb rol "Professor" poden veure (només lectura) les dades dels professors.
