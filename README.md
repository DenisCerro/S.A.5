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

```xml
<record id="grupo_bibliotecario" model="res.groups">
    <field name="name">Bibliotecario</field>
    <field name="users" eval="[(4, ref('base.user_admin'))]" />
</record>
